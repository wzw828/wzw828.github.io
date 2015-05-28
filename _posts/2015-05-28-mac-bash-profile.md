---
layout:      post
title:       Mac更新.bash_profile文件
summary:     
date:        2015-05-28 13:35:00
keywords:    mac,bash
categories:  software
tags:        software
group:       archive
---

1. 打开terminal(终端)
2. cd  ( 进入当前用户的home目录)
3. open .bash_profile (打开.bash_profile文件，如果文件不存在就  创建文件：touch .bash_profile  编辑文件：open -e bash_profile)
4. 直接更改弹出的.bash_profile文件内容
5. command + s 保存文件，然后关闭
6. 在terminal(终端)中输入 source .bash_profile (使用刚才更新之后的内容)