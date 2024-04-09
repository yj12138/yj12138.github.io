---
title: 常用命令
categories: Linux
tags: command
---

# 创建用户
    useradd -m username
    -m 创建用户目录
# 设置密码
    passwd username


# 服务
<!-- 查看服务 -->
service --status-all
    

# 设置时区
    tzselect
    ->Asia
    ->China
    ->BeiJing
    ->Yes
    sudo cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime
    date -R