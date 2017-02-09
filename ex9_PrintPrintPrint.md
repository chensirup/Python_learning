# Print Print Print

**This exercise has a new formatter.**

- **Step1 : Write code by ex9**

```
# Here's some new strange stuff, remember type it exactly.

days=" Mon Tue Wed Thu Fri Sat Sun"
months="Jan\nFeb\nMar\nApr\nMay\nJun\nJul\nAug"

print("Here are the days:",days)
print("Here are the months:",months)

print"""
There's something going on here.
with the three double-quotes.
We'll be able to type as much as we like.
Even 4 lines if we want, or 5,or 6.
"""

```

- **Step2 : Run `ex9.py` code**
```
PS F:\mystuff> python ex9.py
  File "ex9.py", line 14
    """
      ^
SyntaxError: Missing parentheses in call to 'print'
```

Oh, my God! It's something wrong.

**I find it. **

The** `print`** code must add** `()`**, it's python 3.5.2 version on my computer.

- **Step3 : Fix code as below**
```
# Here's some new strange stuff, remember type it exactly.

days=" Mon Tue Wed Thu Fri Sat Sun"
months="Jan\nFeb\nMar\nApr\nMay\nJun\nJul\nAug"

print("Here are the days:",days)
print("Here are the months:",months)

print("""
There's something going on here.
with the three double-quotes.
We'll be able to type as much as we like.
Even 4 lines if we want, or 5,or 6.
""")

```

- **Step4 : Run again**
```
PS F:\mystuff> python ex9.py
Here are the days:  Mon Tue Wed Thu Fri Sat Sun
Here are the months: Jan
Feb
Mar
Apr
May
Jun
Jul
Aug

There's something going on here.
with the three double-quotes.
We'll be able to type as much as we like.
Even 4 lines if we want, or 5,or 6.

```
**Congratulations!**

You did it.
***
### Thinking

- I must remember I installed python 3.5.2 version no my computer.
- It must **add `()` behind `print` code**.
***
- Changlog
- 2017-02-09 10:42:49 ©陈sir

