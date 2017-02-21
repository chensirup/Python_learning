# Function - `def`

### What's Function

What the `Function` can do:

- Function can name the ** code snippet**,  just like `Variable` can name `string` and `data`.

- Function can accept parameter, just like `script` can accept `argv`.

- We can use `#1` or `#2` build **Mico Script** or **Mico command**.

The first function - `def`.

Write new ex18.py :

```
# this one is like your scripts with argv
def print_two(*args):
    arg1,arg2=args
    print("arg1:%r,arg2:%r"%(arg1,arg2))

#ok,that *args is actually pointless, we can just do this
def print_two_again(arg1,arg2):
    print("arg1:%r,arg2:%r"%(arg1,arg2))

# this just takes one argument
def print_one(arg1):
    print("arg1:%r"%arg1)

# this one takes no arguments
def print_none():
    print("I got nothin'.")


print_two("Zed","Shaw")
print_two_again("chen","sir")
print_one("First!")
print_none()
```

Runed it :

```
PS F:\mystuff> python ex18.py
arg1:'Zed',arg2:'Shaw'
arg1:'chen',arg2:'sir'
arg1:'First!'
I got nothin'.
```
***
### Thinking

- One function factor :
    - example `def` function, `def`=`define`
    - give a name behine function, like `print_two`
    - take argument like `*args`
    - take **variable** in `( )`
    - use `:` in the end
    - take one `Tab` = 4 indent, for the new line
    - `print` the unpack

- `run`, `call`, `use` function are the same.

***
- Changelog
- 2017-02-21 17:22:24 ©陈sir