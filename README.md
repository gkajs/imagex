# Install

```
$ npm i imagex
```

# Usage

```js
var imagex = require("imagex");

imagex({
    src       : "/pictures/src",  // 原图片文件夹地址
    dest      : "/pictures/dest", // 输出文件夹地址
    prefix    : "prefix-",  // 序列化重命名
    isMini    : true,  // 图片压缩
    isCrop    : true, // 图片空白裁剪
    isUnique  : true, // 图片去重
    isSprites : true, // 合图
    algorithm : "left-right", // 合图方式
}, function(data){
    
    console.log(data);  // data 图片信息数据
}

```

# Welcome

* 欢迎 Pull requests、Issues 一般在24小时内处理
* 讨论与咨询请+QQ 3201590286  :D

# License

[MIT](./LICENSE) 

Copyright (c) 2017 - present, joeyguo