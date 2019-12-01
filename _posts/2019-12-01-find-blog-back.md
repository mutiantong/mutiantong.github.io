---
layout: post
title: "找回博客"
subtitle: '开始'
author: "沐天同"
header-style: text
tags:
  - 博客搭建
---

## 总归要开始的，那就现在吧！
---

本博客采用 github + [Jekll]( http://jekyllcn.com/ )  



### 搭建本地环境

机器环境： CentOS Linux release 7.7.1908 (Core)

内核：         3.10.0-327.el7.x86_64

按照官方文档很容易就可以快速搭建本地环境

```bash
# 按照 ruby
yum install ruby

# 升级 ruby 2.6
yum install -y gcc-c++ patch readline readline-devel zlib zlib-devel libyaml-devel libffi-devel openssl-devel make bzip2 autoconf automa

curl -L get.rvm.io | bash -s stable

source /etc/profile.d/rvm.sh

rvm install 2.6

gem install jekyll bundler
```



![image-20191201175739340](/img/blog/image-20191201175739340.png)

搭建本地环境时，如果涉及到 Ruby 升级的问题，可以参考 [Linux在线升级ruby]( https://blog.csdn.net/qq_14945847/article/details/77986900 )







本地运行博客并可以让局域网访问

```bash
jekyll serve -w --host=0.0.0.0
```



