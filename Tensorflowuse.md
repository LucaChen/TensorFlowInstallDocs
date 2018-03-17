---
title: Tensorflow学习指南--基础使用篇(vscode or pycharm)
date: 2017-09-29 15:41:26
tags: [Tensorflow,技术笔记]
toc: true
---
# 安装指南

## 1.前言

之前曾经写过几篇Tensorflow环境安装的指南，由于不是直接安装在全局python或者是base环境，所以很多小伙伴不清楚如何使用我们安装好的环境，所以今天来介绍下如何使用Anaconda创建出来的虚拟环境。

这次我们将介绍下Visual Studio Code 和 PyCharm这两个常用IDE的配置方法。

（本文仍旧多图烧流量）

<!-- more -->

## 2.准备工作

在开始本章节之前，请确认自己使用的是 Anaconda 或 Virtualenv 配置的环境

- Anaconda 或 Virtualenv

- Tensorflow CPU 或 GPU

- Visual Studio Code 或 PyCharm

## 3.Visual Studio Code IDE配置

Visual Studio Code是一个轻量级但是十分强大的源代码编辑器，它在Windows, OS X 和Linux操作系统的桌面上均可运行。Visual Studio Code内置了对JavaScript, TypeScript和Node.js语言的支持，并且为其他语言如C++, C#, Python, PHP等提供了丰富的扩展库和运行配置。

### 3.1 创建项目

在开始使用前我们需要创建一个项目，在vscode中我们把每个文件夹当做一个项目，所以我们只需要新建一个文件夹打开他即可

![TensorFlow-use-vscode-1](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/66024570.jpg)

![TensorFlow-use-vscode-1](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/43159967.jpg)

![TensorFlow-use-vscode-1](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/61921963.jpg)

![TensorFlow-use-vscode-1](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/26429425.jpg)

### 3.2 创建新的python文件

Visual Studio Code创建文件的方式也非常的简单，右键->新建文件即可，如果是python文件的话就是用.py作为后缀，如果是nodejs的话就是用.js作为后缀。所以在这里我们使用hello.py当做文件名称。

![TensorFlow-creat-vscode-1](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/7657680.jpg)

![TensorFlow-creat-vscode-2](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/43335413.jpg)



### 3.3 安装Python插件

Visual Studio Code是一个非常强大的源代码编辑器，但是他并不会直接把所有功能都塞给你，你需要在他的插件页面安装你需要的模组。为了能够正常的运行python，我们需要为自己的vscode安装python运行插件。(安好后别忘了重新加载)

![TensorFlow-plugin-vscode-1](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/20211622.jpg)

![TensorFlow-plugin-vscode-2](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/21222257.jpg)

### 3.4 运行python代码

对于一个vscode项目来说，运行时需要一个launch.json，万幸的是这个文件其实不需要我们手动创建，我们只需要按下运行的快捷键F5，点击你想要运行的环境，他会自动帮你生成launch.json。

当然在创建完后，你还需要回到代码界面再次按下F5

![TensorFlow-use-vscode-1](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/2282759.jpg)

![TensorFlow-use-vscode-2](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/7365214.jpg)

![TensorFlow-use-vscode-3](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/86731075.jpg)

![TensorFlow-use-vscode-4](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/5933135.jpg)

### 3.5 配置Anaconda中的Tensorflow环境

在上一步中我们为vscode配置了基础的Python环境，那让我们试下运行TensorFlow代码。你会发现他说找不到我们的TensorFlow模块。这是因为我们并不是在windows或ubuntu全局安装的TensorFlow。

![TensorFlow-tensorflow-vscode-1](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/20961516.jpg)

如果我们想要使用之前配置起来的Anaconda环境要怎么办呢？我们需要在launch.json中添加新的配置。当然在这之前你需要找到自己安装Anaconda的位置。

![TensorFlow-tensorflow-vscode-2](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/8910099.jpg)

点开launch.json后我们可以通过添加配置按钮添加一个新的python启动配置，为了能够使用Anaconda的Tensorflow我们需要把External Terminal/Console(我改名成Tensorflow了)的pythonPath改成Anaconda下虚拟环境的python位置。

![TensorFlow-tensorflow-vscode-3](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/98803050.jpg)

![TensorFlow-tensorflow-vscode-4](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/16338943.jpg)

最后回到我们的Tensorflow代码，点击Debug按钮，选择新环境Tensorflow后重新运行，顺利的输出了Hello Tensorflow

![TensorFlow-tensorflow-vscode-5](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/13432192.jpg)

## 4.PyCharm配置

PyCharm的配置就比较简单了，创建项目的时候直接选择相关的虚拟环境即可。(关于PyCharm购买的问题，广大学生党其实不用担心，JetBrain有学生认证的，用自己学校的邮箱认证即可)

### 4.1 创建PyCharm项目

打开PyCharm后，点击创建Project后会有相关的引导，只需要根据PyCharm的提示一步步来就可以啦，在创建项目的过程中我们就可以配置自己使用什么虚拟环境(Interpreter).

![TensorFlow-use-PyCharm-1](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/64954106.jpg)

![TensorFlow-use-PyCharm-2](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/92568155.jpg)

![TensorFlow-use-PyCharm-3](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/43656801.jpg)

![TensorFlow-use-PyCharm-4](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/59598204.jpg)

![TensorFlow-use-PyCharm-5](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/35241761.jpg)

![TensorFlow-use-PyCharm-6](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/72497861.jpg)

![TensorFlow-use-PyCharm-7](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/61604618.jpg)

### 4.2 创建python文件

由于PyCharm本身就是针对Python而开发的IDE，所以我们不需要配置相关的插件也不需要自己命名编辑器，我们只需要常规的邮件创建文件操作即可。

![TensorFlow-use-PyCharm-8](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/11657507.jpg)

### 4.3 运行Tensorflow代码

在PyCharm中如果有要运行一个Python代码的话直接点击右上角的运行是不能运行的，因为PyCharm启动的时候需要规定启动文件，所以初次运行的时候需要在要运行的python文件右键->Run <'you file name'>.如果你之前有配置过相关的虚拟环境，你就能看到‘Hello，Tensorflow！’啦

![TensorFlow-use-PyCharm-9](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/32400351.jpg)

![TensorFlow-use-PyCharm-10](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/22426145.jpg)
