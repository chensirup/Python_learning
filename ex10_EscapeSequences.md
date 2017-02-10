# What're they.

### **What're escape sequences.**

- back-slash `n` means new line, **`\n`.**

Other escape sequences:
- double back-slash** `\\`**
- single quotes back-slash** `\'`**
- double quotes back-slash **`\"`**
- triple-quotes back-slash**`"""`**
***

-  **Write some code include some escape.**

```
print("I am 6'2\" tall.") # escape double quotes in string
print('I am 6\'2" tall.') # escape single quotes in string
```
- Run code
```
I am 6'2" tall.
I am 6'2" tall.
```
That's amazing!

***
### **escape triple-quotes in string, you can add any line as you like.**

- **Write some code include more escape.**

```
# What're they.
# back-slash `n` means new line, `\n`.
# Other escape sequences, double back-slash `\\`; single quotes back-slash `\'`;  double quotes back-slash `\"`; triple-quotes back-slash`"""`.

#Write some code include some escape.

print("I am 6'2\" tall.") # escape double quotes in string
print('I am 6\'2" tall.') # escape single quotes in string

tabby_cat="\tI'm tabbed in."
persian_cat="I'm split\non a line."
backslash_cat="I'm \\a \\ cat."

fat_cat="""
I'll do a list:
\t* Cat food
\t* Fishies
\t* Catnip\n\t* Grass
"""
print(tabby_cat}
print(persian_cat)
print(backslash_cat）
print(fat_cat)

```

- **Run it**
```
PS F:\mystuff> python ex10.py
  File "ex10.py", line 25
    print(tabby_cat}
                   ^
SyntaxError: invalid syntax
```
Oh, my god.

It's a stupid wrong.

Fix `}`=`)`

Run again.
```
PS F:\mystuff> python ex10.py
  File "ex10.py", line 27
    print(backslash_cat）
                       ^
SyntaxError: invalid character in identifier
```
It's stupid wrong again.

**It must write`)` by English character.**

Fix and run again.
```
PS F:\mystuff> python ex10.py
I am 6'2" tall.
I am 6'2" tall.
        I'm tabbed in.
I'm split
on a line.
I'm \a \ cat.

I'll do a list:
        * Cat food
        * Fishies
        * Catnip
        * Grass
```
**Congratulasions ! **

I did it.
***
### **Thinking**

- **`\t`=Tab**
- I try to take `'''` replace `"""`, the result is the same.
