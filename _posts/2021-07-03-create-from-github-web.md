---
layout: post
title:  "从网页创建的文章"
date:   2021-07-03 08:41:50 +0800
categories: jekyll update
---

## 步骤

1 ssh连接服务器

```bash
sudo -i  #切换到root
passwd   #修改密码
```

2 修改SSH配置文件/etc/ssh/sshd_config

```bash
vi /etc/ssh/sshd_config #编辑文件
```

3 i修改

```bash
PermitRootLogin yes #默认为no，需要开启root用户访问改为yes
PasswordAuthentication yes #默认为no，改为yes开启密码登陆
```

4 保存并退出

```bash
:wq   #保存并退出
```

5 重启服务

```bash
/etc/init.d/ssh restart
```



## 其他Google云相关命令

### 安装基础依赖环境

```bash
yum -y install wget    #ContOS Yum 安装 wget
apt-get install wget   #Debian Ubuntu 安装 wget
```
