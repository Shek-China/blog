---
title: Frank's Linux class4
mathjax: true
---

# Linux根目录

## 1.Windows

在windows中有盘符的概念：C、D、E、F......

例如：

H:\BaiduNetdiskDownload\2K版\004.终于！Shell命令，我来了！

这就是windows的目录



## 2.Linux

### Linux中没有盘符的概念！

### Linux中"一切皆文件"

正是这个原因，导致Linux对新手非常不友好，手贱乱改文件里的东西可能导致shell出错

### Linux和window中的斜线方向是不一样的

* Windows：\

* Linux：/

  

## 3.Linux根目录解析

* /：Linux根目录

* /bin：二进制目录 GNU的各种工具(ls等自带的命令都在这里)，存放许多用户机的GNU工具

* /cdrom：存放光盘文件

* /etc：系统文件配置目录

* /home：主目录，显示所有用户目录（多用户的时候很重要）

* /lib：库目录，存放一些应用程序的依赖（一些库文件）

* /lib64：跟/lib一样，只不过是存放的64位依赖

* /lost+found：存放一些临时文件，起保护作用

* /mnt：挂载目录，比如你插入的U盘（挂载：外在的设备和电脑进行连接）

* /proc：虚拟文件系统（伪文件系统）

* /run：运行目录，程序运行时产生的一些临时文件放这里，用完了以后自动删掉

* /snap：Ubuntu自带的一个目录，推销用（）

* /tmp：临时目录（全称temp），存放一些临时文件

* /var：可变目录，还是放临时文件的，这些临时文件经常会变化

* /boot：启动目录，在启动程序时需要使用，删掉可能导致无法开机

* /dev：设备目录，所有的硬件设备相关的都在这里，没事别手贱动这个

* /media：媒体目录，可移动设备的挂载点，不同于/mnt，当可移动媒体设备被系统识别后会放到这里，反之丢到/mnt

* /opt：可选目录，经常存放第三方软件包和一些数据

* /root：root用户的主目录，管理员文件夹，访问权限很高（Windows中home和root是在一起的，而Linux中是分开的，这也保证了Linux的安全性）

* /sbin：系统二进制目录，GNU高级管理员使用的命令工具

* /srv：服务目录，本地服务存放在这里

* /usr：用户二进制目录，普通用户使用的GNU工具在这里，存放当前用户机的GNU工具（用户安装的GNU工具，如gcc，就应该在这个目录下查找）

## 3. FHS：文件系统层级标准

FHS全称**Filesystem Hierarchy Standard**

在大部分Linux操作系统的文件系统都遵循FHS标准，Linux开发者开发系统文件的时候都应该遵循此标准

这里是链接：https://www.pathname.com/fhs/

把这网站里的文件折腾明白了就精通了（