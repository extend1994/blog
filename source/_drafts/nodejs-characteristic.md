---
title: nodejs-characteristic
tags:
  - nodejs
  - JavaScript
  - note
  - learning
  - characteristic
thumbnail: https://upload.cc/i1/2018/06/01/qk6uAR.png
---

## Node.js 簡介

### Module & Common.js
可以想像成 JavaScript library，有數個 function 可以供開發者使用。
可分為 Built-in Modules 和 external modules

為了讓Javascript擁有更多功能及擴展實用領域，其中定義了一系列的架構和API，包括模組機制、系統、I/O、後端應用...等，讓所有的框架和各種函式庫可以有遵循的規範標準

### Module 使用方式 (Inlcude and Create)
```js
/*** Create a module
exports.<extenal_ref> = function () {}

module.exports = {
  <external_ref>: <internal_function/variable_name>
  ...
}
*/
exports.my_module = function () { console.log("Hello, my module!"); }

/*** Include a module:
var <module_ref> = require('<module_name>');
*/

var http = require('http');
var my_module = require('/path/to/my_module');
```

## Node.js 特性與開發

### Asynchronous I/O 非同步輸入/輸出
> NO waiting, just handle the things come

### Non-blocking

### Event-driven & call back function

### Single Thread & Child Process
NO deadlock

## 參考資料
https://blog.toright.com/posts/4167/%E4%B8%80%E5%80%8B%E6%89%93%E5%8D%81%E5%80%8B%EF%BC%8C%E7%82%BA%E4%BB%80%E9%BA%BC-nodejs-%E6%AF%94%E8%BC%83%E5%BF%AB%EF%BC%9F.html
