---
title: Sublime Text快捷键
date: 2016-05-18 12:39:04
categories:
- 技术
tags:
- 工具
---






### 选择

- `Ctrl + D`：选择当前光标所在的词并高亮该词所有出现的位置，再次按`Ctrl + D`选择该词出现的下一个位置。

在多重选词的过程中，使用`Ctrl + K`进行跳过，使用`Ctrl + U`进行回退，使用`Esc`退出多重编辑

- **`Alt + F3`**： 选中文本按下快捷键，即可一次性选择全部的相同文本进行同时编辑。

例如：快速选中并更改所有相同的变量名、函数名等。

- `Ctrl + ←/→`：进行逐词移动

- `Ctrl + ↑/↓`：移动当前显示区域

- `Shift + ↑/↓`：一行一行地进行选中。

- `Ctrl + Shift + ←/→`：进行逐词选择

- **`Ctrl + Shift + ↑/↓`：移动当前行**

- **`Ctrl+Shift+L`：先选中多行，再按下快捷键，会在每行行尾插入光标，即可同时编辑这些行。**

- **`Ctrl + J`：把当前选中区域合并为一行**。

- `Ctrl+L`：选中整行，继续操作则继续选择下一行，效果和 `Shift + ↓` 效果一样。

- `Ctrl + M`：光标移动至括号内结束或开始的位置

- `Ctrl + Shift + M`：快速选择括号间的内容

- `Ctrl + Shift + J`：快速选择同缩进的内容

- `Ctrl + Shift + Space`：快速选择当前作用域（Scope）的内容

- `Ctrl+Shift+[`：选中代码，按下快捷键，折叠代码。

- `Ctrl+Shift+]`：选中代码，按下快捷键，展开代码。

- `Ctrl+K+0`：展开所有折叠代码。

### 多重选择（Multi-Selection）

多重选择功能允许在页面中同时存在多个光标，让很多本来需要正则表达式、高级搜索和替换才能完成的任务也变得游刃有余。

激活多重选择的方法有两几种：

- 按住 Ctrl 然后在页面中希望中现光标的位置点击。
- 选择数行文本，然后按下 Shift + Ctrl + L。
通过反复按下 Ctrl + D 即可将全文中与光标当前所在位置的词相同的词逐一加入选择，而直接按下 Alt+F3即可一次性选择所有相同的词。
- 按下鼠标中键来进行垂直方向的纵列选择，也可以进入多重编辑状态。






### 搜索

- `Ctrl + Shift + F`：多文件查找&替换

在文件夹内查找，与普通编辑器不同的地方是sublime允许添加多个文件夹进行查找。



- `F3`：跳至当前关键字下一个位置

- `Shift + F3`：跳到当前关键字上一个位置


- `Ctrl + F/H`：进行标准查找/替换，之后：

 - `Alt + C`：切换大小写敏感（Case-sensitive）模式

 - `Alt + W`：切换整字匹配（Whole matching）模式

 - `Alt + R`：切换正则匹配（Regex matching）模式

 - `Ctrl + Shift + H`：替换当前关键字

 - `Ctrl + Alt + Enter`：替换所有关键字匹配



- `Ctrl + P：打开搜索框，跳转到指定文件。输入文件名后可以：

 - 输入当前项目中的文件名，快速搜索文件；

 - 输入@和关键字，查找文件中函数名；

 - 输入：和数字，跳转到文件中该行代码；

 - 输入#和关键字，查找变量名

- `Ctrl + R`：打开搜索框，自带`@`，输入关键字，查找文件中的函数名。

例如：在函数较多的页面快速查找某个函数。

- `Ctrl + G`：打开搜索框，自动带`:`，输入数字跳转到该行代码。

例如：在页面代码比较长的文件中快速定位。

- `Ctrl+ `：打开搜索框，自动带`@`，输入关键字，查找文件中的函数名。

例如：在函数较多的页面快速查找某个函数。


### 显示

- `Ctrl+Tab`：按文件浏览过的顺序，切换当前窗口的标签页。

- `Ctrl+PageDown`：向左切换当前窗口的标签页。

- `Ctrl+PageUp`：向右切换当前窗口的标签页。

- `F11`：普通全屏

- **`Shift + F11`：免打扰全屏**

- `Alt + Shift + 1`：窗口分屏，恢复默认1屏（非小键盘的数字）

- `Alt + Shift + 2`：左右分屏-2列

- `Alt + Shift + 3`：左右分屏-3列

- `Alt + Shift + 4`：左右分屏-4列

- `Alt + Shift + 5`：上下左右分屏-等分4屏

- `Alt + Shift + 8`：上下分屏-2行

- `Alt + Shift + 9`：上下分屏-3行

- `Ctrl+K+B`：开启/关闭侧边栏。

备注：分屏之后，使用`Ctrl + 数字键`跳转到指定屏，使用`Ctrl + Shift + 数字键`将当前屏移动到指定屏



### 窗口

`Ctrl + N`：在当前窗口创建一个新标签

`Ctrl + Shift + N`：创建一个新窗口

`Ctrl + Shift + T`：恢复刚刚关闭的标签

### 其他

- `Ctrl + Shift + P`：调出命令板（Command Palette）

- `Ctrl + `：调出控制台


## 参考链接


- [我的Sublime Text 3 配置](http://lovenight.github.io/2015/11/30/%E6%88%91%E7%9A%84Sublime-Text-3-%E9%85%8D%E7%BD%AE/)

- [知乎：Sublime Text 有哪些实用技巧？](https://www.zhihu.com/question/19976788)

- [如何优雅地使用Sublime Text3](http://www.jeffjade.com/2015/12/15/2015-04-17-toss-sublime-text/)

- [面向 Web 开发者的 Sublime Text 插件](http://chinagdg.org/2016/02/ttt1-sublime-plugins/)

- [Sublime Text 3最好的功能、插件和设置](http://www.css88.com/archives/5858)

- [Sublime Text：我的极简 Markdown 编辑器](http://tinyletter.com/CnFeat/letters/sublime-text-markdown)

- [如何优雅地使用 Sublime Text3 [OS X]](http://qiudeqing.com/tools/2015/05/31/sublime-text-3.html)

- [Seti UI 主题: 让你编辑器焕然一新](http://chinagdg.org/2016/02/ttt2-seti-ui/)

- [Sublime Text 3 配置和使用方法](https://www.zybuluo.com/king/note/47271)


- [20 个强大的 Sublime Text 插件](http://www.oschina.net/translate/20-powerful-sublimetext-plugins)

- [像 Sublime Text 一样使用 Chrome DevTools](http://chinagdg.org/2015/12/%E5%83%8F-sublime-text-%E4%B8%80%E6%A0%B7%E4%BD%BF%E7%94%A8-chrome-devtools/)

网站的这篇文章也可以看看：[http://chinagdg.org/2016/04/android-studio-2-0/](http://chinagdg.org/2016/04/android-studio-2-0/)


- [sublime text插件推荐](http://w3cboy.com/post/2014/01/sublime%E6%8F%92%E4%BB%B6%E6%8E%A8%E8%8D%90/)
