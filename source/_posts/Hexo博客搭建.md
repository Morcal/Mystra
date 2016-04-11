---
title: Hexo博客搭建
date: 2016-04-11 17:06:44
tags: 
- hexo
- github pages
- node.js
- hexo-next 
---
# Hexo 博客搭建
### 下载并安装git
> git:https://git-scm.com/download/

### 安装node.js&npm
> node.js:https://nodejs.org/en/

### npm安装Hexo
```
npm install hexo-cli -g
```
### Setup Hexo
```
hexo init <folder> //如hexo init E:\Hexo Blog
cd <folder>
npm install
```
### 修改全局配置`_config.yml`
包括网站标题、语言、标签、分类等。
### 配置hexo主题
```
$ cd your-hexo-site
$ git clone https://github.com/iissnan/hexo-theme-next themes/next
```
### 启用主题
修改站点下的配置文件：theme: next

### 验证主题
```
hexo clean
hexo s --debug
```
### 配置主题

+ 代码显示高亮：`highlight_theme: night`

+ 添加github page
 >deploy:
 type: git
 repo:
 github: https://github.com/Morcal/Morcal.github.io.git,master
 branch: master  
  
+ 修改头像：avatar: http://7xrfxa.com1.z0.glb.clouddn.com/hexo_logo.png
* Social links

  >social:
  github: https://github.com/Morcal
  简书: http://www.jianshu.com/users/0f0866310203/latest_articles
  douban: http://weibo.com/3029549884
  zhihu: https://www.zhihu.com/people/liu-zhe-yu-11

* 设置阅读全文  

  >auto_excerpt:
  enable: true
  length: 150

* LeanCloud统计
  >leancloud_visitors:
  enable: true
  app_id: MRJYJDbjFrqNNNCusljIyJ4m-gzGzoHsz
  app_key: AFUeslkAn1pq7D21jLs6O4Ll

* 添加背景音乐
 >在博文中任意地方插入网易云音乐外链

### 启动
```
hexo server
```
### 创建github仓库，并设置开启gh-pages功能
* 创建仓库`Morcal.github.io`必须是用户名
* 点击界面右侧的Settings，你将会打开这个库的setting页面，向下拖动，直到看见GitHub Pages，点击Automatic page generator，Github将会自动替你创建出一个gh-pages的页面。那么大约15分钟后yourname.github.io这个网址就可以正常访问


[相关链接](http://www.jianshu.com/p/05289a4bc8b2)





