微信小程序中实现Mixins

## 安装
```
npm i wx-mixins -S
```


## Mixins 使用

### 在小程序的`app.js`里引入 `wx-mixins`
```
require('wx-mixins')
```
### 撰写一个`myMixin.js`
```
module.exports = {
  data: { someData: 'myMixin' },
  onShow () { console.log('Log from mixin!') }
}
```
### 在`page/index/index.js`中使用
```
const myMixin = require('../../myMixin.js')

Page({
  mixins: [myMixin]
})
```


## 实现
[在小程序中实现 Mixins 方案](https://mp.weixin.qq.com/s/V3HAOYCHjSS7tSvyKzXh7A)