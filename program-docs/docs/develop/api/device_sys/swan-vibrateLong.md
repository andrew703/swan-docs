---
title: swan.vibrateLong
header: develop
nav: api
sidebar: swan-vibrateLong
# webUrl: https://qft12m.smartapps.cn/subPackages/apiPackage/pages/vibrate/vibrate
---


 

> 在工具和真机中的实现有区别，详见[API 实现差异](https://smartprogram.baidu.com/docs/develop/devtools/diff/)。

**解释**： 使手机发生较长时间的振动（400ms）

  

## 方法参数 

Object object

### `object`参数说明  

|属性名 |类型  |必填 | 默认值 |说明|
|:---- |:---- |:---- |:----|:----|
|success| Function  |  否  | |接口调用成功的回调|
|fail  |  Function  |  否 | | 接口调用失败的回调函数|
|complete  |  Function |   否 | | 接口调用结束的回调函数（调用成功、失败都会执行）|

## 示例
<a href="swanide://fragment/e87388ef787854a02ca900c6c28307dd1569483846383" title="在开发者工具中预览效果" target="_self">在开发者工具中预览效果</a>


### 扫码体验

<div class='scan-code-container'>
    <img src="https://b.bdstatic.com/miniapp/assets/images/doc_demo/vibrate.png" class="demo-qrcode-image" />
    <font color=#777 12px>请使用百度APP扫码</font>
</div>


###  代码示例 




* 在 js 文件中

```js
Page({
    vibrateLong() {
        swan.vibrateLong({
            success: res => {
                console.log('vibrateLong success', res);
            },
            fail: err => {
                console.log('vibrateLong fail', err);
            }
        });
    }
});
```


