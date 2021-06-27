---
title: 使用Oracle VM VirtualBox安装虚拟机系统
tags:
  - GNU/Linux
  - Oracle VM VirtualBox
categories:
  - 教程
cover: 'https://i.loli.net/2021/06/20/F3aYsSvunODeZCN.png'
top_img: 'https://i.loli.net/2021/06/20/F3aYsSvunODeZCN.png'
updated: 2021-04-20 00:00:00
date: 2021-04-20 00:00:00
---


#  **前言**
&ensp;&ensp;&ensp;&ensp;一般情况我们因为各种原因，日常使用的办公学习电脑都是**Windows**、**MacOS**，并没有接触过**Linux**，这里我们就直接使用虚拟机安装使用**Linux**，推荐使用[**Oracle VM VirtualBox**](https://www.virtualbox.org)虚拟机软件进行安装，下载后我们正常安装即可。有了好的虚拟机软件，我们也需要适合我们的Linux系统镜像，如[**Ubuntu**](https://cn.ubuntu.com/download)、[**deepin**](https://www.deepin.org)、[**ArchLinux**](https://archlinux.org),我们下载需要的系统镜像即可，此次我们为初学者推荐使用**Deepin**进行入门使用,该发行版有较好的本地化服务，和适合普通用户的应用商店。有使用经验的用户可以使用如**Ubuntu**、**ArchLinux**、**Debian**等**Linux**发行版。

---

#  **初识GNU/Linux、Linux内核**

&ensp;&ensp;&ensp;&ensp;**Linux**（/ˈlɪnəks/ LIN-əks）是一种自由和开放源码的类**UNIX**操作系统。该操作系统的内核由林纳斯·托瓦兹在1991年10月5日首次发布，任何个人和机构都可以自由地使用Linux的所有底层源代码，也可以自由地修改和再发布。在加上用户空间的应用程序之后，成为**Linux**操作系统。**Linux**也是自由软件和开放源代码软件发展中最著名的例子。
&ensp;&ensp;&ensp;&ensp;在我们日常中人们都有认为**Linux**发行版并不是主流使用的，其实**GNU/Linux**一直都在影响着我们的生活的方方面面，例如我们专业的网站服务器、大型数据中心、使用**Linux**内核的路由器、嵌入式设备、以及部分国家的国防系统、数学专业领域、科研单位都在使用**Linux**，国内科技公司也合作推出[统信UOS](https://www.chinauos.com/)，**Linux**于1991年开始项目，至今它见证了互联网发展变迁史，它的发展其中不可或缺的来自全世界开发者无私的贡献代码，这也是**Linux**成长的原因，其高效的运行效率以及内存占用就不再赘述，我们直接进入正题，让大家开始学习尝试使用**Linux**发行版。
&ensp;&ensp;&ensp;&ensp;想了解更多可以访问以下网站或其他百科。

[GNU/Linux发行版——自由软件基金会（FSF）](https://www.gnu.org/distros/distros.zh-cn.html)
[ArchLinux—— 一个GNU/Linux的发行版](https://archlinux.org)
[GNU/Linux——维基百科](https://zh.wikipedia.org/wiki/Linux)
[Linux Kernel——维基百科](https://zh.wikipedia.org/wiki/Linux%E5%86%85%E6%A0%B8)
[GNU/Linux————百度百科](https://baike.baidu.com/item/Linux/27050)

---

# **使用Oracle VM VirtualBox安装虚拟机系统**
点击进入[Oracle VM VirtualBox官方网站](https://www.virtualbox.org/)下载

## **打开程序主页面**
![程序主界面](https://i.loli.net/2021/05/09/igI6Y9sEoNJfGdP.png)
**<center>程序主页面</center>**

## **开始新建虚拟机**
![点击 控制→新建](https://i.loli.net/2021/05/09/pUthEJYx7s1BVNQ.png)
**<center>点击 控制→新建</center>**

![](https://i.loli.net/2021/05/10/DtyaSdmAe6k1gYj.png)
**<center>新建虚拟机</center>**
&ensp;&ensp;&ensp;&ensp;填写 系统名称（可以随意填写，无固定要求。）、文件夹（即为存放此虚拟电脑的磁盘位置，建议放在空间较大的位置。）、类型选择Linux（如您要新建Windows则选择Windows。）、版本（如版本选单内没有您使用的Linux发行版则可以选择Linux内核版本，这里我们选择Linux2.6/3.xgi/4.x(64-bit)）、内存大小（根据您实体计算机的内存大小和剩余程度以及个人需求进行分配。例如32GB内存则可以分配16GB内存给虚拟机，16GB内存可以分配8GB内存给虚拟机。）

## **创建虚拟磁盘**
![](https://i.loli.net/2021/05/10/srLSUtj2F7cWhJg.png)
**<center>创建虚拟磁盘</center>**
&ensp;&ensp;&ensp;&ensp;创建虚拟硬盘。（步骤：**虚拟硬盘文件类型选择默认的即可** → **勾选上动态分配磁盘空间** → **现在创建虚拟硬盘** → **创建**）
## **选择虚拟镜像**
![](https://i.loli.net/2021/06/20/F3aYsSvunODeZCN.png)
**<center>返回主界面</center>**
&emsp;&emsp;点击创建后回到主界面，点击启动按钮。

![](https://i.loli.net/2021/06/20/dHqi219xCvShkXt.png)
**<center>启动界面</center>**
&emsp;&emsp;因为没有给虚拟机用的启动盘，所以无法进行启动。点击取消进入下一步。

![](https://i.loli.net/2021/06/20/b5dUAlsEcqFCIPu.png)
**<center>选择虚拟盘</center>**
&emsp;&emsp;选择虚拟盘。（步骤：点击 **设备** → **分配光驱** → **选择虚拟盘** → **进入窗口目录选择你所下载保存的系统镜像文件确认**）

![](https://i.loli.net/2021/06/20/UXOumyrFbxHtEeZ.png)
**<center>选择虚拟盘</center>**
![](https://i.loli.net/2021/06/20/KYlnsz82uUw71TN.png)
**<center>重新启动虚拟机</center>**
&emsp;&emsp;选择上一步添加的虚拟盘后，点击 **控制** → **重启** 进行重启虚拟机。

## **开始安装系统**
![](https://i.loli.net/2021/06/20/mNX1lDFVoSa73kL.png)
**<center>开始安装系统</center>**
![](https://i.loli.net/2021/06/20/QIBzUpvhXFe5Pxy.png)
**<center>选择后正在加载中</center>**
&emsp;&emsp;在重启虚拟机后会读取上一步添加的系统镜像，进入系统安装界面。安装**deepin**直接选择第一个选项即可，如需了解其他deepin安装选项的功能可以访问**deepin**社区、官网了解更多。（如您需要安装其他系统则按照其对应的安装方法步骤进行安装。）

![](https://i.loli.net/2021/06/20/rA75HMzsW34Eaih.png)
**<center>加载完成后进入图形安装界面</center>**
&emsp;&emsp;在加载完成后进入图形安装界面，按照常规进行选择语言。

![](https://i.loli.net/2021/06/20/4GUih6gcpVFNIo3.png)
![](https://i.loli.net/2021/06/20/SswVIL8pkvhZdB7.png)
**<center>硬盘分区</center>**
&emsp;&emsp;无论是虚拟机下还是实机安装，普通用户无特殊需求选择全盘按照即可，至于全盘加密则可选可不选，一般无需选择。选择完毕后点击下一步。

![](https://i.loli.net/2021/06/20/L8Fup5bEBJXPWAh.png)
**<center>准备安装</center>**
&emsp;&emsp;确认无误后点击继续安装。

![](https://i.loli.net/2021/06/20/QqjSN8zlgG3DLYM.png)
**<center>正在安装</center>**
&emsp;&emsp;安装中，耐心等待，安装速度均取决您设备的运算、存储IO等性能。

![](https://i.loli.net/2021/06/20/W3YlibCGgwPD5p8.png)
**<center>安装成功</center>**

![](https://i.loli.net/2021/06/20/7I165nNqEYmAvPu.png)
**<center>移除虚拟盘</center>**

![](https://i.loli.net/2021/06/20/HWgcBtsiMOrTUDQ.png)
**<center>重启虚拟机</center>**

![](https://i.loli.net/2021/06/20/WZqKtwf9cB7MuHn.png)
**<center>选择第一个进入即可</center>**
&emsp;&emsp;在安装成功后，移除虚拟盘，并且重启虚拟机。重启虚拟机后选择第一个即可正常进入系统。

## **系统开机向导**
![](https://i.loli.net/2021/06/20/NwCfWojzUQ8DvR6.png)
**<center>选择语言</center>**

![](https://i.loli.net/2021/06/20/pIribymcv8V4GSZ.png)
**<center>创建账户</center>**

![](https://i.loli.net/2021/06/20/NapDYhVbLesqWOr.png)
**<center>优化系统配置中</center>**
&emsp;&emsp;简单常规的图形化界面选择语言、时区、键盘布局、创建账户。全部设置完后耐心等待加载。（创建账户这里需要注意，**Linux**下用户名也就是电脑的用户名称，我们会经常用到，并且这个密码为**root**用户密码也是在使用sudo调用**root**权限时必须的条件。**root**权限也是**Linux**下经常使用的，同时功能强大也同样危险，请保管并牢记好**root**密码。）

![](https://i.loli.net/2021/06/20/DnYW1mkzj7O65Nx.png)
**<center>用户登录界面</center>**

![](https://i.loli.net/2021/06/20/QLKBeCSuTxaAyHN.png)
**<center>检查到为虚拟机启动的友情提示</center>**
![](https://i.loli.net/2021/06/21/uJP5NpoYVrdCLwM.png)
**<center>桌面样式选择</center>**
&emsp;&emsp;加载完毕后进入账户登陆界面，输入上一步骤设置的密码进行登录系统。虚拟机运行会出现提示，低配置电脑选择普通模式即可。

# **系统界面展示**

## **桌面样式**
![](https://i.loli.net/2021/06/20/Y8kz3IVHTWBJKoD.png)
**<center>Deepin dde界面</center>**
## **系统设置**
![](https://i.loli.net/2021/06/21/Dqr3mHRzXiTsjhY.png)
**<center>Deepin 系统设置</center>**

## **Deepin应用商店**
![](https://i.loli.net/2021/06/21/T3bueIjSGzHRp9Z.png)
**<center>Deepin 应用商店</center>**
&emsp;&emsp;**Deepin**为普通用户可以更加方便的入门使用该系统而制作了应用商店，其中不乏大众用户日常使用的微信、QQ、WPS、钉钉、PS等应用（部分应用由[Wine](https://www.winehq.org/)提供支持。）

## **Deepin 终端**
![](https://i.loli.net/2021/06/21/9egXdRGU4WtF7NQ.png)
**<center>终端执行更新软件包</center>**
![](https://i.loli.net/2021/06/21/VLCwekNcFx6Ws19.png)
**<center>终端安装Vim编辑器</center>**
![](https://i.loli.net/2021/06/21/c2tp1T5Il3Rmgyr.jpg)
**<center>自带的终端主题</center>**
&emsp;&emsp;类**Unix**系统下常用的命令行终端可以说是它的灵魂所在，**Deepin**的终端自带多个主题可供选择。

---
# **后记**

&emsp;&emsp;当代职场上不乏要求员工需要会使用**GNU/Linux**的公司，当然即使我们以后不从事相关工作也可以学习**GNU/Linux**，在系统出现故障时会直观的告诉你出现了什么错误，你可以去尝试解决，在安装你所需要的软件时有安全的包管理器直接从镜像源进行拉取安装，免去了下载的烦恼以及类似Windows下安装软件带来的各种捆绑，开发人员在使用**GNU/Linux**时可以非常方便的下载配置所有所需的环境、组件等。**GNU/Linux**发行版不只是通常映像中的只有黑底白字的终端或者只存在与黑乎乎的服务器机房里，它也可以作为普通用户日常使用，也有比其他系统更漂亮漂亮的桌面，也有丰富的图形GUI程序，其也更开放安全。
&emsp;&emsp;即使你是普通用户，也可以去学习如何使用**GNU/Linux**。

---
本文部分内容引用自以下文章。
[GNU/Linux发行版——自由软件基金会（FSF）](https://www.gnu.org/distros/distros.zh-cn.html)
[ArchLinux—— 一个GNU/Linux的发行版](https://archlinux.org)
[GNU/Linux——维基百科](https://zh.wikipedia.org/wiki/Linux)
[Linux Kernel——维基百科](https://zh.wikipedia.org/wiki/Linux%E5%86%85%E6%A0%B8)
[GNU/Linux————百度百科](https://baike.baidu.com/item/Linux/27050)
