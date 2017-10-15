---
layout:     post
title:      Java Web的一点总结
subtitle:    "\"一点总结\""
date:       2017-10-15
author:     CX
header-img: img/2017-10-15.jpg
catalog: true
tags:
    - javaWeb
---

# 关于web开发一点的总结

## 所用的技术：

Jfinal，jQuery

## 一些值得注意的地方：

### 关于jQuery Ajax：

​     1.分两种工作方式，**同步异步**，这两种工作方式适合不同的场景。

​     2.在静态标记语言HTML下，能够利用好Ajax就能充分与服务器交互。

​     3.在表单提交的时候，在Controller中，或者说Servlet中，应有相应的参数来get到值，否则会抛出异常。简而言之，post多少数据，后台就得get到多少数据。

​     4.前端利用好chorme来调试JS，和前端代码，JS的位置有点重要，ORZ，HTML引用包的位置也很重用。

### 关于jfinal：

​      1.jfianl大法好，感觉用了这个框架以后，都不想用其它的了。

​      2.网页可以用隐藏表单来存储相应的值，最后再交给后台来处理，这个是实现决策树和用户交互的关键，我的十一假期...

​      3.session只存在服务器中，用jQuery session 来操作，网页中是获取不到的，想用session来实现用户访问限制，jfinal貌似给了拦截器的封装，能用，但是对后缀为.html或者.jsp的网页怎么办呢？百度到了一个解决方案，可以在每个的网页头加上session验证，可以在后台写一个方法，来get到session值，使用Ajax大法，写一个JS进行验证。

## 写在最后的话：

​    正文未完待续，说点以下闲话：

​     一个坑接着一个坑。不填坑，不成神。

​    
