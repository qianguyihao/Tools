



## Git的安装及创建版本库

### 在Windows平台安装Git

msysgit是Windows版的Git，下载链接：<https://git-for-windows.github.io/>。下载完成后，按照默认的配置，一路next，即可安装完成。


### 在Linux平台安装Git

首先，可以试着输入git，看看系统有没有安装Git：

```bash
$ git

The program 'git' is currently not installed. You can install it by typing:

sudo apt-get install git
```

如果用Debian或Ubuntu Linux，通过一条命令即可完成安装：

```bash
sudo apt-get install git
```

如果是其他Linux版本，可以直接通过源码安装。先从Git官网下载源码，然后解压，依次输入如下命令即可：

```bash
./config
make
sudo make install
```



## 配置用户信息



```bash
# 设置提交代码时的用户信息
$ git config --global user.name "Your Name"
$ git config --global user.email "email@example.com"

# 显示当前的Git配置
$ git config --list
```

如果用的是TortoiseGit，也可以在`Settings-->Git-->User Info`下，直接填写name和Email。


Git的配置文件为.gitconfig，它可以在用户主目录下（全局配置：`C:\Users\name\.gitconfig`），也可以在项目目录下（项目配置）。


**某个Git命令如何得到详细的帮助：**

比如我想知道`config`命令的详细介绍，那么我可以输入：

```bash
git help config
```



## 创建本地版本库并提交文件

### 创建本地版本库

```bash
$ mkdir mysite  //创建一个名为mysite的目录
$ cd mysite //进入mysite的目录

# 在当前目录下创建版本库
$ git init   

Initialized empty Git repository in e:/codes/mysite/.git/

## 下载一个项目和它的整个代码历史
git clone [url]
```

整个`mysite`文件夹称之为**工作区**。最后生成的`.git`文件夹就是**版本库**。


### 提交文件

- `git add`：把文件修改添加到暂存区。
- `git commit`：把暂存区的所有修改提交到版本库（提交到当前分支）。

**`git add`的使用如下：**

```bash
$ git add .  //添加当前目录下的所有文件
$ git add readme.txt  //添加指定文件
$ git add src/   //添加指定目录（含子目录）
$ git add src/\*.txt    //添加src目录下的所有txt文件

```

PS：可以使用`git status`查看状态。


**`git commit`的使用如下：**

```bash
# 提交暂存区到仓库区
$ git commit -m "一些说明"

# 使用一次新的commit，替代上一次提交
# 如果代码没有任何新变化，则用来改写上一次commit的提交信息
$ git commit --amend -m "一些说明"

# 重做上一次commit，并包括指定文件的新变化
$ git commit --amend [file1] [file2] ...

```

PS：可以使用`git log`查看版本提交记录。每提交一个新版本，实际上Git就会把它们自动串成一条时间线。这条命令可以更清楚地看到提交历史的时间线。

`commit id`（版本号）是使用SHA-1算法产生唯一标识符，保证全球唯一。


### 小节

- git config（使用git命令之前，如何配置用户信息？）

- git help config（如何使用帮助）

- git init (git 初始化，创建版本库)

- git status (如何查看git管理的状态)

- git add (如何跟踪文件)

- git commit ( 如何提交到版本库中？)

- git log (如何查看提交记录)


## 工作区、暂存区的概念

- untracked：没有被跟踪（即未被add）
- Workspace：工作区
- Index / Stage：暂存区
- Local Repository：本地仓库/本地版本库
- Remote Repository：远程仓库

来看下面这张图：

img2016110601


**工作区：**

就是我们进行工作的地方。


**暂存区（Working Directory）：**

暂存（index），又名暂存区（staging erea）。位于文件夹`/.git/index`下。

暂存区是可以设置哪些变更要提交到版本库，哪些先不提交。

**本地仓库（local repository）：**

本地仓库，就是我们自己工作的电脑上保存版本数据的地方。位于文件夹`/.git/object`下。

**远程仓库（remote repository）：**

远程仓库，我们用Git进行操作，为了防止数据在自己电脑上丢失，比如错误删除，病毒攻击等原因造成了数据丢失，我们需要备份到远程的服务器上，这个服务器可以理解为远程仓库。








## 其他操作


**[修改commit message](http://stackoverflow.com/questions/179123/edit-an-incorrect-commit-message-in-git)：**

```bash
git commit --amend -m "New commit message"
```



**强制push，[覆盖](https://ruby-china.org/topics/7365)远程版本：**

```bash
git push origin master -f
```







## Others

### 参考书籍

- 《[Git权威指南](https://book.douban.com/subject/6526452/)》



### 参考链接

- [Gitlab的使用](https://blog.cnbluebox.com/blog/2014/04/15/gitlabde-shi-yong/)

从这里知道了图形界面工具[SoureTree](http://www.sourcetreeapp.com/)

- [常用 Git 命令清单](http://www.ruanyifeng.com/blog/2015/12/git-cheat-sheet.html)













