## POST /api/uploadErrors
> 发送若干条报错数据
```js
[
  {
    type: 'vue_error',
    error_info: 'vue错误测试 is not defined',
    error_url: '组件名App',
    error_row: 0,
    error_col: 0,
    error_extra: 'ReferenceError: vue错误测试 is not defined\n' +
      '    at VueComponent.created (webpack-internal:///./node_modules/cache-loader/dist/cjs.js?!./node_modules/vue-loader/lib/index.js?!./src/App.vue?vue&type=script&lang=js&:40:3)\n'
    hash: '524b09ebe232bf59ef32f4da7bbfc656',
    amount: 1,
    user_id: 'JPcwmH8MSW1629076016127',
    app_id: '114514114514abc',
    time: '2021-08-16T01:35:41.905Z'
  },
  {
    type: 'js_error',
    error_info: 'Uncaught ReferenceError: test3 is not defined',
    error_url: 'webpack-internal:///./src/main.js',
    error_row: 32,
    error_col: 1,
    error_extra: {},
    hash: '90b4bd4993043b913af9473c5b033f1a',
    amount: 1,
    user_id: 'JPcwmH8MSW1629076016127',
    app_id: '114514114514abc',
    time: '2021-08-16T01:35:41.917Z'
  },
  {
    type: 'ajax_error',
    error_info: 'Cannot POST /api/x',
    error_url: 'http://127.0.0.1:3030/api/x',
    error_row: 0,
    error_col: 0,
    error_extra: { status: 404, statusText: 'Not Found' },
    hash: '93aa3f3bbdcddf3926c3f13d8f3b4ba6',
    amount: 30,
    user_id: 'JPcwmH8MSW1629076016127',
    app_id: '114514114514abc',
    time: '2021-08-16T01:35:41.927Z'
  },
  {
    type: 'resource_error',
    error_info: '加载IMG资源失败',
    error_url: 'https://pic.xiaohuochai.site/blog/chromePerformance2_error.png',
    error_row: 0,
    error_col: 0,
    error_extra: {},
    hash: 'e98e12d5e1e061869549464aa9fc1f8d',
    amount: 11,
    user_id: 'JPcwmH8MSW1629076016127',
    app_id: '114514114514abc',
    time: '2021-08-16T01:35:42.107Z'
  },
  {
    type: 'promise_error',
    error_info: 'woops',
    error_url: '[object Window]',
    error_row: 0,
    error_col: 0,
    error_extra: '',
    hash: '87e3daaf1230787ae76f3b3c4deaa375',
    amount: 1,
    user_id: 'JPcwmH8MSW1629076016127',
    app_id: '114514114514abc',
    time: '2021-08-16T01:35:42.418Z'
  }
]
```


## POST /api/uploadPerformance
> 发送用户页面的性能数据
```js
{
  url: 'http://192.168.0.108:8080/',
  redirectTime: 0,
  dnsTime: 0,
  ttfbTime: 8,
  reqTime: 0,
  loadPageTime: 390,
  user_id: 'JPcwmH8MSW1629076016127',
  time: '2021-08-16T01:36:17.076Z'
}
```

## POST /api/uploadDevice
> 发送用户设备数据
```js
{
  deviceType: 'PC',
  OS: 'Windows',
  OSVersion: '10.0',
  screenHeight: 1080,
  screenWidth: 2560,
  language: 'zh_CN',
  netWork: '4g',
  orientation: '竖屏',
  browserInfo: 'Chrome（版本: 91.0.4472.164&nbsp;&nbsp;内核: Blink）',
  user_id: 'JPcwmH8MSW1629076016127',
  time: '2021-08-16T01:35:41.895Z'
}
```