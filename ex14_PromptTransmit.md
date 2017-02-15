# Prompt Transmit

Today write new code include `argv` and `input`, like following:

```
from sys import argv

script,user_name=argv
prompt='>'

print("Hi %s, I'm the %s script."%(user_name,script))
print("I'd like to aks you a few questions.")
print("Do you like me %s"% user_name)
likes=input(prompt)

print("Where do you like %s?"%user_name)
lives=input(prompt)

print("What kind of computer do you have?")
computer=input(prompt)

print("""
Alright, so you said %r about liking me.
You live in %r. Not sure where that is.
And you have a %r computer.Nice.
"""%(likes,lives,computer))

```
- **There're some wrong like:**
    - 01 SyntaxError: invalid syntax
```
PS F:\mystuff> python ex14.py
  File "ex14.py", line 14
    print(What kind of computer do you have?")
                  ^
SyntaxError: invalid syntax
```

It's less `"` code.

- 
    - 02 ValueError:
```
PS F:\mystuff> python ex14.py
Traceback (most recent call last):
  File "ex14.py", line 3, in <module>
    script,user_name=argv
ValueError: not enough values to unpack (expected 2, got 1)
```

It must be add `user_name` value.

- 
    - 03 TypeError:
```
PS F:\mystuff> python ex14.py chensir
Hi chensir, I'm the ex14.py script.
I'd like to aks you a few questions.
Do you like me %s
Traceback (most recent call last):
  File "ex14.py", line 8, in <module>
    print("Do you like me %s")% user_name
TypeError: unsupported operand type(s) for %: 'NoneType' and 'str'
```

The right type is `print("Do you like me %s"% user_name)`

### **Fixed and Run again:**

```
PS F:\mystuff> python ex14.py chensir
Hi chensir, I'm the ex14.py script.
I'd like to aks you a few questions.
Do you like me chensir
>yes
Where do you like chensir?
>China
What kind of computer do you have?
>Lenovo

Alright, so you said 'yes' about liking me.
You live in 'China'. Not sure where that is.
And you have a 'Lenovo' computer.Nice.
```

Congratulations!

***

### **Thinking**

- **Must write everyday one by one**

***
- Changelog
- 2017-02-16 00:08:14 ©陈sir
