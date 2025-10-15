## Funtions in Python ##

**Question 1a**
```python
def is_integer(input_string):  ##this function will check to see if the user input is an actual number
    try:
        int(input_string)
        return True
    except ValueError:
        print("Error: I can only convert numbers/integers")
        return False

def kpl_to_mpg(x):  ##created a function to convert kpl to mpg
    converted_kpl = float(kpl) * 2.35
    print(f"{kpl} kpl is equal to {converted_kpl} mpg.")

def mpg_to_kpl(y):  #created another function to convert mpg to kpl
    converted_mpg = float(mpg) / 2.35
    print(f"{mpg} mph is equal to {converted_mpg} kpl.")

# asking the user to choose between converting to kpl or mpg
question_1 = input("Do you want to convert to kpl or mpg? ")

if question_1 == "kpl": #if the user answers kpl, the program will ask them to enter a mpg
    mpg = (input("Enter your current mpg: ")) #converting input into a float
    if is_integer(mpg):
        mpg_to_kpl(mpg)  # calling the function
elif question_1 == "mpg":
    kpl = (input("Enter your current kpl: "))
    if is_integer(kpl):
        kpl_to_mpg(kpl)
else:
    print("Invalid response") #error handler for user input
```
**Question 1b**
```python
def reverse_order(*name):
    print(name)

user_input = input("Enter as many numbers as you like: ")
numbers = user_input.split()
num_order = sorted(numbers, reverse=True)

reverse_order(num_order)
```

**Question 1c**
Anything inside the function that used those parameters could possibly be changed. Using the global keyword ensure your changes are seen outside the function

**Question 1d**
After func_1 is run x will still be equal to 5, but once func_2 is run, x will now be equal to 2 because of the global keyword that allows it to be seen outside the function

**Question 2**
```python
def my_func(a,b,**c): #i fixed this code be removing the second star next to the variable c, this will allow it to accept the other 4 values as a tuple
  print(c)
```

```python
def my_func_global():
  x = 100

global x
x = 10
my_func_global()
print(x)
```
Answer: 10 is being printed because it was given a value of 10 globally, so it 10 inside and outside of the function

my_func(1,2,3,4,5,6)


