---
layout: post
title: webpack--清理/dist文件夹
---

# webpack学习笔记--清理/dist文件夹

在学习使用webpack的过程中会碰到[清理/dist文件夹](https://webpack.js.org/guides/output-management/#cleaning-up-the-dist-folder)的内容。因为指导手册之前的内容都是如何在/dist下生成各种文件，导致学习到这一步时，/dist下已经是杂乱一片，所以有这样的诉求。webpack也给出了自己的解决办法，点击前面的链接即可看到。巧合的是昨天在查`NODE_ENV`相关知识点时，偶然发现另一种方法，直接用npm的脚本也能达到同样的效果，即`rm -rf dist && mkdir dist`,具体文章可以移步[这里](https://segmentfault.com/a/1190000005811347)。

webpack的插件是如何实现的暂时没有时间细究，之后有空一定补上。

[返回](https://www.icenzhao.com/)