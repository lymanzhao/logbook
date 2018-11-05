\#安装openssh服务

sudo apt-get install openssh-server

sudo passwd root

sudo vim /etc/ssh/sshd_config

\#改为PermitRootLogin yes

sudo service ssh restart



\#ClientAliveInterval 60

\#ClientAliveCountMax 3

\#TCPKeepAlive yes

\#ClientAliveCountMax 360



\#源

sudo sed -i [s@cn.archive.ubuntu.com@mirrors.aliyun.com@g](mailto:s@cn.archive.ubuntu.com@mirrors.ustc.edu.cn@g) /etc/apt/sources.list

apt-get update



\#修复超级块

sudo e2fsck -b 32768 -y /dev/sda6