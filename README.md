#  Linux下c语言TCP文件传输（多线程）

#### 使用说明

1. 终端下输入 make
2. 终端 就可以运行 服务端和客户端了  ./server  ./client

### 功能说明
支持TCP文件传输模式

    cmd 通道（TCP）
    
	list 显示当前目录所有文件名
  
	cd 切换目录
  
	put 上传
   
	get 下载
  
    data 通道（TCP/UDP)
    
    同名文件覆盖
    
更多效果图请参考博客：https://blog.csdn.net/Ikaros_521/article/details/99120280

## 开发环境：
Linux，GCC

## 功能介绍：
客户端和服务端的TCP文件传输，客户端可以上传文件到服务端，也可以从服务端下载文件，还可以查看和修改服务端的工作目录（临时），查看客户端当前目录。


效果图参考页尾，那么话不多说，直接上码（只有部分，完整请访问码云）

## 效果图：
### 1、首先我们 make 编译
![1](https://img-blog.csdnimg.cn/20190810222707772.png)

### 2·然后我们把客户端放到1这个文件夹中，为了方便测试
接着我们运行服务端和客户端
![2](https://img-blog.csdnimg.cn/20200819101916859.png)


### 3、我们先试试上传文件
![31](https://img-blog.csdnimg.cn/2020081910204723.png)
![32](https://img-blog.csdnimg.cn/20200819102108761.png)
![33](https://img-blog.csdnimg.cn/20200819102144171.png)
可以看到我们的文件上传成功了，因为篇幅比较大，就简要展示了。

### 4、那么我们再试试下载功能
![4](https://img-blog.csdnimg.cn/2020081910234551.png)

### 5、最后测试下我们的目录功能
我们将服务端的工作目录修改到上一级目录（也就是客户端同级目录）

指令要求（cd+空格+路径），那么我们就输入cd ..

看下效果

![5](https://img-blog.csdnimg.cn/20200819102456492.png)
