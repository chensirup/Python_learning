# Function and Files

### Write and Run `ex20.py`

- Writed

```
from sys import argv

script,input_file=argv

def print_all(f):
    print(f.read())

def rewind(f):
    f.seek(0)

def print_a_line(line_count,f):
    print(line_count,f.readline())

current_file=open(input_file)

print("First let's print the whole file:\n")

print_all(current_file)

print("Now let's rewind,kind of like a tape.")

rewind(current_file)

print("Let's print three lines:")

current_line=1
print_a_line(current_line,current_file)

current_line=current_line+1
print_a_line(current_line,current_file)

current_line=current_line+1
print_a_line(current_line,current_file)
```

- Runned

```
PS F:\mystuff> python ex20.py test.txt
First let's print the whole file:

To all people out there.
I say I don't like my hair.
I need to shave it off.

Now let's rewind,kind of like a tape.
Let's print three lines:
1 To all people out there.

2 I say I don't like my hair.

3 I need to shave it off.
```

- The wrong

That's sth wrong following

- SyntaxError

```
PS F:\mystuff> python ex20.py
  File "ex20.py", line 6
    print f.read()
          ^
SyntaxError: invalid syntax
```

- less agrv

```
PS F:\mystuff> python ex20.py
Traceback (most recent call last):
  File "ex20.py", line 3, in <module>
    script,input_file=argv
ValueError: not enough values to unpack (expected 2, got 1)
```

### Thinking

- Try use `+=`
    - First test

```
print("Let's print three lines:")

current_line=1
print_a_line(current_line,current_line+1,current_line+2,current_file)
```

- 
    - TypeError

```
PS F:\mystuff> python ex20_1.py test.txt
First let's print the whole file:

To all people out there.
I say I don't like my hair.
I need to shave it off.

Now let's rewind,kind of like a tape.
Let's print three lines:
Traceback (most recent call last):
  File "ex20_1.py", line 27, in <module>
    print_a_line(current_line,current_line+1,current_line+2,current_file)
TypeError: print_a_line() takes 2 positional arguments but 4 were given
```

That isn't work.

***
- Changelog
- 2017-02-25 12:25:17 ©陈sir