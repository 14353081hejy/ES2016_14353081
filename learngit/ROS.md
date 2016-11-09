##一、实验目的
安装ROS
##二、安装过程
__1 首先确定虚拟机版本（我的为ubuntu 14.04__
***
**2  Installation**
  sudo apt-get update
  sudo apt-get install libgl1-mesa-dev-lts-utopic
***
**3 Desktop-Full Install**
 sudo apt-get install ros-jade-desktop-full
***
**4 Initialize rosdep**
  sudo rosdep init
  rosdep update
***
**5 Environment setup**
echo "source /opt/ros/jade/setup.bash" >> ~/.bashrc
source ~/.bashrc
***
**6 Getting rosinstall**
sudo apt-get install python-rosinstall
##三、实验结果

![Paste_Image.png](http://upload-images.jianshu.io/upload_images/3230336-8eb6be15939078e3.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
由图可见 ros安装成功。
##四、实验感想
* ros简介
ROS是开源的，是用于机器人的一种后操作系统，或者说次级操作系统。它提供类似操作系统所提供的功能，包含硬件抽象描述、底层驱动程序管理、共用功能的执行、程序间的消息传递、程序发行包管理，它也提供一些工具程序和库用于获取、建立、编写和运行多机整合的程序。
ROS的首要设计目标是在机器人研发领域提高代码复用率。ROS是一种分布式处理框架（又名Nodes）。这使可执行文件能被单独设计，并且在运行时松散耦合。这些过程可以封装到数据包（Packages）和堆栈（Stacks）中，以便于共享和分发。ROS还支持代码库的联合系统。使得协作亦能被分发。这种从文件系统级别到社区一级的设计让独立地决定发展和实施工作成为可能。上述所有功能都能由ROS的基础工具实现。
