---
title: hexo 搭建
date: 2017-09-08 09:24:18
tags: hexo
---
### 搭建准备
1. nodejs安装
hexo是基于nodejs的一个博客框架，因此首先得安装nodejs.[Nodejs安装文件下载](http://nodejs.cn/download/)

2. git安装
我们在github上搭建github pages，需要git的支持

3. hexo安装
``` bash
npm install hexo-cli -g
```

### 创建博客
1. 进入需要创建博客的目录，创建blog目录
``` bash
hexo init blog
```
2. 进入blog目录，使用npm来安装依赖
``` bash
cd blog
npm install
```
3. 安装完毕，启动服务器
``` bash
hexo server
```
