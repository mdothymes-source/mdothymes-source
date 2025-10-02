## Lab3a Decision Statements

**Question 1**  
```python
def main():
    # Printable ASCII characters range from 32 (space) to 126 (~)
    for code in range(32, 127):
        char = chr(code)
        # Use repr to make space and quotes visible, this line will print
        # the character and the ascii code
        print(f"{repr(char)} = {code}")

if __name__ == "__main__":
    main()
```

**Question 5a**
```python
# Read 3 numbers
number1 = int(input("Enter the first number: "))
number2 = int(input("Enter the second number: "))
number3 = int(input("Enter the third number: "))

# Choose the larger number
if (number1 > number2) and (number1 > number3)
    larger_number = number1
elif (number2 > number1) and (number2 > number3)
    larger_number = number2
else:
    larger_number = number3

# Print the result
print("The largest number is:", larger_number)
```
**Question 5b**  
```python
#######################
# Approach 1
user_input = int(input("Enter any number: "))
if user_input % 2 == 0:
    print("Your number is EVEN")
else:
    print("Your number is ODD")
#######################
# Approach 2
user_input = int(input("Enter any number: "))
if user_input & 1 == 0:
    print("Your number is EVEN")
else:
    print("Your number is ODD")
#######################
# Approach 3, checking the remainder of the number when dividing by 10 and 
# comparing it to a list of even numbers. 
user_input = int(input("Enter any number: "))
remainder_check = user_input % 10
my_list = [0, 2, 4, 6, 8]
if remainder_check in my_list:
    print("EVEN")
else:
    print("ODD")
#######################
```
**Question 5c**
```python
grade_input = int(input("What is your current grade?: ")) #user input for current grade
if grade_input >= 90:
    print("Grade A: Work of genuinely superior quality.") #prints A if user input is above 90
elif grade_input >= 80:
    print("Grade B: Passing performance falls approximately in the upper distribution of "
          "passing grades.")
elif grade_input >= 71:
    print("Grade C: Passing performance falls approximately in the center of the distribution"
          " of all passing grades.")
elif grade_input >= 65:
    print("Grade D: Passing performance falls approximately in the lower distribution of "
          "passing grades.")
else:
    print("Grade F: Failing performance that does not satisfy the basic requirements of the course"
        " and needs to be improved in significant ways.")
```
**Question 5d**
```python
user_input = str(input("Please type in AND, OR, or NOT:"))
if user_input == "NOT":
    print("--- NOT Truth Table ---")
    print("Input | Output")
    print("-----------------------")
    print("   A   |   Y  ")
    print("   0   |   1  ")
    print("   1   |   0  ")
else:
    print("You did not type AND, OR, or NOT")
```

**Question 5e**
```python
user_input = int(input("Enter any number, I will tell you if it is ODD or EVEN: "))
#this will check and compare the last number in the binary representation of the input
if user_input & 1 == 0:
    print("Your number is EVEN")
else:
    print("Your number is ODD")
```
**Question 6**
```python
name = input("What's your name? ")
time = int(input("What time is it? "))

if (time < 1200):
    print("Hi "+name + ", good morning!")
# if the above operation is false the elif below will check to see if the time is less than 1800
elif (time < 1800):
    print("Hi "+name + ", good afternoon!")
# if the elif above is false the elif below will compare time to 1800
elif (time > 1800):
    print("Hi "+name + ", good evening!")
# the statement below will print good bye if none of the above conditions are met
else:
    print("Good Bye," + name)
```

**Question 7**  
one  
two  
Because the elif and else was not executed because the condition of the first "if" in the nested if were true.

