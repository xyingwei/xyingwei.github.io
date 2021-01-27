---
title: Hexo相关指令
date: 2020-12-23
categories: HexoBlog
tags: Hexo
cover: https://w.wallhaven.cc/full/ym/wallhaven-ym95z7.png
---

## 新建一篇文章
    hexo new "文章名称"
## 启动服务器。默认情况下，访问网址为： http://localhost:4000/。
    hexo s
## 部署
+ 清除缓存文件 (db.json) 和已生成的静态文件 (public)。
    hexo clean
+ 生成静态文件。
    hexo g
+ 部署网站。部署之前预先生成静态文件，执行第二步 hexo g
    hexo d