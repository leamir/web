---
title: Port Forwarding
sidebar_label: Port Forwarding
description: Server port forwarding tutorial.
---

**欢迎来到端口转发教程!**

此教程是Leopard编写的端口转发教程.

你所需要的是一个samp-server或omp-server以及一个路由器。如果你没有路由器，那么你不需要进行端口转发!

## 开始

首先找到你的**网关(gateway)**。假设你使用的是Vista系统。点击开始，点击搜索栏，输入**cmd**。然后会出现一个黑框。输入以下内容；**ipconfig**。等待文本加载完毕，然后在其中查找。直到你找到**网关(gateway)**，并且不要关闭黑框!

找到之后，打开浏览器。当它加载完毕后，在地址栏输入**网关(gateway)**值（例如：192.168.0.1/192.168.1.1）。按下回车.

## 路由器配置

做得好，你已经进入了路由器的配置页面。接下来我们需要进行端口转发.

所以……在该页面上有一个名为以下之一的类别;

- 虚拟服务器(Virtual Server)
- 端口转发(Port Forwarding)
- 端口控制(Port Control)
- 应用共享(Application Sharing)
- 任何名称中带有`端口`的选项.

如果你找到了它，点击它。然后，点击 '添加新条目(Add new)', '新端口(New Port)' 或其他按钮以开启新端口.

输入以下详细信息:

```
端口(Port)：服务器的端口（默认：7777）
端口类型(Port Type)：UDP
启用(Enabled)：是
**IP：继续第3步**
```

现在你需要知道你的电脑IP地址.

## 获取IP，继续

现在，最大化黑框并再次查看文本，直到你看到**_IPv4_**。它的格式应该是这样的：**192.168.0.100**。复制它，这就是你的IP地址！继续填写路由器主页上的信息。例如，我的IP是192.168.0.100

```
端口(Port)：服务器的端口（默认：7777）
端口类型(Port Type)：UDP
启用(Enabled)：是
IP：192.168.0.100
```

然后点击**保存(save)**。接着你就完成了。并且！不要忘记在**Windows防火墙**中进行端口转发。这是一个简短的教程;

进入开始菜单，在搜索栏中输入 "防火墙(firewall)" 并选择 "Windows防火墙(Windows Firewall)". 打开它并点击 _更改设置(Change preferences)_. 弹出一个新窗口. 点击 _例外(Exceptions)_ 选项卡, 点击 _添加端口(Add port).._ 然后填写以下信息;

```
名称(Name): SA-MP Server (名称可以随意)
端口号(Port Number): 服务器的端口 (默认: 7777)
协议(Protocol): UDP
```

然后就完成了！点击确定并关闭它。启动服务器，看看它是否有效. 如果有效, 进入你的SA-MP客户端并输入: localhost:端口(默认: 7777). 如果ping发生变化，那么你的服务器运行完全正常。接下来你只需前往:

[WhatIsMyIP.COM](http://whatismyip.com).

## 完成

到达该页面后，获取屏幕上的IP。再次进入你的SA-MP客户端, 将该IP添加到收藏夹并在IP的末尾添加 服务器的端口(默认: 7777)，如果正常运行,

**恭喜你**! _你已经成功完成了端口转发_!
