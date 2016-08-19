---
title: hexo使用七牛作为文件存储
date: 2016-08-19 09:51:30
tags: [hexo,qiniu]
keywords: hexo
comments: true
categories: hexo
---

### 注册七牛账号
进入 [七牛](https://portal.qiniu.com/signup?code=3ldwahs7n653m) 官网注册账号


### 安装hexo七牛插件

插件地址：[点击](https://github.com/gyk001/hexo-qiniu-sync)

文档说明比较全，按照README.md文件一步一步安装、配置即可

### 本地上传图片
hexo qiniu sync	
*同步本地图片到七牛*

hexo qiniu sync2	
*增加同步上传那些本地与七牛空间有差异的文件*

### 在md文件中使用图片
\{ % qnimg test/demo.png title:图片标题 alt:图片说明 'class:class1 class2'  % \}
其中是qnimg是七牛插件定义的标签


***

附上是我的配置

{% qnimg blog/hexo-qiniu-config.png title:七牛插件配置 alt:七牛插件配置 %}
