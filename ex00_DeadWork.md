### 安装调适软件

古人云：「**工欲善其事，必先利其器。**」

如何提高效率，而不被电脑剥削，最为关键的就是利用工具。

从人类进化史来看，我们一直在创造工具提高我们的效率，没有刀，很难将肉切碎，而且还要美观。

所以，安装并调适好工具，符合自身的使用习惯非常重要。

看看在开始学习之前都要安装哪些工具，如何设置？

### **1. 安装调适Python**

- **1.1 下载Python**

按照《笨方法学Python》第四版教材，一定建议我们使用2.x版本。

Tips：如果你正在使用Mac，系统是OS X 10.8~10.10，那么系统自带的Python版本是2.7。

Windows系统的同学请移步官网下载安装，请选择2.x，不要像我这样作，安装3.x版本，到时有苦头吃。

下载地址：[Python Download](https://www.python.org/downloads/)，国内网速问题的同学移步：[点击下载](https://pan.baidu.com/s/1boNo6Lp).

**温馨提示：下载时特别考验「人品」，请多一点点耐心。**
  
- **1.2 安装Python**

以Win10，64位系统为例。

在下载完成后，安装Python软件，就像其他软件一样。
**特别注意：**安装时一定要勾选 `Add Python 3.5 to PATH`，然后再安装。

- **1.3 运行Python**

安装完成后，打开命令提示符窗口 （或直接用`cmd`命令），敲入python后，如果得到：
```
C:\mystuff> python
Python 3.5.2 (v3.5.2:4def2a2901a5, Jun 25 2016, 22:18:55) [MSC v.1900 6
Type "help", "copyright", "credits" or "license" for more information.
>>>
```
说明安装成功，并进入了Python的交互模式，尝试在`>>>`后面输入`100+200`，敲下`Enter`，看看会出现什么神奇的答案。

###2. 安装调适gedit

gedit 是文本编辑器，支持很多系统和语言。还有一款神器：Notepad++，应用也很广。（不过，为了后面学习不出幺鹅子，还是先老老实实用gedit。）

- **2.1 下载gedit**

直接到官网即可下载：[点击下载](https://gedit.en.softonic.com/)

选择适用的符合电脑系统的版本，直接下载并安装。

-  **2.2 设置gedit**

由于Python编程语法特殊，需要重新设置一下gedit 编辑器。

Tips：把  gedit 放到桌面或者快速启动栏，这样你就可以方便地访问到该程序了。

安装完成后，运行 gedit，我们要先改掉一些愚蠢的默认设定。

>a.从`编辑`中打开`首选项`  ，选择`编辑器`页面。
> b.将`跳格宽度`：改为4。
> c.勾选并启用`自动缩进`。
> d.点击`查看`页面，勾选并启用`显示行号`。

OK，大功告成，以后就可以用gedit 编写代码啦。

### 3. 使用运行Python
运行Python，一般不在`cmd`命令符里，而用「**PowerShell**」程序来运行。

从开始菜单运行「PowerShell」程序。你可以使用开始菜单的搜索功能，输入名称后敲回车即可打开。（为了方便后续使用，请为它创建一个快捷方式，放到桌面或者快速启动栏。）

打开后，输入`Python`，回车，如果同样看到：

```
C:\mystuff> python
Python 3.5.2 (v3.5.2:4def2a2901a5, Jun 25 2016, 22:18:55) [MSC v.1900 6
Type "help", "copyright", "credits" or "license" for more information.
>>>
```
恭喜你，可以正常使用Python，开始编程啦。

再次在`>>>`后面输入`100+200`，敲下`Enter`，看看又会出现什么神奇的答案。
