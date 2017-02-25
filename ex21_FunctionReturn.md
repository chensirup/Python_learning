# FunctionReturn

### Write `ex21.py`

```
def add(a,b):
    print("ADDING %d+%d"%(a,b))
    return a+b

def subtract(a,b):
    print("SUBTRACTING %d-%d"%(a,b))
    return a-b

def multiply(a,b):
    print("MULTIPLYING %d*%d"%(a,b))
    return a*b

def divide(a,b):
    print("DIVIDING %d/%d"%(a,b))
    return a/b

  
print("Let's do some math with just functions!")

age=add(30,5)
height=subtract(78,4)
weight=multiply(90,2)
iq=divide(100,2)

print("Age:%d,Height:%d,Weight:%d,IQ:%d"%(age,height,weight,iq))


#A puzzle for the extra credit,type it in anyway.

print("Here is a puzzle.")

what=add(age,subtract(height,multiply(weight,divide(iq,2))))

print("That becomes:",what,"Can you do it by hand?")
```

- Runed

```
PS F:\mystuff> python ex21.py
Let's do some math with just functions!
ADDING 30+5
SUBTRACTING 78-4
MULTIPLYING 90*2
DIVIDING 100/2
Age:35,Height:74,Weight:180,IQ:50
Here is a puzzle.
DIVIDING 50/2
MULTIPLYING 180*25
SUBTRACTING 74-4500
ADDING 35+-4426
That becomes: -4391.0 Can you do it by hand?
```
***
### The error
- 1st

```
PS F:\mystuff> python ex21.py
  File "ex21.py", line 18
    print("Let's do some math with just functions！“）
                                                    ^
SyntaxError: EOL while scanning string literal

---
PS F:\mystuff> python ex21.py
  File "ex21.py", line 18
    print("Let's do some math with just functions！"）
                                                   ^
SyntaxError: invalid character in identifier

---
PS F:\mystuff> python ex21.py
  File "ex21.py", line 18
    print("Let's do some math with just functions!"）
                                                   ^
SyntaxError: invalid character in identifier
```

- 2nd

```
PS F:\mystuff> python ex21.py
Let's do some math with just functions!
ADDING 30+5
SUBTRACTING 78-4
MULTIPLYING 90*2
DIVIDING 100/2
Age:35,Height:74,Weight:180,IQ:50
Here is a puzzle.
Traceback (most recent call last):
  File "ex21.py", line 32, in <module>
    what=add(age,subtract(height,muliply(weiht,divide(iq,2))))
NameError: name 'muliply' is not defined

---
PS F:\mystuff> python ex21.py
Let's do some math with just functions!
ADDING 30+5
SUBTRACTING 78-4
MULTIPLYING 90*2
DIVIDING 100/2
Age:35,Height:74,Weight:180,IQ:50
Here is a puzzle.
Traceback (most recent call last):
  File "ex21.py", line 32, in <module>
    what=add(age,subtract(height,multiply(weiht,divide(iq,2))))
NameError: name 'weiht' is not defined
```

### Thinking

More `return`.

***
- Changelog
- 2017-02-25 12:55:42 ©陈sir