```python
var1 = 10
print(hex(id(var1)))
0x103df6ad8
var1 = 100
print(hex(id(var1)))
0x103df7618
```

**Question 1**  
When you reassign a new value to a variable Python will use a new memory slot because of how Python is designed. 
Even if you reassigned the same value Python would still use a new memory slot.  

```python
var2 = 100
print(hex(id(var2)))
0x103df7618
```
**Question 2**  
It reused the same address as the first time i assigned the value of 100  

```python
str1 = "Hello"
str2 = "World"
print(hex(id(str1[0])), hex(id(str1[1])))
0x103e06140 0x103e066b0
print(hex(id(str1[2])), hex(id(str1[3])))
0x103e06800 0x103e06800
print(hex(id(str1[4])))
0x103e06890
print(hex(id(str2[0])), hex(id(str2[1])))
0x103e06410 0x103e06890
print(hex(id(str2[2])), hex(id(str2[3])), hex(id(str2[4])))
0x103e06920 0x103e06800 0x103e06680
```
| Address in hexadecimal | Char |
| ---------------------- | ---- |
| #  0x103e06140         |  H    |
| #  0x103e066b0         |  e    |
| #  0x103e06800         |  l    |
| #  0x103e06800         |  l    |
| #  0x103e06890         |  o    |
| #  0x103e06410         |  W    |
| #  0x103e06890         |  o    |
| #  0x103e06920         |  r    |
| #  0x103e06800         |  l    |
| #  0x103e06680         |  d    |  

