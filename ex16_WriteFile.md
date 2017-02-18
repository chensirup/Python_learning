# Write File

If I dit ex15's bonus exercise, I must kown command following:

- close - colse files. It means `file`-`save`
- read - read some files.
- readline - read some lines in txt.
- truncate - clear files, becareful.
- write(stuff) - write stuff in some files.

### We exercise `write` command .

- write new code in `ex16.py`
```
from sys import argv

script,filename=argv

print("We're going to erase %r."%filename)
print("If you don't want that, hit CTRL-C(^C).")
print("If you do want that, hit RETURN.")

input("?")

print("Opening the file...")
target=open(filename,'w')

print("Truncating the file. Goodbye!")
target.truncate()

print("Now I'm going to ask you for three lines.")

line1=input("line 1:")
line2=input("line 2:")
line3=input("line 3:")

print("I'm going to write these to the file.")

target.write(line1)
target.write("\n")
target.write(line2)
target.write("\n")
target.write(line3)
target.write("\n")

print("And finally, we close it.")
target.close()
```

- Runing `python ex16.py test.txt`
```
PS F:\mystuff> python ex16.py test.txt
We're going to erase 'test.txt'.
If you don't want that, hit CTRL-C(^C).
If you do want that, hit RETURN.
?
Opening the file...
Truncating the file. Goodbye!
Now I'm going to ask you for three lines.
line 1:To all people out there.
line 2:I say I don't like my hair.
line 3:I need to shave it off.
I'm going to write these to the file.
And finally, we close it.
```
***

### Thinking

- wirte the `read` command by `ex16_1.py` or `ex16_2.py`
    - `ex16_1.py`
```
from sys import argv

script,filename=argv

txt=open(filename)

print("I want to read %r."%filename)
print(txt.read())
```

    - `ex16_2.py`
```
from sys import argv

script,filename=argv

file =input(">")

print("Type the %r again."%filename)

txt=open(filename)

print(txt.read())
```

- Runing `ex16_1.py test.txt` and `ex16_2.py test.txt`
    - `ex16_1.py test.txt`
```
PS F:\mystuff> python ex16_1.py test.txt
I want to read 'test.txt'.
To all people out there.
I say I don't like my hair.
I need to shave it off.
```

    - `ex16_2.py test.txt`
```
PS F:\mystuff> python ex16_2.py test.txt
>test.txt
Type the 'test.txt' again.
To all people out there.
I say I don't like my hair.
I need to shave it off.
```

- line 25-30 can write one line together like following

`target.write(line 1+'\n' + line 2+'\n' +line 3 +'n\')`

***
- Changelog
- 2017-02-18 22:23:38 ©陈sir
