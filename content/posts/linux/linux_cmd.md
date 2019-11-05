+++
categories = ["Linux"]
date = "2019-11-05"
description = "一些Linux常用命令"
tags = ["Linux"]
title = "Linux常用的命令"
url = "/linux/linux_cmd/"
+++

## 用户管理
1. 添加用户
```
useradd fancy
```
2.  添加组
```
groupadd fancy
```
3.  设置密码
```
passwd fancy
echo "xxxxx" | passwd fancy --stdin
```
5. 加入sudo用户
```
sudo echo "%fancy ALL=(ALL) NOPASSWD: ALL" >> /etc/sudoers
```

## 后台运行
1. 
```
nohup ./a.out&
```

## 遍历删除所有文件
1. 
```
find . -name .svn -exec rm -rf {} \;
```
 
## 时间
1. 计算指定时间的时间戳
```
date +%s -d '2015-11-10 01:01:01'
```
2. 时间戳转换为实际时间
```
date -d @1233631748
```
3. 设置系统时间
```
date -s "20091112 18:30:50"
```

## 文件夹大小
1. 
```
du -s ./
du -h --max-depth=1
```

## KILL
1. 查看信号定义
```
kill -l
```
2. 给进程发信号
```
kill -s SIGHUB 进程号
```

## 查看公网ip
1. 
```
curl cip.cc
```

## netstat
1. 
```
netstat -anpt
```
