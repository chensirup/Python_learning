语法报错
```
PS F:\mystuff> python ex5.py
  File "ex5.py", line 17
    print("His teeth are usually %s depending on the coffee."%my_teeth)
        ^
 SyntaxError: invalid syntax
```
解析报错
```
PS F:\mystuff> python ex5.py
  File "ex5.py", line 20

    ^
SyntaxError: unexpected EOF while parsing
```
大小写错误
```
PS F:\mystuff> python ex5_1.py
Let's talk about chensir.
He's 65 inches tall.
He's 264 pounds heavy.
Actually that's not too heavy.
He's got Brown eyes and Black hair.
His teeth are usually White depending on the coffe.
Traceback (most recent call last):
  File "ex5_1.py", line 17, in <module>
    Print("If I add %d,%d,and %d I get %d."%(age,height,weight,age+height,weght))
NameError: name 'Print' is not defined
```

