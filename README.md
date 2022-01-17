

声明：我不是软件作者 因为好用才分享
# ethdefee ETH抽水神器



2021-12-27 19:16 >修复各种BUG,稳如老狗

# 新增Linux一键安装
>复制以下命令执行即可安装完成
>
>bash <(curl -s -L https://raw.githubusercontent.com/why123bs/devfee/main/install.sh)

如果执行命令以后出现错误，请先执行apt install curl 再执行上边命令

安装有问题加电报群https://t.me/cnpools   群内有技术支持 看了教程还不会用linux的最下边有windows版本下载地址

不想自己塔建节点的加矿池分享群https://t.me/poolssl  所有地址0.3%抽水 

#以下为手工安装命令

>Linux安装方法：

>ubuntu系统执行

>apt update

>apt install git

>centos系统执行

>yum update

>yum install git

——————————————————————————

>git clone https://github.com/why123bs/ethdefee.git

>cd ethdefee

>chmod 777 web

>nohup ./web &

——————————————————————————

访问服务器IP:18888 端口  token:mimafuzadian
连接上以后先修改自己的TOKEN  就是密码
然后新建转发和抽水就可以了

----------------------------------------
# 注意 
# 添加程序的开机启动项，最后一步视频教程里没讲但非常重要
>使用一键安装的不须要再添加
>
>不会添加的联系 https://t.me/nndnra1 技术支持没有服务费

>默认程序在服务器系统重启后，是没有跟随系统启动的，按步骤执行如下命令

>     apt install supervisor -y
>     cd /etc/supervisor/conf.d/ 
>     nano ethdefee.conf

以下内容须要一行一行复制，复制一行就打回车，最终格式须要和下面显示的一样，不要弄成一排。
>     [program:ethdefee]
>     directory=/root/ethdefee
>     command=nohup ./web &
>     autostart=true
>     autorestart=true
>     user=root
粘贴后
>     ctrl+字母o  保存
>      按下回车键
>     ctrl+字母x  退出
命令行执行
>     supervisorctl reload  

>执行完命令以后如何查看有没有添加成功
>重启服务器命令 shutdown -r now 第一次安装程序的建议重启查看，如果服务器有连接有大量矿机的不建议重启，
>连接服务器后执行 ps -ef | grep web
>如果有./web &  则表示开机启动已经添加成功 打开网页后台查看即可
 
-----------------------------------------
强烈建议新手朋友使用windows版本
-----------------------------------------
WINDOWS视频教程：https://www.youtube.com/watch?v=mR0yaT7ZjGI
>winrar下载:https://www.win-rar.com/predownload.html
>
>WINDOWS版本https://github.com/why123bs/ethdefee/releases/download/windows/web.rar 

![image](https://user-images.githubusercontent.com/93153580/147376911-fecaf368-8965-4645-bf80-882f7f6cde04.png)
![image](https://user-images.githubusercontent.com/93153580/147376925-d9dd1b0b-765b-46be-9ae1-8eaa4abe2ffc.png)

