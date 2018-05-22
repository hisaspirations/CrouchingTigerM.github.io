---
layout: post
title: webpack 学习笔记
---

# webpack学习笔记--less-loader

### 先说结果：less-loader需要先安装less `npm install less --save-dev`.

昨天晚上尝试使用webpack提供的众多loaders中的less-loader,然而过程却是相当的曲折。现记录如下：
 
 一开始按照webpack文档提供的[文档](https://webpack.js.org/loaders/less-loader/)安装less-loader，修改webpack.config.js等。一顿操作之后，执行 `webpack` 控制台却提示`module build failed: error: cannot find module 'less'`，一脸懵逼，赶紧就是一顿百度，google。这里真的得吐槽一下百度，基本上你想要的他都没有……
以上面控制台输出内容为关键词Google一下，基本上很快就能推断出解决办法，即安装less，那么为什么安装less-loader的时候没有一并安装less呢？回头仔细刷一下webpack的文档，会发现有这样一句话：`The less-loader requires less as peerDependency. Thus you are able to control the versions accurately.`关键就在这个`peerDependency`上，这里必须夸一下webpack的文档，直接在其文档上点[这个链接](https://docs.npmjs.com/files/package.json#peerdependencies),一切就真相大白了！！！

不想点的同学可以直接看以下摘录：
```NOTE: npm versions 1 and 2 will automatically install peerDependencies if they are not explicitly depended upon higher in the dependency tree. In the next major version of npm (npm@3), this will no longer be the case. You will receive a warning that the peerDependency is not installed instead. ```
