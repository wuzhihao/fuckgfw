# fuckgfw
# 写来自己看的 （￣▽￣）
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

9、安装完成！Enjoy it !

# 分割线

现在虽然搭建完SS，但就算再好的VPS，速度都会很慢。

这时就必须要加速器了，锐速这种过时的单向加速器和那些收费的就别说了。

这里说的是免费的双向加速器 FinalSpeed ！

# FinalSpeed

1、
