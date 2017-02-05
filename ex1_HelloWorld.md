# This is the first ex.
**注意Python3版本以上'print'后面要加英文状态下的括号'()'.**

第一个练习步骤：
- **01 输入**

打开**gedit**编辑器，编写你人生的第一个代码程序吧。
```
print ("Hello World!")
print ("Hello Again")
print ("I like typing this.")
print ("This is fun.")
print ('Yay! Printing.')
print ("I'd much rather you 'not'.")
print ('I "said" do not touch this.')
print (' ')
```
- **02 保存**

请将编写好的「代码程序」保存到一个指定的文件夹，并另存为ex1.py。一定是`.py`后缀，才能被Python识别并运行。

- **03 运行**

马上运行人生第一个代码了，想想还是有点小激动。

接下来是见证奇迹的时刻。

打开运行「**PowerShell**」命令行终端，CD到存放`.py`文件的文件夹。

**输入下面的命令代码：**
```
python ex1.py
```
敲下回车，看看会看到什么结果？

#### 如果代码没写错，就能看到：

```
PS F:\mystuff> python ex1.py
Hello World!
Hello Again
I like typing this.
This is fun.
Yay! Printing.
I'd much rather you 'not'.
I "said" do not touch this.
```

### 容易出错的点

严正声明：**一切错误都是你的错，计算机永远不会错。**

所以，出错了，请认真回去检查代码编写是否有误。

- **语法错误**

比如，出现下面报错代码：

```
PS F:\mystuff> python ex1.py
  File "ex1.py", line 6
    print ("I like typing this.)
                               ^
SyntaxError: EOL while scanning string literal
```
我们要学会看懂：

>a.我们运行了`ex1.py`脚本程序；
> b.Python告诉我们`exq1.py`文件中第6行代码有错误；
> c.Python把错误的地方标记出来打上了`^`符号，仔细检查发现，少了一个`"`符号。（不管是单引号还是又引号，包括所有符号，都要使用英文状态下的。）
d.Python打印出一个`SyntaxError`告诉我们是代码错误。

- **编码错误**

如果你来自另外一个国家，而且你看到关于 ASCII 编码的错误，那就在你的Python 脚本文件的**最上面**加入这一行：

`# -- coding: utf-8 --`

这样你就在脚本中使用了 unicode UTF-8 编码，这些错误就不会出现了。
***
OK，人生的第一个代码已经成功实现了，继续加油吧。
