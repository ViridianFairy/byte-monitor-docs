# 字节监控前端JSSDK

## 调研阶段

调用市面上流行的前端监控jssdk

## 确定需求
#### 基本需求
1. 错误监控：监控```jsError, resourceError, promiseError, ajaxError, consoleError```，报错数据要尽可能详细
1. 性能监控：通过```performance```API获得用户加载页面时的白屏时间
1. 设备监控：通过```navigator```API获得用户的运行环境如浏览器、分辨率等
1. 上报策略：默认延迟到在用户关闭页面时，将三项监控数据post到后端。

例如：
```js
new Monitor({
	vue: Vue,
	app_id:"abcdabcdabcdabcd123",
});
```
即可运行

5. 使用策略：无侵入式。用户提供一个事先发放的```app_id```对即可使用，```app_id```用来唯一标识一个web应用。

## 开发落地
详情跳转 **test-mini-monitor** 项目

## npm发布