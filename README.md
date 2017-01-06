### 作用
Vuejs 单页应用在iOS的微信webview(或者其他APP)中 标题不能通过 document.title = xxx 的方式修改
该插件只为解决该问题而生

### 效果 (请使用微信扫描打开体验) Vuejs1.x实现

![预览](./preview.png)

直接打开: [http://vue-wechat-title.deboy.cn/](http://vue-wechat-title.deboy.cn/)

### 安装

> Vuejs 1.x

```bash
npm install vue-wechat-title@1.0.6 --save
```

> Vuejs 2.x

```bash
npm install vue-wechat-title@2.0.0 --save
```

### 用法 [demo](https://github.com/deboyblog/vue-wechat-title-demo/tree/use-directive)

##### ES6
> main.js

```js
Vue.use(require('vue-wechat-title'))
```

> App.vue **建议全局只使用一次该指令 标题可用wuex或者router中定义 不要多处使用!!**

```html
<!-- 任意元素中加 v-wechat-title 指令 建议将标题放在 route 的定义中 -->
<div v-wechat-title="$route.title || 'your-title'"></div>
```

### 欢迎提交PR