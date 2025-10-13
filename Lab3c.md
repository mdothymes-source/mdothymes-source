## Lists in Python ##

**Question 1a**  
```python
my_list = list(range(0,100))
print(my_list)
print(type(my_list))

my_list.append(100) # adding 100 to end of the list
print(my_list)

my_list.pop() # removes the last item in the list
print(my_list)

my_list.insert(0, '-1') # adding -1 to my list of 100
print(my_list)

my_list.clear() #clears my list completely
print(my_list)
```
**Question 1b**  
```python
my_list = list(range(0,10))
last_three = my_list[7:] # making new list with last three items
del my_list[7:] # deleting the last three items in my list

last_three.reverse() # reversing new list to add them in order they were removed

for x in last_three:
    my_list.insert(0, x)

print(my_list)
```

**Question 1c**
6 is my guess
```python
my_list = [[1, 2]]
list_length = len(my_list) * 3
print(list_length)
```
Using pythong the answer should be "3", the double brackets make a list within a list causing it to have just 1 element

**Question 1d**
```python
my_list_ten = ["apple", "banana", "orange", "strawberry", "blueberry", "kiwi", "apple", "banana", "pear", "plum"]
my_list_ten_mem = [] # creating an empty list to fill with the memory ids

for item in my_list_ten: # stepping through the list of ten
    my_list_ten_mem.append(id(item)) # adding each item's memory id to the empty list
print(my_list_ten_mem) # printing the new list i created
```
Results:  
"4375178016", "4375178304", 4375178400, 4375348144, 4375348208, 4375178592, "4375178016", "4375178304", 4375178880, 4375178976

The list of mememory locations will have repeats for "apple" and "banana"

**Question 1e**
```python
my_list_ten = ["apple", "banana", "orange", "strawberry", "blueberry", "kiwi", "apple", "banana", "pear", "plum"]
my_list_ten.clear() # this clears the list
```

**Question 1f**
```python
# my_list_ten = ["apple", "banana", "orange", "strawberry", "blueberry", "kiwi", "apple", "banana", "pear", "plum"]
# my_list_ten_mem = [] # creating an empty list to fill with memory ids

# for item in my_list_ten: # stepping through the list of ten
#    my_list_ten_mem.append(id(item)) # adding each item's memory id to the empty list
# print(my_list_ten_mem) # printing the new list i created

my_list_ten = ["apple", "banana", "orange", "strawberry", "blueberry", "kiwi", "apple", "banana", "pear", "plum"]
my_new_list = ["apple", "banana", "orange", "strawberry", "blueberry", "kiwi", "apple", "banana", "pear", "plum"]
my_list_ten_mem = [] # creating an empty list to fill with memory ids
my_new_list_mem = [] # creating an empty list for my new lists memory

for item in my_list_ten: # stepping through the list of ten
    my_list_ten_mem.append(id(item)) # adding each item's memory id to the empty list

for new_item in my_new_list:
    my_new_list_mem.append(id(new_item))

print(my_list_ten_mem) # printing the new list i created
print(my_new_list_mem) # printing the memory for the new list to compare
```
Results:
[4379142944, 4379143232, 4379143328, 4379313072, 4379313136, 4379143520, 4379142944, 4379143232, 4379143808, 4379143904]
[4379142944, 4379143232, 4379143328, 4379313072, 4379313136, 4379143520, 4379142944, 4379143232, 4379143808, 4379143904]
The memory locations for the two seperate lists are exactly the same. No wasted memory space

**Question 1g**
```python
import copy

x = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
y = copy.deepcopy(x)

print(y)
```
I would use the import copy to do a deep copy. This will allow me to change y without effecting x



