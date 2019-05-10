



## SVN 本地操作

### 添加ignore文件

"SVN--> add to ignore list "


### 修改已提交日志信息

（1）选择指定目录后，右键选择「show log」；

（2）在出来的日志列表对话框中，选择某个提交版本，再点击右键，选择「Edit log message」。


由于缺省情况下为安全起见Subversion不允许开发人员修改已提交reversion的日志信息，这样会报错误，提示不能修改以及请SVN管理员安装pre revprop change hook。

这个hook是什么意思呢? 实际上是一个版本日志变更的预处理程序，主要是用来保存老的日志信息，以避免在变更发生错误的时候，无法恢复。

那么需要管理员执行以下操作，就可以赋予开发人员变更日志的操作能力：

```bash
#cd /opt/svn/repos/hooks  
#mv pre-revprop-change.tmpl pre-revprop-change  
#chmod 755 pre-revprop-change  
```


参考链接：[SVN:修改已提交日志信息](http://blog.csdn.net/iefreer/article/details/19755595)






