---
layout: post
title: webpack 学习笔记
---

# webpack学习笔记--less-loader

### 先说结果：less-loader需要先安装less `npm install less --save-dev`.

昨天晚上尝试使用webpack提供的众多loaders中的less-loader,然而过程却是相当的曲折。现记录如下：
 
 一开始按照webpack文档提供的[文档](https://webpack.js.org/loaders/less-loader/)安装less-loader，修改webpack.config.js等。一顿操作之后，执行 `webpack` 控制台却提示`module build failed: error: cannot find module 'less'`，一脸懵逼，赶紧就是一顿百度，google。这里真的得吐槽一下百度，基本上你想要的他都没有……

