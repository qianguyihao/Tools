



## 方法一：使用Calibre去除kindle/Google play书籍的DRM导入多看（推荐）


参考链接：[使用Calibre去除kindle/Google play书籍的DRM导入多看](http://www.jianshu.com/p/63f70e660ad5)





## 方法二：使用DeDRM破解kindle图书（此法已经失效）


### 什么是DRM保护


DRM，全称 Digital Rights Management（数字版权管理），是随着电子音频视频节目在互联网上的广泛传播而发展起来的一种新技术。出版者利用这些技术保护有数字化内容（例如：软件、音乐、电影），防止数字出版物被非法复制，或者在一定程度上使复制很困难，使得最终用户必须得到授权后才能使用数字媒体。解释听起来很官方，其实在这里我们只需要知道DRM是为了保护电子书版权而使用的一种限制技术就可以了。



### 为什么要破解 DRM保护


为了保护电子书的版权，亚马逊提供的 azw 或 azw3 格式电子书都是经过 DRM 加密了的，即便是获取到了 azw 或 azw3 格式的电子书文件，也无法直接在其他阅读器或阅读设备上阅读。



### 破解 DRM 保护的准备工作

在开始破解 DRM 保护之前，我们需要准备好以下内容：

- 1、DRM 移除软件

- 2、带 DRM 保护的电子书

- 3、你的亚马逊账号绑定的 Kindle 设备的序列号

下面分别详细介绍。

**1、DRM 移除软件：DeDRM tools**

DeDRM tools (v6.3.3) 下载：[官方下载](https://github.com/apprenticeharper/DeDRM_tools)、 [百度网盘](https://pan.baidu.com/s/1bnExMYN)

注意：在 Windows 系统中运行 `DeDRM_Drop_Target.bat` 时如果出现“找不到 Python”之类的提示，请务必确保您的系统安装了 Python 和 PyCrypto 这两款软件：

- Python 下载：官方下载 | 百度网盘
- PyCrypto 下载：官方下载 | 百度网盘


**2、准备好需要移除 DRM 保护的电子书到本地**

把需要破解的 azw 或 azw3 格式的电子书获取到本地，获取方式有以下几种：

- 方式一：从亚马逊云端下载（推荐）

进入亚马逊后台的 我的内容（用绑定 Kindle 的亚马逊账号登录），找到想要破解的那本书，点击电子书旁边的【…】按钮，在弹出的菜单中点击“通过电脑下载USB传输”，选择你的 Kindle 设备，点击【下载】按钮把电子书下载到电脑中，然后再按照本文的方法进行破解即可。

- 方式二：从 Kindle 阅读软件的目录中拷贝

需要安装 Kindle 桌面客户端软件。如果没有安装请先在下面的列表中选择合适您的系统版本安装。安装完成后打开软件，用亚马逊账号登录，然后下载想要破解的电子书，再从相应电子书存放路径中找到它们（文件名类似于“B0080BKP1K_EBOK.azw”这种），请将它们拷贝到如桌面等任意位置备用。

Kindle for Windows 版：官方去下载。电子书存放路径：C:\Users\你的用户名\Documents\My Kindle Content

Kindle for Mac 版：官方去下载。电子书存放路径：/Users/你的用户名/Library/Application Support/Kindle/My Kindle Content

- 方式三：直接从 Kindle 阅读器中拷贝。

用USB线将 Kindle 连接到电脑，打开 Kindle 驱动器，在根目录里的 Documents 文件夹内找到 azw 或 azw3 格式的电子书文件将其拷贝出来。这种方法现在不建议使用，因为最新版本固件已经将下载到 Kindle 中的电子书中的图片抽离出去，导致直接复制的电子书缺失图片。



**3、记下 Kindle 设备的序列号**

Kindle 的序列号可以在包装盒或保修单上找到，没有包装盒或保修单的话也可以在系统里找到，因为 Kindle 系列阅读器的序列号位置不一样，下面列出了各个版本查看序列号的步骤：

- kindle paperwrite 1 / 2

中文版：首页 — 菜单（右上角的三道杠） — 设置 — 菜单（右上角三道杠） — 设备信息。

英文版：Home — Menu — Settings — Menu — Device Info

- kindle 4 / kindle touch

home — menu — setting — 第二页的Device Info里的“Serial Number:”

- Kindle 1 / 2 / 3 / Keyboard / DX / DXG
home — menu — settings — 屏幕右下角会显示序列号（未证实）



## 移除 Kindle 电子书 DRM 保护详细步骤

做完以上准备工作就可以开始破解操作了。下面的操作步骤分为 Mac OS X 系统和 Windows 系统，选择适合自己系统的方法。

### Mac OS X 系统操作步骤

打开刚才解压的 `DeDRM_tools-master`文件夹，进入 `DeDRM_Macintosh_Application` 目录，双击打开 `DeDRM`，界面如下图所示， 点击界面右下角「Configure…」

在弹出的窗口中选中第一项「eInk Kindle ebooks」，然后点击「Configure…」（也可以双击「eInk Kindle ebooks」这一项）。

在弹出的窗口中输入你的 Kindle 序列号，点击「Add」按钮，然后点击「close」，然后点击「finish」。

返回主界面后，点击界面下方的「Select Ebook」，选择刚才拷贝的那个 azw 或 azw3 文件，点击确定即可完成破解。

### Windows 系统操作步骤

打开刚才解压的 `DeDRM_tools-master`文件夹，进入 `DeDRM_Windows_Application\DeDRM_App`目录，双击打开 `DeDRM_Drop_Target.bat`，出现如下界面：

在「eInk Kindle Serial Number list」一栏中填写你的 Kindle 序列号，然后点击下方的「Set Prefs」按钮保存。接下来，点击界面下面的「Select an eBook to Process」一栏后面的「…」按钮，选择电子书，点击「Process eBook」即可完成破解。




参考链接：[用 DeDRM 破解去除 AZW 格式电子书 DRM 保护 （Kindle 图书破解）](http://www.jianshu.com/p/d838f593c8ca)







