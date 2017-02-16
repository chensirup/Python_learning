# Read File

### **The new code:`open`**

- **01 Write a file `ex15_sample`:**
```
This is stuff I typed into a file.
It is really cool stuff.
Lots and lots of fun to have in here.
```

- **02 Write `ex15.py`:**
```
from sys import argv

script,filename=argv

txt=open(filename)

print("Here's your file %r:"%filename)
print(txt.read())

print("Type the filename again:")
file_again=input(">")

txt_again=open(file_again)

print(txt_again.read())

```

- **03 The last result:**

```
PS F:\mystuff> python ex15.py ex15_sample.txt
Here's your file 'ex15_sample.txt':
This is stuff I typed into a file.
It is really cool stuff.
Lots and lots of fun to have in here.
Type the filename again:
>ex15_sample.txt
This is stuff I typed into a file.
It is really cool stuff.
Lots and lots of fun to have in here.
```

***

### **Some wrong by running**
- **01 SyntaxError:**
```
PS F:\mystuff> python ex15.py ex15_sample.txt
  File "ex15.py", line 15
SyntaxError: Non-UTF-8 code starting with '\xa3' in file ex15.py on line 15, but no encoding declared; see http://python
.org/dev/peps/pep-0263/ for details
```

The `ex15.py` writed by **Notepad++**, must add `# -- coding: utf-8 --` on the first line.

- **02 SyntaxError:**
```
PS F:\mystuff> python ex15.py ex15_sample.txt
  File "ex15.py", line 16
    print\ufffd\ufffdtxt_again.read())
                   ^
SyntaxError: invalid character in identifier
```

It's the wrong code `（` by Chinese-characterizing，the right code is English-characterizing by `(`.

- **03 FileNotFoundError:**
```
PS F:\mystuff> python ex15.py ex15_samlpe.txt
Traceback (most recent call last):
  File "ex15.py", line 6, in <module>
    txt=open(filename)
FileNotFoundError: [Errno 2] No such file or directory: 'ex15_samlpe.txt'
```

The filename is `ex15_sample.txt` not** `ex15_samlpe.txt`.**

***

### **Thinking**

Must be careful.

***
- Changelog
- 2017-02-16 08:11:24 ©陈sir
