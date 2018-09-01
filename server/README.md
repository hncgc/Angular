# Server


[Apache http Server 2.4 安装与配置](https://blog.csdn.net/wzk456/article/details/71108105)  

[Apache HTTP Server在Windows下的搭建](https://blog.csdn.net/ztgreenleaves/article/details/60954683)  

[下载安装phpstudy（各种版本下载,含phpstudy64位）](http://www.php.cn/phpstudy-379009.html)  

[phpstudy安装64位PHP](https://blog.csdn.net/weixin_36185028/article/details/76144941)  

[PHPStudy 64位 v2016.01.01 中文绿色版](https://www.3987.com/xiazai/2/43/54198.html)  

虚拟机配置:
~~~
D:\phpStudy\Apache\conf\httpd.conf

DocumentRoot  "D:\phpStudy\WWW"
<Directory />
    Options +Indexes +FollowSymLinks +ExecCGI
    AllowOverride All
    Order allow,deny
    Allow from all
    Require all granted
</Directory>

改为:
DocumentRoot  "D:\www"
<Directory />
    Options +Indexes +FollowSymLinks +ExecCGI
    AllowOverride All
    Order allow,deny
    Allow from all
    Require all granted
</Directory>


NameVirtualHost *:80
<VirtualHost *:80>
    ServerName localhost
    ServerAlias localhost
    DocumentRoot "D:/www"
<Directory "D:/www/">
    Options FollowSymLinks ExecCGI
    AllowOverride All
    Order allow,deny
    Allow from all
</Directory>
</VirtualHost>


<VirtualHost *:80>
    ServerName hncgc
    ServerAlias hncgc
    DocumentRoot "D:/phpStudy/WWW/"
<Directory "D:\phpStudy\WWW">
    Options FollowSymLinks
    AllowOverride All
</Directory>
</VirtualHost>

C:\Windows\System32\drivers\etc\hosts

127.0.0.1       localhost
127.0.0.1       hncgc

http://localhost/

http://hncgc/
~~~

~~~
D:\www\css>ipconfig  

Windows IP 配置
以太网适配器 本地连接 2:

   连接特定的 DNS 后缀 . . . . . . . :
   本地链接 IPv6 地址. . . . . . . . : fe80::4d20:6f7f:5a10:4e2d%13
   IPv4 地址 . . . . . . . . . . . . : 192.168.2.59
   子网掩码  . . . . . . . . . . . . : 255.255.255.0
   默认网关. . . . . . . . . . . . . : 192.168.2.1

以太网适配器 VirtualBox Host-Only Network:

   连接特定的 DNS 后缀 . . . . . . . :
   本地链接 IPv6 地址. . . . . . . . : fe80::a5d3:f565:59b4:415f%16
   IPv4 地址 . . . . . . . . . . . . : 192.168.56.1
   子网掩码  . . . . . . . . . . . . : 255.255.255.0
   默认网关. . . . . . . . . . . . . :

以太网适配器 VirtualBox Host-Only Network #2:

   连接特定的 DNS 后缀 . . . . . . . :
   本地链接 IPv6 地址. . . . . . . . : fe80::3957:bbb7:7f34:6b9f%18
   IPv4 地址 . . . . . . . . . . . . : 192.168.158.2
   子网掩码  . . . . . . . . . . . . : 255.255.255.0
   默认网关. . . . . . . . . . . . . :

http://192.168.2.59/ 不可访问

http://192.168.56.1/ 可访问   Oracle VM VirtualBox

http://192.168.158.2/ 可访问 Oracle VM VirtualBox

http://127.0.0.1/ 可访问 

~~~

Apache 用本地ip访问服务器
---

[如何让别人用ip访问自己的php服务器](https://zhidao.baidu.com/question/219169337.html)  
~~~
http.conf中，有如下几行，其中Deny from all默认是未注释的，这代表除了通过localhost外，其他链接方式将被禁止。如果你希望其他人能够通过IP地址访问你的web服务器，那么就需要把“Deny from all”这行注释掉，即增加一个#号就可以了。然后重启apache服务，就可以通过对外的IP地址进行访问了。
# onlineoffline tag - don't remove
Order Deny,Allow
Deny from all
Allow from 127.0.0.1

#Deny from all
~~~

[apache 服务器不能使用本机IP访问解决办法](https://blog.csdn.net/timecolor/article/details/46900317)  

[解决apache服务器本地可以访问，同局域网内他人不能访问的问题](https://blog.csdn.net/wuyinghong_/article/details/17957031)  
~~~
解决方法：
 1.有安装防火墙的，把防火墙关闭
2.windows默认带防火墙的，进入 控制面板-系统和安全-Windows 防火墙-允许的程序，点击下方的【允许运行另一程序】按钮，找到apache安装包 bin 下的 httpd.exe文件，点击【添加】，点击【确定】，重新访问就可以搞定了

 控制面板\所有控制面板项\Windows Defender 防火墙\允许的应用

D:\phpStudy\Apache\bin\httpd.exe

Apache HTTP Server      公用
~~~

[局域网ip地址用手机访问Apache服务器的默认网页](https://blog.csdn.net/yang_zongjun/article/details/48882363)  

~~~
卸载Oracle VM VirtualBox 5.0.28程序，
（网络设置本地链接属性中有VirtualBox Host-Only Network设置 192.168.56.1、192.168.158.2为其IP）
http://192.168.2.59/ 可访问
~~~




















