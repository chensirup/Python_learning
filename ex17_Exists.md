# The new command `exists`

### New `import` code `exists`

 - Write `ex17.py`
```
from sys import argv
from os.path import exists

script,from_file,to_file=argv

print("Copying from %s to %s"%(from_file,to_file))

# we could do these two on one line too, how?

input=open(from_file)
indata=input.read()

print("The input file is %d bytes long"%len(indata))

print("Does the output file exist? %r"%exists(to_file))
print("Ready, hit RETURN to continue,CTRL-C to abort.")
input()

output=open(to_file,'w')
output.write(indata)

print("Alright, all done.")

output.close()
input.close()
```

- Runing `python ex17.py test.txt copied.txt`
```
PS F:\mystuff> python ex17.py test.txt copied.txt
Copying from test.txt to copied.txt
The input file is 77 bytes long
Does the output file exist? False
Ready, hit RETURN to continue,CTRL-C to abort.
Traceback (most recent call last):
  File "ex17.py", line 17, in <module>
    input()
TypeError: '_io.TextIOWrapper' object is not callable
```

I has no idea for the **TpyeError**.

**I try deleted `input()` on line 17**, then run again, the amazing result has been:
```
PS F:\mystuff> python ex17.py test.txt copied.txt
Copying from test.txt to copied.txt
The input file is 77 bytes long
Does the output file exist? False
Ready, hit RETURN to continue,CTRL-C to abort.
Alright, all done.
```

There's sth. didn't understand.

***
### Thinking
- What the line 17 `input()` means?

***
- Changelog
- 2017-02-18 23:01:26 ©陈sir