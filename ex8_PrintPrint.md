# Print Print

**只管编写，然后打印：**

```
# ex8 print print

formatter="%r %r %r %r"

print(formatter%(1,2,3,4))
print(formatter%("one","two","three","four"))
print(formatter%(True,False,False,True))
print(formattre%(formatter,formatter,formatter,formatter))
print(fomatter%(
"I had this thing.",
"That you could type up right.",
"But it didn't sing.",
"So I said goodnight."))

```

运行结果**报错**啦：
```
PS F:\mystuff> python ex8.py
1 2 3 4
'one' 'two' 'three' 'four'
True False False True
Traceback (most recent call last)：
  File "ex8.py", line 8, in <module>
    print(formattre%(formatter,formatter,formatter,formatter))
NameError： name 'formattre' is not defined
```
提示 第8行 有一个名称错误`formattre`，仔细一看，应该是`formatter`。

**再次警告自己，不能再犯这种拼写低级错误。**

- **PS：如果代码程序中有一行出错，后面的代码行结果也不会出现，卡在那里。**

第一次修正后的结果：
```
PS F:\mystuff> python ex8.py
1 2 3 4
'one' 'two' 'three' 'four'
True False False True
'%r %r %r %r' '%r %r %r %r' '%r %r %r %r' '%r %r %r %r'
Traceback (most recent call last)：
  File "ex8.py", line 9, in <module>
    print(fomatter%("I had this thing.","That you could type up right.","But it didn't sing.","So I said goodnight."))
NameError： name 'fomatter' is not defined

```
呃，快被自己蠢哭了，又是一个拼写的低级错误。

**严重警告：**如果以后遇到一次报错，就应该从头开始检查一遍，尽量一次修正错误。

第二次检查并修正后的结果：
```
PS F:\mystuff> python ex8.py
1 2 3 4
'one' 'two' 'three' 'four'
True False False True
'%r %r %r %r' '%r %r %r %r' '%r %r %r %r' '%r %r %r %r'
'I had this thing.' 'That you could type up right.' "But it didn't sing." 'So I said goodnight.'
```
恭喜，运行成功。
***
- **思考题**
    - **问题：**最后一行代码有单引号`'`，又有双引号`""`，他们是如何工作的？
    - **猜想：**如果字符串中有单引号，字符串会转成双引号。
    - **留白：**可是单引号是怎么工作的呢？？

***
- Changelog
- 2017-02-08 09:47:47 ©陈sir
