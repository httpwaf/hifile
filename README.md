# hiddos

#### 一 、介绍
hiddos是一款基于Linux 进程防火墙和抗DDOS流量防火墙为一体的产品，以弥补iptables没有的功能。

#### 二 、主要用途
##### 1、DDOS防护  

```
可以直接安装在服务器上，大幅降低DDOS攻击流量防御费用，高版本内核采用XDP下一代防火墙技术。
```


##### 2、发现黑客利用未知RCE漏洞，直接在服务器上安装后门

    现在高级漏洞都不直接公开了，上升为国家之间情报战略，秘密潜伏的进程比破坏的多得多。



#### 三、系统支持和主要功能
支持Linux x86系统，主要功能有：

1、 全程记录Linux每个进程的IP、进出流量、在线时长等数据。

2 、用AI技术分析危险进程，异地IP/异常流量/危险行为等将报警。

3 、自动记录各种流量峰值，生成DDOS防御参数，也可以和应用层WAF等联动精确阻断CC/DDOS。

4、安装方法用root权限运行./hiproc命令即可，无需任何设置，更多请参考详细说明书。


#### 四、商业版演示地址

商业版也可以开源，演示地址 [http://59.110.1.135:9998/hiddos.html](http://59.110.1.135:9998/hiddos.html)

#### 五、源码部署请加微信号httpwaf

![](https://gitee.com/httpwaf/httpwaf/raw/master/img/wechat.png)

#### 六、来一张首页大图

![](https://gitee.com/httpwaf/hiproc/raw/master/img/home.png)