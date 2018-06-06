---
layout: post
title: JavaScript查漏补缺之判断变量是否数组
---

# JavaScript查漏补缺之判断变量是否数组

昨天面试碰到这个问题，回答的不太好，当时大致的思路如下：
1. 使用`typeof`，但是话说出口马上反应过来`typeof []`得到的是"object"；
2. 使用`instanceof`，面试官说这个倒是可以，但是遇到`iframe`还是会有问题；

当时聊到这里基本就结束了，面试官没再追问。不过其实还有别的方法。

3. ES5中给Array增加了isArray(),可以方便地判断一个变量是否数组，但就当前的浏览器环境而言，还是有部分用户的浏览器不支持ES5。接下来就请出终极大宝剑！登登登：
Object.prototype.toString.call(someVar)
由于[这篇文章](https://blog.csdn.net/a31017799/article/details/70850418)介绍的已经非常清楚，此处不再赘述。

以上。

[返回](./)