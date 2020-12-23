---
title: shoka主题 添加评论功能
date: 2020-12-23
categories: HexoBlog
tags: Hexo
cover: https://w.wallhaven.cc/full/5w/wallhaven-5we787.jpg
---
# shoka主题 添加评论功能
<!-- more -->
## 开启评论配置
    + 安装好 hexo-symbols-count-time 插件后，不需要修改站点配置文件，直接使用插件默认配置就行。
    + 需要修改主题配置文件，找到两处 cout ，修改为 true ：
    ```
    # 页尾全站统计
    footer:
      since: 2010
      count: true

    # 文章界面统计
    post:
      count: true
    ```
## 开启Valine
我们的评论系统其实是放在==Leancloud上==的，因此首先需要去注册一个账号 [点我注册](https:leancloud.cn)
+ 注册完以后需要创建一个应用，名字可以随便起，然后 进入应用->设置->应用key ,获取你的 appid 和 appkey
+ 打开shoka主题配置文件(_config.yml), 搜索 valine，填入==appid== 和 ==appkey==
+ 在Leancloud -> 设置 -> 安全中心 -> Web 安全域名 把你的域名加进去🎉结束撒花～
## 文章关闭评论权限
    如果某一篇文章需要关闭评论功能，则在文章 Front Matter 中配置：
    ```
    ---
    title: 关闭评论
    comment: false
    ---

    ```