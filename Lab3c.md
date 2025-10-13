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
my_list_ten_mem = id(my_list_ten)

for item in my_list_ten:
    print(id(item))
```
Results:
4375620720
4375620816
4375620912
4375790512
4375790576
4375621104
4375620720
4375620816
4375621392
4375621488
The list of mememory locations will have repeats for the items that repeat in my list

**Question 1e**
```python
my_list_ten = ["apple", "banana", "orange", "strawberry", "blueberry", "kiwi", "apple", "banana", "pear", "plum"]
my_list_ten.clear()
```

**Question 1f**



