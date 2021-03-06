---
title: Tensorflow学习指南--安装配置篇(windows-cpu)
date: 2017-09-29 15:41:26
tags: [Tensorflow,技术笔记]
toc: true
---
# 安装指南

## 1.前言

本文的主要内容为如何在Windows环境下安装配置cpu版的Tensorflow供初心者体验并尝试，文章内包含大量的图片(多图烧流量)，另外除了windows-cpu外还有windows-gpu，Ubuntu16.04-cpu,Ubuntu16.04-gpu三个版本，请根据自身需求自行取用。

Tips:个人而言比起windows我更推荐使用ubuntu系统

<!-- more -->

## 2.准备工作

由于一些众所周知的原因，身处国内的我们下载国外的资源会比较困难，不是下载不了就是下载速度慢，在这里我先贴出安装前我们要准备的内容。

- Anaconda 5.1([官网](https://www.anaconda.com/download/#windows) | [百度云](https://pan.baidu.com/s/15DkD9Ommh1TKumCcWUNdLw) (密码:fsb2))

Tips：请根据自己电脑的版本选择下载32或64位安装程序，百度云盘中的安装程序为Anaconda官网源程序，如有需要可以用md5验证真伪

### 2.1 Anaconda安装指南

在下载好Anaconda后我们就可以开始安装了，整体的安装过程没什么特别的，和我们安装其他软件的流程一样可以一路Next过去，值得注意的是**请勿必记住自己安装Anaconda的位置**

以下为我安装过程中的贴图：

Anaconda-install-1

![Anaconda-install-1](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/45960978.jpg)

Anaconda-install-2

![Anaconda-install-2](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/6924894.jpg)

Anaconda-install-3

![Anaconda-install-3](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/26761751.jpg)

Anaconda-install-4

![Anaconda-install-4](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/37590487.jpg)

Anaconda-install-5

![Anaconda-install-5](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/34334942.jpg)

Tips：这里的1其实是可以不点的，它主要的作用是将Anaconda添加到你的环境变量中，如果你以后更改了Anaconda位置，bash中使用Anaconda命令可能会失效(需要手动修改环境变量)

Anaconda-install-6

![Anaconda-install-6](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/51414653.jpg)

Anaconda-install-7

![Anaconda-install-7](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/35164873.jpg)

Anaconda-install-8

![Anaconda-install-8](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/20099441.jpg)

Tpis : 如果已经安装过vscode或者vscode安装失败也没关系，直接下一步就好，之后可以去微软官网下载vscode安装包

Anaconda-install-9

![Anaconda-install-9](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/67023783.jpg)

## 3.安装Tensorflow

由于安装的是CPU版的Tensorflow，整体上来说没什么坑点，只要保持网络通常即可。

Tpis：以下内容虽然分了章节，但其实是连续操作，**请勿关闭操作界面**

### 3.1 为Tensorflow配置独立环境

为什么在安装Tensorflow之前我们要先安装Anaconda呢？这主要是想为Tensorflow配置一个隔离的环境，目前python的版本非常多，各种辅助计算与富含多种功能的库也很多，其中不同的库可能会依赖于不同版本的python，不同的python库也有可能会互相影响(极个别情况)。所以推荐为Tensorflow配置一个独属于自己的环境。

在这里我们推荐使用Python3.5作为Python的基础版本，相对于3.6版本，这个版本的机器学习库更多一些，适应性也相对好一点。

TensorFlow-setting-1

![TensorFlow-setting-1](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/87298029.jpg)

AnacondaUi启动的时间比较长，可能需要等一会

![waiting](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/83024932.jpg)

TensorFlow-setting-2

![TensorFlow-setting-2](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/89943739.jpg)

TensorFlow-setting-3

![TensorFlow-setting-2](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/6830634.jpg)

TensorFlow-setting-4

![TensorFlow-setting-4](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/61235229.jpg)

TensorFlow-setting-5

![TensorFlow-install-5](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/99216583.jpg)

TensorFlow-setting-6

![TensorFlow-install-6](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/95243812.jpg)

### 3.2 正式安装Tensorflow

接下来就是在我们创建的环境中进行安装了，打开Anaconda Navigator，找到Environment中的Tensorflow，点击Open Terminal后输入以下命令(如果因为网络问题失败，请重新输入相同命令)

```bash

pip install tensorflow

```

TensorFlow-install-1

![TensorFlow-install-1](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/95758287.jpg)

TensorFlow-install-2

![TensorFlow-install-2](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/50310869.jpg)

Tpis: 前面括号内的名称代表你当前所在环境的名称

TensorFlow-install-3

![TensorFlow-install-3](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/34712426.jpg)

TensorFlow-install-4

![TensorFlow-install-4](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/17675344.jpg)

TensorFlow-install-error

![error](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/81569950.jpg)

Tpis：如果失败原因是time out的话请重新输入pip install tensorflow(其他原因可复制错误原因百度以下，有可能是pip被锁住了)

### 3.3 验证Tensorflow环境

在安装完Tensorflow后，我们还需要验证下Tensorflow是否安装成功，在刚才打开的Terminal中输入python，并输入以下代码，如果看到Hello, TensorFlow!输出则证明安装成功，如果是no moudle的话请检查是否安装错误

```bash
python
```

![TensorFlow-check-1](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/94025000.jpg)

接下来在python中输入下列代码

```python
import tensorflow as tf
hello = tf.constant('Hello, TensorFlow!')
sess = tf.Session()
print(sess.run(hello))
```

![TensorFlow-check-2](http://ox0sjjwt5.bkt.clouddn.com/18-3-11/26151015.jpg)
