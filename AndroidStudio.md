---
title: AndroidStudio安装指南
date: 2017-09-29 15:41:26
tags: [AndrdoidStudio,技术笔记]
toc: true
---
# 安装指南

## 1.前言

AndroidStdio是开发Android APP的IDE。接下来的说明中我们将介绍如何安装AndroidStduio以及JDK的安装
![icon](http://ok33lph8y.bkt.clouddn.com/1.png)

<!-- more -->

## 2.安装Java SDK

开发Android软件所使用的主要语言是java所以在安装AndroidStudio前我们需要先安装用来开发java的工具 java jdk。

首先从我们提供的百度云盘中下载需要用到的jdk-8u161-windows-x64
[百度云盘](https://pan.baidu.com/s/15DkD9Ommh1TKumCcWUNdLw) (密码:fsb2))



### 2.1 JAVA SDK 安装

在下载好JAVA SDK后我们就可以开始安装了，整体的安装过程没什么特别的，和我们安装其他软件的流程一样可以一路Next过去。

以下为我安装过程中的贴图：



![jdk-2](http://ok33lph8y.bkt.clouddn.com/2.png)

双击程序，开始安装

![jdk-3](http://ok33lph8y.bkt.clouddn.com/3.png)

点击下一步，如果有修改地址的话请记住自己的安装地址

![jdk-4](http://ok33lph8y.bkt.clouddn.com/4.png)

![jdk-5](http://ok33lph8y.bkt.clouddn.com/5.png)

在安装的过程中会跳出一个弹窗，直接点击下一步就好

![jdk-6](http://ok33lph8y.bkt.clouddn.com/6.png)

![jdk-7](http://ok33lph8y.bkt.clouddn.com/7.png)

然后我们的安装过程就结束了

![jdk-8](http://ok33lph8y.bkt.clouddn.com/8.png)
### 2.2 配置 JAVA SDK 环境变量

在安装好jdk后我们需要配置我们电脑的环境，打开你安装jdk的文件夹（如果没有修改地址的话应该在C:\Program Files\Java下）

![jdk-9](http://ok33lph8y.bkt.clouddn.com/9.png)

打开jdk文件夹下的bin目录

![jdk-10](http://ok33lph8y.bkt.clouddn.com/10.png)

复制当前文件夹所在位置

![jdk-11](http://ok33lph8y.bkt.clouddn.com/11.png)

打开我的电脑点击标题栏的计算机（win7 请右键我的电脑点击属性->高级系统设置）

![jdk-12](http://ok33lph8y.bkt.clouddn.com/12.png)

然后点击系统属性

![jdk-13](http://ok33lph8y.bkt.clouddn.com/13.png)

点击高级系统设置

![jdk-14](http://ok33lph8y.bkt.clouddn.com/14.png)

点击环境变量设置

![jdk-15](http://ok33lph8y.bkt.clouddn.com/15.png)

双击系统变量中的Path，讲我们刚才复制的地址添加进来

![jdk-16](http://ok33lph8y.bkt.clouddn.com/16.png)

![jdk-17](http://ok33lph8y.bkt.clouddn.com/17.png)

最后打开我们的cmd测试成果（win+R  然后输入cmd）

![jdk-18](http://ok33lph8y.bkt.clouddn.com/18.png)

你会打开一个黑色的窗口，在这里输入java –version，如果配置成果会类似下图的内容

![jdk-19](http://ok33lph8y.bkt.clouddn.com/19.png)

## 3.安装Android Studio

做了这么多，我们终于要进入正片了，Let`t part!（咳咳无耻的盗了个图）是老样子下载百度云盘里面的android-studio-bundle-143.2821654-windows并解压
[百度云](https://pan.baidu.com/s/15DkD9Ommh1TKumCcWUNdLw) (密码:fsb2))

![as-20](http://ok33lph8y.bkt.clouddn.com/20.png)

之后一直点击NEXT，看到下面界面后再next

![as-21](http://ok33lph8y.bkt.clouddn.com/21.png)

接下来就是正常的我同意

![as-22](http://ok33lph8y.bkt.clouddn.com/22.png)

注意全程不能有中文，顺便记下你sdk安装的位置

![as-23](http://ok33lph8y.bkt.clouddn.com/23.png)

之后直接点击install即进入安装界面 ，等待安装完成 

![as-24](http://ok33lph8y.bkt.clouddn.com/24.png)

![as-25](http://ok33lph8y.bkt.clouddn.com/25.png)

之后next就好

![as-26](http://ok33lph8y.bkt.clouddn.com/26.png)


![as-27](http://ok33lph8y.bkt.clouddn.com/27.png)

## 4.下载并安装Android SDK

安装完后你可能会发现为什么自己的AndroidStudio打不开,而且一直卡在初始界面，界面一直在显示Download

这是由于我大天朝自有国情存在，你们都懂得，我们需要通过代理下载sdk

打开我们的sdk安装位置，双击SDK Manager

![as-28](http://ok33lph8y.bkt.clouddn.com/28.png)

回传下下图一样的界面

![as-29](http://ok33lph8y.bkt.clouddn.com/29.png)

然后你可能会发现，他说下载失败，这个时候不要担心~

我们给你们准备好了代理


![as-30](http://ok33lph8y.bkt.clouddn.com/30.png)

输入给你们的代理网址和端口即可，然后点击Close，接下来你们就可以愉快的点击安装和下载

![as-31](http://ok33lph8y.bkt.clouddn.com/31.png)

![as-32](http://ok33lph8y.bkt.clouddn.com/32.png)

## 4.运行自己的第一个Android 程序
是时候试试自己的劳动成果了!

打开刚才打不开的AndroidStudio，选择Start a new Android Studio Project

![as-33](http://ok33lph8y.bkt.clouddn.com/33.png)

确认完图中的内容后就可以点击下一步了，投一次你也可以什么都不修改直接next

![as-34](http://ok33lph8y.bkt.clouddn.com/34.png)

在接下来的这个页面你们可以选择支持的最小sdk，个人推荐是从4.4开始,点击next

![as-35](http://ok33lph8y.bkt.clouddn.com/35.png)

选择开始生成的默认类型，我们选择Empty Activity就好

![as-36](http://ok33lph8y.bkt.clouddn.com/36.png)

确认完图中内容后就可以直接点击确认啦

![as-37](http://ok33lph8y.bkt.clouddn.com/37.png)

在我们刚刚打开一个项目的时候，他需要一段时间进行初始化

![as-38](http://ok33lph8y.bkt.clouddn.com/38.png)

在初始化结束后我们就可以直接点击标题栏的绿色小箭头了

![as-39](http://ok33lph8y.bkt.clouddn.com/39.png)

点击OK你的第一个HelloWord程序就写好啦，我们的Android开发环境就搭建好啦(:зゝ∠)_

![as-40](http://ok33lph8y.bkt.clouddn.com/40.png)





















































































































































































































