# hifile

#### 一 、介绍
hifile是一款基于Linux的开源文件防篡改软件，对目录文件保护实时生效，保护关键文件不被黑客篡改。

#### 二 、主要用途
##### 1、对重要目录只读  

```
可以对/etc/、网站等敏感目录进行监控，设置只能读，不能修改和删除。
```


##### 2、防止黑客利用未知RCE漏洞，落地木马或者修改服务器重要文件

    现在高级漏洞都不直接公开了，上升为国家之间情报战略，秘密潜伏的木马文件比破坏的多得多。



#### 三、系统内核要求
要求内核版本大于5.10，推荐2023年以后的linux发行版本：

Debian 12+

RHEL 9.0+

Rocky Linux 9.0+

Fedora 36+

...

编译环境需要gcc、make，先用apt install libelf-dev或者yum install  elfutils-libelf-devel安装好依赖库后，
用root用户，直接make运行./file-tamper即可，默认保护/root/目录文件不被篡改，可以用rm或者vi编辑修改/root/下的文件，将报错。

商业版集成到全流量防火墙防御系统OpenHFw中，支持Linux x86 64位系统（内核大于5.0），保证可以上网，以root权限运行下面命令：

    1、 wget http://101.42.31.94/openhfw  (每天限10个下载体验）
    2、 chmod +x ./openhfw
    3、 ./openhfw

首次安装下载大约半分钟，出现System is running.....代表安装成功，可以WEB管理口9998（防火墙允许）登录进去。

#### 五、运行停止卸载
启动运行:  ./openhfw         后台模式运行:   ./openhfw daemon

停止运行:  ./openhfw stop    卸载 :   rm  /openhfw/ -rf

默认没加开机启动，请自行把openhfw 加入开机启动程序。

#### 四、商业版演示地址

商业版演示地址 [http://39.106.251.213:9998/ok.html](http://39.106.251.213:9998/ok.html)

#### 五、源码部署请加微信号httpwaf

![](https://gitee.com/httpwaf/httpwaf/raw/master/img/wechat.png)

#### 六、来一张首页大图

![](https://gitee.com/httpwaf/httpwaf/raw/master/img/home.png)
