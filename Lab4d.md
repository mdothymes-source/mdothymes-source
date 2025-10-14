## Dictionary in Python ##

**Question 1a**
```python
capitals = {"California": "Sacramento",
            "New York": "Albany",
            "Florida": "Tallahassee",
            "Texas": "Austin",
            "Nebraska": "Lincoln",
            "Georgia": "Atlanta",
            "Iowa": "Des Moines",
            "Ohio": "Columbus",
            "Utah": "Salt Lake City",
            "Arizona": "Phoenix"}
print(capitals)
```

**Question 1b**
```python
my_user_dict = {}

while True:
    key_input = input("Please enter the key you want to update: ")
    value_input = input(f"What is your '{key_input}': ")

    my_user_dict[key_input] = value_input
    print(my_user_dict)
    cont = input("Do you want to continue (y/n)?")
    if cont == "n":
        print("Have a nice day!")
        break # program will end if user enters "n"
```
Answer: You need zero keys to created a dictionary. I was able to create an empty dictionary

**Question 1c**

**Question 1d**
```python
my_list = [('Name', 'Sarah Connor'),
 ('Date of birth', '1 Jan 1980'),
 ('Address', '1000 Black Mountain Drive 92126'),
 ('Name', 'Jim Hawkins')]

my_dict = {}

for key, value in my_list:
    my_dict[key] = value

print(my_dict)
```
**Question 1e**
```python
sentence = ("The tiger (Panthera tigris) is a large cat and a "
            "member of the genus Panthera native to Asia. It has"
            " a powerful, muscular body with a large head and paws, "
            "a long tail and orange fur with black, mostly vertical"
            " stripes. It is traditionally classified into nine recent"
            " subspecies, though some recognise only two subspecies, "
            "mainland Asian tigers and the island tigers of the Sunda"
            " Islands.")

my_string = sentence.lower().split() #splitting string into seperate elements
my_dict = {}

for word in my_string:
    my_dict[word] = 1
print(len(my_dict)) # this will pring the number of items in the dictionary i created
``
**Question 2a**
```python
import copy

d_orig = {123:"Coconut"}
#using a deep copy will keep the values the same in original dictionary
#when changing the values of the copied dict
d_copy = copy.deepcopy(d_orig) 
print(d_orig)
print(d_copy)

d_copy[123] = "Lemon"
print(d_orig)
print(d_copy)
```
**Question 2b**
Answer: The code as presented changed the original value when i tried to change the copy
I added a deep copy and this allowed me to change the copy w/o affecting the original
(code prensented in 2a above)

**Question 2c**
```python
my_dict = {}
my_list = [1, 2, 3]
# This will raise the TypeError
my_dict[my_list] = "some_value"
```
Answer: in the code above i tried to use a list as keys for the dictionary and this gave me an unhashable error
since lists do not have a fixed hash value, this will not work. 
