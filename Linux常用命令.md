


显示所有文件：（含隐藏文件）

```bash
ls -la
```



### not a directory

使用adb push 一个文件到手机中一个并不存在的目录下。虽然显示push成功了，但是cd 到那个目录下时，却显示`not a directory`。

原因是：要先使用mkdir创建这个文件夹，才能再push文件进去。



### 查看文件大小

http://www.cnblogs.com/xxoome/p/5891768.html


进入指定文件夹，输入如下命令：


```bash
du -sh *
```





