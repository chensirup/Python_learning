# More Print

### **练习7**

这是一节巩固练习，复习及综合应用前面的练习。

所以，简单直接输入：
```
print("Mary had a little lamb.")
print("Its fleece was white as %s."%'snow')
print("And everywhere that Mary went.")
print("."*10)# what'd that do?

end1="C"
end2="h"
end3="e"
end4="e"
end5="s"
end6="e"
end7="B"
end8="u"
end9="r"
end10="g"
end11="e"
end12="r"

# watch that comma at the end. try removing it to see what happens
print(end1+end2+end3+end4+end5+end6),
print(end7+end8+end9+end10+end11+end12)

```

运行得到的结果：
```
PS F：\mystuff> python ex7.py
Mary had a little lamb.
Its fleece was white as snow.
And everywhere that Mary went.
..........
Cheese
Burger
```

**最后的结果与教程有出入：**

最后两行代码，原教程的结果是 `Cheese Burger`，而我运行出来的却是断行的：
```
Cheese
Burger
```
**自我判断**：

应该是`,`带来的差异，按教程的意思comma打印的结果应该是`空格`。而自己运行的结果却是`断行`。

- 尝试改变代码1未果:
```
print(end1+end2+end3+end4+end5+end6),print(end7+end8+end9+end10+end11+end12)
```
结果还是断行：
```
Cheese
Burger
```
- 尝试改变代码2未果:
```
print(end1+end2+end3+end4+end5+end6),(end7+end8+end9+end10+end11+end12)
```
结果只显示前一段代码的结果：
```
Cheese
```

- 尝试改变代码3，成功:
```
print(end1+end2+end3+end4+end5+end6,end7+end8+end9+end10+end11+end12)
```
最终的结果是，奖励一朵小红花：
```
Cheese Burger
```
***
### **检查错误**

- **代码编写错误**
在第一次输入的时候，最后两行代码加了`""`：
```
print("end1+end2+end3+end4+end5+end6"),
print("end7+end8+end9+end10+end11+end12")
```

运行的结果变成了：

```
end1+end2+end3+end4+end5+end6
end7+end8+end9+end10+end11+end12
```

错误点在于：代码加入了`""`后，即变成了**字符串**，将作为显示的内容直接打印出来，而不是运算了。

- **倒序检查错误**

恕我无能，好像不知道错误在哪里。
***
- Changelog
- 2017-02-07 09:46:46 ©陈sir