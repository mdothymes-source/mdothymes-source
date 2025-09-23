## Lab2d User input using input() function  

**Question 1a:**  
```python
kg_to_lbs = float(2.2)
weight_kg = float(input("Enter your weight in kilograms:"))
print("Your weight in pounds is:", weight_kg * kg_to_lbs)
```  

**Question 1b:**
```python
netBalance = float(input("Enter the net balance:"))
payment = float(input("What is the payment amount?"))
d1 = int(input("Number of days in the billing cycle:"))
d2 = int(input("How many days early is the payment?"))
int_rate = float(input("What is the current interest rate?"))
avg_daily_bal = netBalance * d1 - payment * d2 / d1
interest = avg_daily_bal * int_rate

print("Your interest is:", interest)
```

**Question 1c:**  
```python
x_avg = int(input("What was your average speed, Car A?"))
y_avg = int(input("What was your average speed, Car B?"))
x_time = float(input("How long was your trip, Car A?"))
y_time = float(input("How long was your trip, Car B?"))
x_dist = (x_avg * x_time)
y_dist = (y_avg * y_time)
# below im using a^2 + b^2 = c^2 to find the distance between Car A and Car B
distance = x_dist ** 2 + y_dist ** 2 
# i am using ** 0.5 to get the square root of distance 
print("Car A and Car B are", distance ** 0.5, "miles apart.")
```

**Question 2:**  
a. valid variable name but may not be the best idea because it can get confusing  
b. valid variable, they are allowed to start with an underscore  
c. not valid, not special characters in the variable names  
d. "print" is a keyword and cannot be used for variable names  
e. "False" is also a keyword that should not be used in variable names
