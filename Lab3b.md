##Loops##

**Question 1a**  
```python  
n0 = int(input("Please enter a number greater than 0: "))  
  
while n0 > 0:  
    if n0 % 2 == 0:  
        n0 = n0 // 2
        print(n0)  
        if n0 == 1:  
            break  
    else:  
        n0 = 3 * n0 + 1  
        print(n0)  
        
print("Goodbye")  
```

**Question 1b**
```python
n0 = int(input("Please enter a number greater than 0: "))

while n0 > 0:
    if n0 % 2 == 0:
        n0 = n0 // 2
        print(n0)
        if n0 == 1:   
            break    ###This line is what fixed my infinite loop
    else:
        n0 = 3 * n0 + 1
        print(n0)

print("Goodbye")
```
**Question 1c**
```python
while True:

    num1 = int(input("Please enter the first number: "))
    num2 = int(input("Please enter the second number: "))

##while num1.is_integer() and num2.is_integer():

    math = input("Please choose between add, subtract, multiply, or divide: ")

    if math == "add":
        print("The answer is: ", num1 + num2)
    elif math == "subtract":
        print("The answer is: ", num1 - num2)
    elif math == "multiply":
        print("The answer is: ", num1 * num2)
    elif math == "divide":
        print("The answer is: ", num1 // num2)
    else:
        print("Please enter a valid operation.")
        continue

    usr_input1 = input("Would you like to continue? (y/n): ")
    if usr_input1 == 'y':
        continue
    elif usr_input1 == 'n':
        print("Have a good day!")
        break
    else:
        print('Invalid input, please enter "y" or "n".')
```

**Question 2a**  
```python
sentence = "to be, or not to be, that is the question."
unique = []
for char in sentence:
    if char not in unique:
        unique.append(char)

count = 0
for char in sentence:
    if char != " ":
        count = count + 1
print(sentence)
print("Total number of letters:", count)
print("Total number of distinct letters are:", len(unique))
print("t =", sentence.count('t'))
print("o =", sentence.count('o'))
```

