---
layout:      post
title:       sketch自动存储占用大容量解决办法
summary:     前几天发现硬盘空间越来越小，之前在知乎上阅读过一篇介绍关于sketch3.x版本自动备份，导致占用大量存储的问题…
date:        2015-6-09 14:41:00
keywords:    sketch,经验总结
categories:  tools
tags:        tools
group:       archive
---

前几天发现硬盘空间越来越小，之前在知乎上阅读过一篇介绍关于sketch3.x版本自动备份，导致占用大量存储的问题，于是查看了下，结果发现有14G的自动备份，我的SSD只有500G，空间宝贵啊！

废话不多说，赶紧操作：

1. 打开终端输入 cd / 然后回车
2. 输入ls -la然后回车
3. 输入sudo du -sh .DocumentRevisions-V100然后回车
4. 输入你mac的登录密码回车查看这个缓存文件多大
5. 看好了，在确保没有sketch文件打开的情况下输入删除命令:

> sudo rm -rf .DocumentRevisions-V100 然后回车

搞定！
