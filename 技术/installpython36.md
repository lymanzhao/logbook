# [源码安装Python3.6](https://www.cnblogs.com/weifeng1463/p/7883765.html)



### 一、安装环境及版本

　　　　 CentOS 6.5
　　　　 Python 3.6.1

### 二、安装依赖包

##### 1、安装静态库

```
# yum install -y openssl-static
```

###### 注：如果不安装该静态库，会导致python的pip安装失败

##### 2、安装gcc

```
# yum install -y gcc wget
# yum groupinstall "Development tools"
# yum install zlib-devel bzip2-devel openssl-devel ncurses-devel sqlite-devel readline-devel tk-devel gdbm-devel db4-devel libpcap-devel xz-devel
```

### 三、下载和安装Python3

##### 1、通过官网下载Python3安装包

```
# wget http://python.org/ftp/python/3.6.1/Python-3.6.1.tar.xz
```

##### 2、解压安装包

```
# tar xf Python-3.6.1.tar.xz
```

##### 3、编译安装

进入Python-3.6.1文件夹下，进行编辑安装

```
# ./configure --prefix=/usr/local/python3
# make & make install
```

###### 注：--prefix设置的是python3要安装到的位置

### 四、添加文件链接（添加到环境变量）

##### 1、添加刚安装的python3版本的文件连接

```
# ln -s /usr/local/python3/bin/python3 /usr/bin/python3
```