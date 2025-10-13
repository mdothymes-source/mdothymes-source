##Loops##

**Question 1a**
'''python
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


