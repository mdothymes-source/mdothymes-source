## Lab 2b Python literals  

**Question 1**  
print(5 + 2 - 2)  
Answer:  5  
______________________
print(5 / 2)  
Answer:  2.5  
______________________
print(6 // 2) # // integer division  
Answer:  3  
______________________
print(2. * 3)  
Answer:  6.0  
______________________
print(2 < 4)  
Answer:  .5   
______________________
print(2 >= 2)  
Answer:  True  
______________________
print("Hello"+"World")  
Answer:  HelloWorld   
______________________
print("bla" * 3)  
Answer: Error  
______________________
print(2 * 3 ** 3)  
Answer:  54    
______________________
print(5 * 25 // 13 + 100 / 2 % 13 // 2)  
Answer:  14.0   
______________________
print(2 * 3 % 5)  
Answer:  1    
______________________
print((2 % -4), (2 % 4), (2 ** 3 ** 2))  
Answer:  -2 2 512  

**Question 2**  
type("Hello")
Answer:  <class 'str'>
type(1+"2")  
______________________
type(1.)  
Answer:  <class 'float'>
______________________
type('A')  
Answer:  <class 'str'>
______________________
type(500)  
Answer:  <class 'int'>
______________________
type(True)  
Answer:  <class 'bool'>  
______________________
type("False")  
Answer:  <class 'str'>  

**Question 3a/b**  
5 * 25 % 13 + 100 / -2 * 13 // 2 ** 3  
5 * 25 % 13 + 100 / -2 * 13 // **2 ** 3** (bold operation has number 1 priority)  
**5 * 25** % 13 + 100 / -2 * 13 // 8 (from left to right the bold is the next priority)  
**125 % 13** + 100 / -2 * 13 // 8 (from left to right bold is next highest priority)  
7 + **100 / -2** * 13 // 8   
7 + **-50 * 13** // 8  
7 + **-650 // 8**  
**7 + -82**  
-75  

**Question 3c**  
print(5 * 25 % 13 + 100 / -2 * 13 // 2 ** 3)  
-74
