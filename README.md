# fuckgfw

# 用Shadowsocks + FinalSpeed 实现翻墙+双向加速！

# Shadowsocks搭建

1、Linode买Fremont机房的VPS。安装CentOS系统，开机。

2、用putty，登陆服务器。

3、输入：yum -y install wget

4、输入下面：

wget –no-check-certificate https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocks.sh

5、输入：chmod +x shadowsocks.sh

6、输入：./shadowsocks.sh 2>&1 | tee shadowsocks.log

7、设置密码：xxx     设置端口：xxx     选择：7）aes-256-cfb加密

8、点击任意键进行安装。

9、安装完成！

# 分割线

现在虽然搭建完SS，但就算再好的VPS，速度都会很慢。

这时就必须要加速器了，锐速这种单向加速器和那些收费的不说。这里说的是免费的双向加速器 FinalSpeed ！

# FinalSpeed

1、安装完SS后，开始进行FS的服务器端搭建：

一键安装代码：

wget -N --no-check-certificate https://raw.githubusercontent.com/91yun/finalspeed/master/install_fs.sh && bash install_fs.sh

2、安装完成会显示：finalspeed start success.

3、下载FS客户端.exe。输入：服务器IP地址、传输协议、物理带宽（输入高于物理带宽可能会丢包）。

   加速列表：名称ss、加速端口（你的SS端口）、本地端口（随便设，例如2000）。

4、SS添加新服务器、服务器地址127.0.0.1、服务器端口2000、密码、加密aes-256-cfb、代理端口1080。

5、然后看FS界面显示连接成功和速度。双向加速速度和没连VPN差不多快就说明搭建成功了！

# 在手机中使用FS加速功能

1、在Shadowsocks中连接127.0.0.1的服务器，右键勾选“允许来自局域网的连接”，并且开启连接服务器。

2、在手机选择与电脑的同一个无线网络，并在代理设置中输入电脑IP（cmd-ipconfig-ipv4）和端口1080。

   注意：
   1、手机和电脑必须在同一网络下。
   2、SS必须勾选允许来自局域网的连接。
   3、电脑SS和FS必须处于启动状态下才能在手机中连接。

3、用完记得关闭代理，否则手机会无法上网。
