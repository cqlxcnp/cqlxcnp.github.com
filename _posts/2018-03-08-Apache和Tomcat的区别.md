---
layout: post
title: Apache和Tomcat的区别
key: 20180308
tags: Apache Tomcat 
---
## 介绍   

1. Apache是web服务器，Tomcat是应用（java）服务器，它只是一个servlet(jsp也翻译成servlet)容器，可以认为是Apache的扩展。
Apache和Tomcat都可以做为独立的web服务器来运行。但是Apache不能解释java程序（jsp,serverlet）
2. Apache是普通服务器，本身只支持html即普通网页。不过可以通过插件支持PHP,还可以与Tomcat连通(单向Apache连接Tomcat,就是说通过Apache可以访问Tomcat资源。反之不然)
3. 两者都是一种容器，只不过发布的东西不同。Apache是html容器，功能像IIS一样，Tomcat是jsp/servlet容器，用于发布JSP及JAVA的，类似的有IBM的webshere、EBA的Weblogic，sun的JRun等
4. Apache和Tomcat是独立的，在通一台服务器上可以集成。


 

## 打个比方
Apache是一辆卡车，上面可以装一些东西如HTML等。但是不能装水，要装水必须要有容器（桶），Tomcat就是一个桶（装像Java这样的水），而这个桶也可以不放在卡车上。