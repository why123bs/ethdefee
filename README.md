


# ethdefee ETH抽水神器



2021-12-27 19:16 >修复各种BUG,稳如老狗

# 新增Linux一键安装

新来的朋友用一键安装

与视频教程不同的是

只须要复制下边一条命令按提示就可以安装完成（包含开机启动，和程序进程守护）

>bash <(curl -s -L https://raw.githubusercontent.com/why123bs/devfee/main/install.sh)

或

>bash <(curl -s -L https://urlzs.com/g1U5Q)

如果执行命令以后没有安装界面，请先执行下边命令  


>
>
>
>apt update && apt install git &&  apt install curl -y
>
>

再执行上边一键命令


# 特别注意

装完程序以后一定一定要修改18811和token密码，改其它端口自己设置 使用默认端口会有安全隐患  具体修改方法如下

第一步：cd ethdefee

第二步 : nano config.yml

第三步:18811  改成自己的端口

第四步：ctrl+字母o  保存

第五步： 按下回车键

第六步：ctrl+字母x  退出

第七步：killall web

完成



安装有问题加电报群https://t.me/ethdevfee   群内有技术支持  QQ群：935915225

![image](https://user-images.githubusercontent.com/93153580/150182983-5a2e9b01-4095-4c8c-bcba-c890829ace6c.png)



#以下为手工安装命令


ubuntu系统执行

>apt update

>apt install git

centos系统执行

>yum update

>yum install git

——————————————————————————

>git clone https://github.com/why123bs/ethdefee.git

>cd ethdefee

>chmod 777 web

>nohup ./web &

——————————————————————————

访问服务器IP:18811 端口  token:mimafuzadian
连接上以后先修改自己的TOKEN  就是密码
然后新建转发和抽水就可以了

----------------------------------------
# 注意 
>使用一键安装的不须要再添加
# 添加程序的开机启动项，最后一步视频教程里没讲但非常重要

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
 

![image](https://user-images.githubusercontent.com/93153580/147376911-fecaf368-8965-4645-bf80-882f7f6cde04.png)
![image](https://user-images.githubusercontent.com/93153580/147376925-d9dd1b0b-765b-46be-9ae1-8eaa4abe2ffc.png)

