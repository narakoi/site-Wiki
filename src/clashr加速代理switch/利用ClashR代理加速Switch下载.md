---
layout: post
title: 利用Clash代理加速Switch下载
slug: clashrtoswitch
date: 2020-03-21 23:30
status: publish
author: KOI
categories: 
  - clash
tags:
  - Switch
  - ClashR
excerpt: 优雅的使用Clash
---

## 前言

鉴于现在Switch在线下载游戏的速度实在是太慢，更换dns效果也不是很明显。经过一番折腾，用Clash(R)成功给Switch连上了代理，这里我就简单分享下。

ClashR-PC端：[点我下载](https://github.com/narakuzi/clashr-for-window/releases/download/v1.0/ClashR.for.Windows-1.0-win.7z)

订阅获取：[KoiCloud](https://kois.pw)

### 电脑端配置

1.首先要先获取你的Clash(R)订阅，在Profiler处一键导入到你的Clash(R)客户端。再切换到Proxies界面，选择合适的节点。

![](https://cdn.jsdelivr.net/gh/narakoi/narakoi.github.io@master/archives/assets/500aeb83d30cfa491aea2e0e57df928b.png)

选完节点以后回到General主界面。将Allow LAN和System Proxyz开关打开。

![](https://cdn.jsdelivr.net/gh/narakoi/narakoi.github.io@master/archives/assets/6daf12a451940e583cca0862195057bb.png)

接着鼠标移至Allow LAN处查看本机局域网IP并记下，稍后会用到。

![](https://cdn.jsdelivr.net/gh/narakoi/narakoi.github.io@master/archives/assets/be11e2a2fc7eb7e67bad3006bd70ffdb.png)

### Switch主机配置



1.打开Switch 并在设置里找到互联网，更改当前连接wifi的设置，代理服务器设为启用，服务器ip填写刚刚记住的本机局域网IP，端口一般默认为7890.DNS设置可改可不改，这里推荐阿里的DNS：233.5.5.5 谷歌的：8.8.8.8

![](https://cdn.jsdelivr.net/gh/narakoi/narakoi.github.io@master/archives/assets/7c16196f262011c59d80b2ab04c5894f.jpg)

设置完毕后点击保存，连接到此网络，提示连接成功即可。

![](https://cdn.jsdelivr.net/gh/narakoi/narakoi.github.io@master/archives/assets/5e755623831013a52298e4d47cafbb30.jpg)

来跑下测速把！

![](https://cdn.jsdelivr.net/gh/narakoi/narakoi.github.io@master/archives/assets/af85e876118a0ad3ff8089fb73f29475.jpg)

可以看到下载速度比之前快了不少。

