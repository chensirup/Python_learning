# Write new code import script

### **ex13 include `argument`、`variable`、`unpack`.**

- **we write a new script include `argv` is following**

```
from sys import argv

script,first,second,third=argv

print("The script is called:"),script
print("Your first variable is:"),first
print("Your second variable is:"),second
print("Your third variable is:"),third

```

- **Run**

```
PS F:\mystuff> python ex13.py first 2nd 3rd
The script is called:
Your first variable is:
Your second variable is:
Your third variable is:
```
There's sth wrong, checkouted and fined the trouble.

The`)` code must put the last, fixed as follow:

```
from sys import argv

script,first,second,third=argv

print("The script is called:",script)
print("Your first variable is:",first)
print("Your second variable is:",second)
print("Your third variable is:",third)

```

- **Run again**

```
PS F:\mystuff> python ex13.py first 2nd 3rd
The script is called: ex13.py
Your first variable is: first
Your second variable is: 2nd
Your third variable is: 3rd
```
Congratulations!

***

### **Thinking**

- **If we change the `argv`, it'll print what result?**

    - We run the new code as `python ex13.py cheese apples bread`
    - We saw the result as following

```
PS F:\mystuff> python ex13.py cheese apples bread
The script is called: ex13.py
Your first variable is: cheese
Your second variable is: apples
Your third variable is: bread
```
  - If we write more or less `argv` it'll some error like:
       - less `argv`
```
PS F:\mystuff> python  ex13.py chensir
Traceback (most recent call last):
  File "ex13.py", line 5, in <module>
    script,first,second,third=argv
ValueError: not enough values to unpack (expected 4, got 2)
```

The error prompt us the unpack included 4 values at least, it has 2 values.

- 
   - more `argv`
```
PS F:\mystuff> python ex13.py chensir is kind man
Traceback (most recent call last):
  File "ex13.py", line 5, in <module>
    script,first,second,third=argv
ValueError: too many values to unpack (expected 4)

```

The error prompt us the unpack included 4 values at most.

- **If we use `input` and `argv` together in one script, what's result will be?**

***
- Changelog
- 2017-02-14 13:22:46 ©陈sir

