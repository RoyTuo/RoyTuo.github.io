---
title: Linux系列——	一、初识GNU/Linux、Linux内核
tags:
  - GNU/Linux
categories:
  - GNU/Linux
cover: >-
  https:
top_img: >-
  https:
date: 2021-04-20 00:00:00

---

#  **前言**
&ensp;&ensp;&ensp;&ensp;一般情况我们因为各种原因，日常使用的办公学习电脑都是**Windows**、**MacOS**，并没有接触过**Linux**，这里我们就直接使用虚拟机安装使用**Linux**,这里我们推荐使用[**VirtualBox**](https://www.virtualbox.org)虚拟机软件，下载后我们正常安装即可。有了好的虚拟机软件，我们也需要适合我们的Linux系统镜像，如[**Ubuntu**](https://cn.ubuntu.com/download)、[**deepin**](https://www.deepin.org)、[**ArchLinux**](https://archlinux.org),我们下载需要的系统镜像即可，这边我们为初学者推荐使用**deepin**进行演示,该发行版有较好的本地化服务，和适合普通用户的应用商店。

---

#  **初识GNU/Linux、Linux内核**

&ensp;&ensp;&ensp;&ensp;**Linux**（/ˈlɪnəks/ LIN-əks）是一种自由和开放源码的类**UNIX**操作系统。该操作系统的内核由林纳斯·托瓦兹在1991年10月5日首次发布，任何个人和机构都可以自由地使用Linux的所有底层源代码，也可以自由地修改和再发布。在加上用户空间的应用程序之后，成为**Linux**操作系统。**Linux**也是自由软件和开放源代码软件发展中最著名的例子。
&ensp;&ensp;&ensp;&ensp;在我们日常中人们都有认为**Linux**发行版并不是主流使用的，其实**GNU/Linux**一直都在影响着我们的生活的方方面面，例如我们专业的网站服务器、大型数据中心、使用**Linux**内核的路由器、以及部分国家的国防系统、数学专业领域、科研单位都在使用**Linux**，国内科技公司也合作推出[统信UOS](https://www.chinauos.com/)，**Linux**于1991年开始项目，至今它见证了互联网发展变迁史，也从一个系统内核变成了享誉世界的操作系统，其中来自全世界开发者无私的贡献代码，也是**Linux**成长的原因，其高效的运行效率以及内存占用就不再赘述，我们直接进入正题，让大家提前开始学习尝试使用**Linux**发行版。
&ensp;&ensp;&ensp;&ensp;想了解更多可以访问以下网站或其他百科。

[GNU/Linux发行版——自由软件基金会（FSF）](https://www.gnu.org/distros/distros.zh-cn.html)
[GNU/Linux——wikipeidia](https://zh.wikipedia.org/wiki/Linux)
[Linux Kernel——wikipedia](https://zh.wikipedia.org/wiki/Linux%E5%86%85%E6%A0%B8)
[GNU/Linux————百度百科](https://baike.baidu.com/item/Linux/27050)

---

# **使用VirtualBox安装系统**
点击进入[VirtualBox官方网站](https://www.virtualbox.org/)下载

## **打开VirtualBox的程序主页面**
![VirtualBox程序主界面](https://i.loli.net/2021/05/09/igI6Y9sEoNJfGdP.png)
<center>VirtualBox的程序主页面</center>

## **点击 控制 → 新建 开始新建虚拟机**
![点击 控制→新建](https://i.loli.net/2021/05/09/pUthEJYx7s1BVNQ.png)
<center>点击 控制→新建</center>

## **开始新建虚拟电脑**
![](https://i.loli.net/2021/05/10/DtyaSdmAe6k1gYj.png)
<center>新建虚拟电脑</center>
&ensp;&ensp;&ensp;&ensp;填写 系统名称（可以随意填写，无固定要求。）、文件夹（即为存放此虚拟电脑的磁盘位置，建议放在空间较大的位置。）、类型选择Linux（如您要新建Windows则选择Windows。）、版本（如版本选单内没有您使用的Linux发行版则可以选择Linux内核版本，这里我们选择Linux2.6/3.xgi/4.x(64-bit)）、内存大小（根据您实体计算机的内存大小和剩余程度进行分配，如32GB内存则可以分配16GB内存给虚拟机，16GB内存可以分配8GB内存给虚拟机。）

![](https://i.loli.net/2021/05/10/srLSUtj2F7cWhJg.png)
<center>创建虚拟磁盘</center>
&ensp;&ensp;&ensp;&ensp;创建虚拟硬盘（虚拟硬盘文件类型选择默认的即可 → 勾选上动态分配磁盘空间 → 选择 现在创建虚拟硬盘 → 创建）


&ensp;&ensp;&ensp;&ensp;









[GNU/Linux发行版——自由软件基金会（FSF）](https://www.gnu.org/distros/distros.zh-cn.html)
[GNU/Linux——wikipeidia](https://zh.wikipedia.org/wiki/Linux)
[Linux Kernel——wikipedia](https://zh.wikipedia.org/wiki/Linux%E5%86%85%E6%A0%B8)
[GNU/Linux————百度百科](https://baike.baidu.com/item/Linux/27050)

以上部分内容引用自以上文章