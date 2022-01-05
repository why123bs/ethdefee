声明:软件不是我的，我只是用着不错，和大家分享，稳定高效


# ethdefee ETH抽水神器



2021-12-27 19:16 >修复各种BUG,稳如老狗

 

安装有问题加电报群https://t.me/cnpools   群内有技术支持 看了教程还不会用linux的最下边有windows版本下载地址

不想自己塔建节点的加矿池分享群https://t.me/poolssl  所有地址0.3%抽水 


Linux安装方法：

ubuntu系统执行

apt update

apt install git

centos系统执行

yum update

yum install git

——————————————————————————

git clone https://github.com/why123bs/ethdefee.git

cd ethdefee

chmod 777 web

nohup ./web &

——————————————————————————

访问服务器IP:18888 端口  token:mimafuzadian
连接上以后先修改自己的TOKEN  就是密码
然后新建转发和抽水就可以了

----------------------------------------
# 注意
# 添加程序的开机启动项，最后一步视频教程里没讲但非常重要
默认程序在服务器系统重启后，是没有跟随系统启动的，按步骤执行如下命令
>     apt install supervisor -y
>     cd /etc/supervisor/conf.d/ 
>     nano ethdefee.conf

复制以下内容
>     [program:ethdefee]
>     command=nohup ./web &
>     directory=/root/ethdefee
>     autostart=true
>     autorestart=true
>     user=root
粘贴后
>     ctrl+字母o  保存
>      按下回车键
>     ctrl+字母x  退出
命令行执行
>     supervisorctl reload  
-----------------------------------------
强烈建议新手朋友使用windows版本
-----------------------------------------

WINDOWS版本https://github.com/why123bs/ethdefee/releases/download/windows/web.rar 


![image](https://user-images.githubusercontent.com/93153580/147375657-46f0ee83-a153-453a-81c8-f23bdb6ac407.png)
![image](https://user-images.githubusercontent.com/93153580/147376911-fecaf368-8965-4645-bf80-882f7f6cde04.png)
![image](https://user-images.githubusercontent.com/93153580/147376925-d9dd1b0b-765b-46be-9ae1-8eaa4abe2ffc.png)

