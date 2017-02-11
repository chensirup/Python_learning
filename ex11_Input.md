# Input code

- Software's work
    - 01 : input of recipient
    - 02 : change input
    - 03 : print out the changed input


###  What's the `raw_input` work?

- **Write new code**

```
print("How old are you?"),
age=raw_input()
print("How tall are you?"),
height=raw_input()
print("How much do you weight?"),
weight=raw_input()

print("So, you're %r old,%r tall and %r heavy."%(age,height,weight))
```

- **Run code**

```
PS F:\mystuff> python ex11.py
How old are you?
Traceback (most recent call last):
  File "ex11.py", line 10, in <module>
    age=raw_input()
NameError: name 'raw_input' is not defined
```

**Waring : That's sth wrong.**

Search the code `raw_input` ,and fined it's the new code `input` by Python3.x version, fixed the code.

```
print("How old are you?"),
age=input()
print("How tall are you?"),
height=input()
print("How much do you weight?"),
weight=input()

print("So, you're %r old,%r tall and %r heavy."%(age,height,weight))

```

- **Run again**

```
PS F:\mystuff> python ex11.py
How old are you?
- 
```

 Tips : We must input **data** by ourselves.

- 
    - input data 
    - Then enter one by one until the last line.
Last result is following :

```
PS F:\mystuff> python ex11.py
How old are you?
30
How tall are you?
65
How much do you weight?
264
So, you're '30' old,'65' tall and '264' heavy.
```

Congratulations, I did it.
***
### **Thinking :**
- It's only code `input` by Python3.x, that's not `raw_input`.
- It must to manully input one by one.
***
- Changelog
- 2017-02-11 17:17:41 ©陈sir
