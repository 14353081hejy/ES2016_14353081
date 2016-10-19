##1.实验过程：
1）编辑文档：
*Deadlock.java

![Paste_Image.png](http://upload-images.jianshu.io/upload_images/3230336-8f447b379e7f9756.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


![Paste_Image.png](http://upload-images.jianshu.io/upload_images/3230336-291374f06825dc3c.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
*Deadlock.bat

![Paste_Image.png](http://upload-images.jianshu.io/upload_images/3230336-639b2923108a8762.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

*Deadlock.sh（因为虚拟机中无法直接运行bat文件）

![Paste_Image.png](http://upload-images.jianshu.io/upload_images/3230336-6e79ba214d12ee72.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
2）编译.java文件：
javac Deadlock.java
3）运行.sh文件
./Deadlock.sh
##2.实验截图：

![Paste_Image.png](http://upload-images.jianshu.io/upload_images/3230336-77ae6c9148e55ed3.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

##3.产生死锁的必要条件：
1）互斥
2）占有并等待
3）非抢占
4）循环等待
##4.实验结果解释：
对于synchronized，当它用来修饰一个方法或者一个代码块的时候，能够保证在同一时刻最多只有一个线程执行该段代码。当一个线程访问object的一个synchronized同步代码块或同步方法时，其他线程对object中所有其它synchronized同步代码块或同步方法的访问将被阻塞。
通过改变count的值，增长延时，会增加a和b同时调用method的机率，而又因为synchronized会将线程的访问阻塞从而造成死锁。
