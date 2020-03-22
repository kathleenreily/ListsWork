# ListsWork
# Examples of applying and creating lists

# adding items in a list
def sum_wines(wine_prices):
  total_price = 0
  for wine_price in wine_prices:
    total_price += wine_price
  return total_price
print(sum_wines([13, 9, 12]))
# when printed:
34

# sum items in a list
def sum_cups(coffee_list):
  all_cups = 0
  for coffee in coffee_list:
    all_cups += coffee
  return all_cups
print(sum_cups([1,1,2]))
# when printed:
4

# find range
print(list(range(5)))
# when printed:
[0, 1, 2, 3, 4]


# updating lists
things = ['cats', 'dogs', 'rats', 14, [24, 'shoes'], 9]
things[2] = 'elephants'
print(things[2])
# when printed:
elephants

# here we are creating a sentence using one of the items in our list
trees = ['leaves', 'trunk', 'branches']
first_word = trees[0] 
print("the first word are '{}.'".format(first_word))
# when printed:
the first word are 'leaves.'

# counting number of values in a list using len() function
my_name = ['k', 'a', 't', 'h', 'l', 'e', 'e', 'n']
print(len(my_name))
# when printed
8

# .append() a list
list_2 = [114, 16, 'pavemment', 'colorado']
list_2.append(112)
print(list_2)
# printed:
[114, 16, 'pavemment', 'colorado', 112]

# .insert() a new value into a list
list_2 = [114, 16, 'pavemment', 'colorado']
list_2.insert(0, 'tree')
print(list_2)
# printed:
['tree', 114, 16, 'pavemment', 'colorado']

# .pop() function elimating values from a list
list_1 = ['shoes', 'people', 1, 2]
delet_item = list_1.pop()
print(delet_item)
2
print(list_1)
# printed:
2
['shoes', 'people', 1]

# index practicing with lists- identifying the number of the item placement in your list
list_2 = [114, 16, 'pavement', 'colorado']
print(list_2.index('pavement'))
# printed:
2

# .sort() practicing putting numbers and words in order
list_3 = ['shoes', 'people', 'Austin', 'Sanfran']
list_3.sort()
print(list_3)

numbers = [1,9,7,4]
numbers.sort()
print(numbers)

words = ['apples', 'pears', 'tomatoes', 'berries']
words.sort()
print(words)
# printed:
['Austin', 'Sanfran', 'people', 'shoes']
[1, 4, 7, 9]
['apples', 'berries', 'pears', 'tomatoes']

# for loops 
words = ['apples', 'pears', 'tomatoes', 'berries']
def fruits(color):
  for i in color:
    if color == 'red':
      return 'apple or tomato'
    elif color == 'blue':
      return 'berries'
    else:
      return 'pears'
fruits('red')
# called:
'apple or tomato'

# calculating the mean with if and for statements
grades_list = [79, 92, 98, 81]
def calculate_grade(score):
  total = 0
  for one in score:
    total += one
    avg = total/len(score)
  if 90 <= avg <= 100:
    return 'A'
  elif 80 <= avg <90:
    return 'B'
  elif 70 <= avg < 80:
    return 'C'
  elif 60 <= avg < 70:
    return 'D'
  else: 
    return 'F'
print(calculate_grade([92, 99, 98, 92]))
# printed:
A

# basic mean practice
lst = [79, 92, 98, 81]
def practice_mean(numbers):
  total = 0
  for i in numbers:
    total += i
    avg = total/len(numbers)
  return total
practice_mean(lst)
# called:
350

# slicing, then subtract and multiply  sublists
list_1 = [[8, 2], [9, 5], [3, 9], [14, 21]]
def calculate_total(list_1):
  subtract_list = []
  for one in list_1:
    subtract = one[0]-one[1]
    subtract_list.append(subtract)
  multiply_list = 1
  for item in subtract_list:
    multiply_list *= item
  return multiply_list
calculate_total(list_1)
# called:
1008

# multiply all items in a list
numbers_list = [2, 4, 6]
def multiply_items(numbers_list):
  multiply = 1
  for number in numbers_list:
    multiply *= number
  return multiply
multiply_items(numbers_list)
# called:
48

# Write a Python program to get the largest number from a list.
def largest_number(list_1):
  max_num = list_1[0]
  for item in list_1:
    if item > max_num:
      max_num = item
  return max_num
print(largest_number([-9, 12, 14, 28]))
# printed:
28

# Write a Python program to get the smallest number from a list.
def smallest_num_in_list(list_1):
    min_num = list_1[0]
    for item in list_1:
        if item < min_num:
            min_num = item
    return min_num
print(smallest_num_in_list([1, 2, -8, 0]))
# printed:
-8


