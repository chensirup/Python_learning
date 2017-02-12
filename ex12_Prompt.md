# Prompt = 提示别人


### **We can use prompt code write `ex11.py` again**

```
age=input("How old are you?")
height=input("How tall are you?")
weight=input("How much do you weigh?")

print("So, you're %r old, %r tall and %r heavy."%(age,height,weight))
```

- **Run code**

```
PS F:\mystuff> python ex12.py
How old are you?30
How tall are you?65
How much do you weigh?264
So, you're '30' old, '65' tall and '264' heavy.
```

***

### **Thinking**

- **How to make String line break a new line?**
    - Try the code `'` and `\n` are not work.

- Try run `python -m pydoc input`,the result is following
```
PS F:\mystuff> python -m pydoc input
Help on built-in function input in module builtins:

input(prompt=None, /)
    Read a string from standard input.  The trailing newline is stripped.

    The prompt string, if given, is printed to standard output without a
    trailing newline before reading input.

    If the user hits EOF (*nix: Ctrl-D, Windows: Ctrl-Z+Return), raise EOFError.
    On *nix systems, readline is used if available.
```
I don't understand it.

***
- Changelog
- 2017-02-12 10:51:53 ©陈sir
