---
layout: post
title: JavaScript-数据类型-boolean
---

# JavaScript数据类型之布尔类型

Boolean类型是ECMAScript五种简单数据类型（Undefined，Null，Boolean，Number，String）之一。

Boolean类型只有两个字面值：true和false。需要注意的是，这两个值是区分大小写的，诸如True和False等都只是标识符而非Boolean值。

虽然Boolean类型只有两个字面值，但ECMAScript中每个其他类型的值都可以转换为Boolean类型的值。要实现转换，可以使用转型函数`Boolean()`，例如：

```javascript
var message = 'Hello World!';
var messageAsBoolean = Boolean(message);
```

以下是一份各种数据类型对应的转换规则：


| 数据类型|转换为true的值|转换为false的值|
|-------|---------|---------|
|Boolean|true|false|
|String|任何非空字符串|''（空字符串）|
|Number|任何非零数字值（包括无穷大）|0和NaN|
|Object|任何对象|null|
|Undefined|*不适用*|undefined

今天的总结就到这里吧，以上。

*注：以上内容摘录或节选自《JavaScript高级程序设计（第3版）》page：26-27*

[返回](https://www.icenzhao.com/)