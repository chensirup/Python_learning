# 字符串(string) 和文本

**再次警告自己要特别细心。**

### **几个概念：**

**01 字符串：**

字符串是指你想要展示给别人的、或者是你想要从程序里“导出”的一小段字符。Python里用双引号`""`或单引号`''`来识别。再用print("")打印出来。

如输入`print("我想显示这里的内容")`，运行之后的结果是：

```
我想显示这里的内容
```

**02 变量**

变量是用来指代某个东西的名字。通常是给予`=`的赋值，可以简化，方便记忆。

如：`x=10`或者`w = "This is the left side of..."`

只要输入`print(w)`，即可打印出：
```
This is the left side of...
```
这样是不是很方便了。

**03 格式化字符**

格式化字符的操作符号就是我们常见的百分号`%`。

在Python在有一些特定的格式符。

格式符为真实值预留位置，并控制显示的格式。格式符可以包含有一个类型码，用以控制显示的类型，如下:

>%s    字符串 (采用str()的显示)
> 
%r    字符串 (采用repr()的显示)
> 
%c    单个字符
> 
%b    二进制整数
> 
%d    十进制整数
> 
%i    十进制整数
> 
%o    八进制整数
> 
%x    十六进制整数
> 
%e    指数 (基底写为e)
> 
%E    指数 (基底写为E)
> 
%f    浮点数
> 
%F    浮点数，与上相同
> 
%g    指数(e)或浮点数 (根据显示长度)
> 
%G    指数(E)或浮点数 (根据显示长度)


### 代码练习

输入:
```
x="There are %d types of people."%10
binary="binary"
do_not="don't"
y="Those who know %s and those who %s."%(binary,do_not)

print(x)
print(y)

print("I said:%r."%x)
print("I also said:'%s'."%y)

hilarious="Flase"
joke_evaluation="Isn't that joke so funny?!%r"

print(joke_evaluation%hilarious)

w="This is the left side of..."
e="a string with a right side."

print(w+e)
```

运行后的结果:
```
F:\mystuff> python ex6.py
There are 10 types of people.
Those who know binary and those who don't.
I said:'There are 10 types of people.'.
I also said:'Those who know binary and those who don't.'.
Isn't that joke so funny?!'Flase'
This is the left side of...a string with a right side.
```

未完成:给每一行代码写一个解释说明。