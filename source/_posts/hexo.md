---
title: Hexo
categories: Hexo
tags: hexo
--- 

## 简介

 [Hexo](https://hexo.io/)
 [Doc](https://hexo.io/docs/) 
 [GitHub](https://github.com/hexojs/hexo/issues)

### 安装Hexo

``` bash
$ npm install -g hexo-cli
# git 推送服务
$ npm install hexo-deployer-git --save
```

### 创建工程

``` bash
$ hexo init "my_blog"
```

### 配置git仓库

修改_config.yml

``` yaml
# Deployment
## Docs: https://hexo.io/docs/one-command-deployment
deploy:
  type: git
  repo: https://github.com/yj12138/yj12138.github.io.git
  branch: master
```

### 创建新页面

``` bash
$ hexo new [layout] "new_page"
```

More info: [Writing](https://hexo.io/docs/writing.html)

### 启动服务

``` bash
$ hexo server
```

More info: [Server](https://hexo.io/docs/server.html)

### 生成静态网站

``` bash
$ hexo generate
```

More info: [Generating](https://hexo.io/docs/generating.html)

### 布署网站

``` bash
$ hexo deploy
```

More info: [Deployment](https://hexo.io/docs/one-command-deployment.html)
