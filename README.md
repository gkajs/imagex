<p align="center">
<a href ="https://github.com/gkajs/imagex"><img alt="gka" src="https://user-images.githubusercontent.com/10385585/29361266-603625b0-82b9-11e7-9243-2d0cf405a579.png"></a>
</p>

# imagex

<a href="https://www.npmjs.org/package/imagex"><img src="https://img.shields.io/npm/v/imagex.svg?style=flat"></a>
<a href="https://github.com/joeyguo/imagex#license"><img src="https://img.shields.io/badge/license-MIT-blue.svg"></a>

专注于序列帧图片优化。

使用 imagex 进行图片优化、生成图片信息数据(可用于图片还原)。

![imagex](https://user-images.githubusercontent.com/10385585/29180779-6c97a69a-7e2b-11e7-8763-bd5f721233b0.png)

# Install

```
$ npm i imagex
```

# Usage

```js
var imagex = require("imagex");

imagex({
    src       : "/pictures/src",  // 图片文件夹地址
    dest      : "/pictures/dest", // 输出文件夹地址
    prefix    : "prefix-",        // 重命名前缀
    isMini    : true,             // 压缩
    isCrop    : true,             // 空白裁剪
    isUnique  : true,             // 去重
    isSprites : true,             // 合图
    algorithm : "left-right",     // 合图布局模式 默认 binary-tree，可选 top-down | left-right..
    spritesCount: 2               // 生成多合图，指定几张图片合成一张合图，可选
}, function(data){
    console.log(data);            // 图片信息数据
}
```


# Welcome

* 欢迎 Pull requests、Issues 一般在24小时内处理
* 讨论与咨询请+QQ 3201590286  :D

# License

[MIT](./LICENSE) 

Copyright (c) 2017 - present, joeyguo
