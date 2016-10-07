![](http://portrait7.sinaimg.cn/1664452254/blog/180)
## DOL框架描述
DOL（distributed operation layer）是一个用于平行应用编程的软件开发框架。DOL允许基于卡恩网络计算模型区分应用程序并且基于systemC特性化一个模拟引擎。此外，DOL提供了一个基于xml的规范格式来描述在一个多处理器系统中实现并行应用程序的过程,包括绑定和映射。
## DOL安装笔记
* 安装一些必要环境
* sudo apt-get update
* sudo apt-get install ant
* sudo apt-get install openjdk-7-jdk
* sudo apt-get install unzip
* 下载文件dol & systemc并解压
* 进入systemC目录，新建临时文件夹objdir，进入objdir，运行configure
* 编译systemC
* 进入dol文件夹，修改 build_zip.xml
* 编译dol
## 实验感想
第一次实验很简单，按照文档一步一步来就可以了。虚拟机还是怪坑的，如果把文件直接拖进去很有可能出现复制不完全的情况，所以还是先复制，再在虚拟机内右键粘贴保险一点。在最后一步的时候没有能build成功，检查发现是之前的库没有安装好。
ADD TEST
