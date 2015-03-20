---
layout: post
title: DDMS下无法读取data目录的解决方案
categories:
 - 教程
 - Android
 - Eclipse
 - DDMS
tags:
 - Android
 - Eclipse
 - DDMS
 - ROOT
 - 解决方案
 - 教程
listimg: /images/article/rootloaddata/eclipse_4.4.0_about_screenshot.png
listimgalt: 教程中Eclipse版本
---
安卓开发往往需要获取系统目录下的文件用作分析，但是在我们开发过程中发现，/data这个文件夹有时候无法获取里面的文件，那是因为你对Android(Linux) 文件权限机制还不够了解。

<!-- more -->

>本教程使用的Eclipse 版本如下：

>![{{ page.listimgalt }}]({{ page.listimg }})

###解决前提

>- 设备已经root
>- RE 文件管理器 或者ES 文件管理器 等 安卓应用

###解决方案


####例子

>想要获取/data/下的文件

####文字步骤

>  1. 在/data文件夹列表上长按
 2. 进入权限设定
 3. 在“其他”的读或写上打钩（需要读权限就读上打钩，都需要就都打钩），并按确定
 4. 在DDMS的File Explorer 面板里点击/data左边的箭头就可以展开文件列表

####截图展示

![在/data文件夹列表上长按](/images/article/rootloaddata/root_load_data_dir_lists_permission_771.png)

![进入权限设定](/images/article/rootloaddata/root_load_data_dir_longpress.png)

![在“其他”的读或写上打钩（需要读权限就读上打钩，都需要就都打钩），并按确定](/images/article/rootloaddata/root_load_data_dir_permission_777.png)

![在DDMS的File Explorer 面板里点击/data左边的箭头就可以展开文件列表](/images/article/rootloaddata/fileexplorer_777_accessed.png)

 



