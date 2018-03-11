---
author: "zhuangsheng"
date: 2018-03-11
title: "Linux Tools"
tags: [
    "linux",
    "tool",
]
categories: [
    "linux",
    "tool",
]
---

### 1. autojump
它的主要作用是记录常用目录,实现快速跳转,如`cd /var/www/html/`,只需输入`j h`即可实现跳转
安装:
    git下载[autojump](https://github.com/joelthelion/autojump)
    ```bash
    git clone git@github.com:joelthelion/autojump.git
    cd autojump
    python install.py
    ```
    安装完后,再在`~/.bashrc`加入下面一行
    `[[-s /root/.autojump/etc/profile.d/autojump.sh]] && source /root/.autojump/etc/profile.d/autojump.sh`
使用:
    j -h查看帮助
    j -a [目录] 加入目录
    j -i [权重] 增加常用目录的权重(在该目录下执行)
    j -d [权重] 减少权重
    j -s 查看变化
    j --purge　显示数据库中统计