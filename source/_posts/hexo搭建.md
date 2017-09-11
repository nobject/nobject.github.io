---
title: hexo 搭建
date: 2017-09-08 09:24:18
tags: hexo
---
### 搭建准备
1. nodejs安装
hexo是基于nodejs的一个博客框架，因此首先得安装nodejs。[Nodejs安装文件下载](http://nodejs.cn/download/)

2. git安装
我们在github上搭建github pages，需要git的支持。[git下载地址](https://git-scm.com/downloads)


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
### 部署git
编辑blog目录下的_config.yml的deploy选项

```bash
deploy:
  type: git
  repo: git@github.com:nobject/nobject.github.io.git
  branch: master
```
安装部署git插件：

```bash
npm install hexo-deployer-git --save
```
发布至git

```bash
hexo g //生成文件  hexo generate的简写
hexo d //部署至git hexo deploy  的简写
```

