## Tuples ##

**Question1a**
```python
# Get 5 individual inputs
item1 = input("Enter the first number: ")
item2 = input("Enter the second number: ")
item3 = input("Enter the third number: ")
item4 = input("Enter the fourth number: ")
item5 = input("Enter the fifth number: ")

# Create a tuple from the inputs
my_tuple = (item1, item2, item3, item4, item5)

print("Your tuple:", my_tuple)
```

**Question 1b**  
```python
tuple_single = (1,)
print(tuple_single)
```

**Question 1c**
```python
my_tuple = (1,2,3,4,3,2,1,2,3,5,4,3,2,1)
ones = my_tuple.count(1)
twos = my_tuple.count(2)
threes = my_tuple.count(3)
fours = my_tuple.count(4)
fives = my_tuple.count(5)

print("There are", ones, "1s,", twos, "2s,", threes, "3s,", fours, "4s, and", fives, "5s in my_tuple.")
#for x in my_tuple:
#    print(x)
```

**Question 1d**
```python
my_tuple = (1,2,3,4,3,2,1,2,3,5,4,3,2,1)
print(id(my_tuple))

my_tuple = my_tuple + my_tuple
print(id(my_tuple))
```
Results: 
4307929824
4308075648
The two different IDs show that the my_tuple from the previous question is different than the new one
