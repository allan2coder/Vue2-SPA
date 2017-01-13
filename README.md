# Vue2-SPA

> A Vue.js project 

### Other SPA(其他单页)
- [vue2.x](https://github.com/allan2coder/VUE2-SPA-Tutorial)
- [React.js 2.x](https://github.com/allan2coder/React-SPA-Tutorial) :fire: :fire: :fire:
- [Angularjs 2.x](https://github.com/allan2coder/Angular2-SPA)

## screenShot
![image](https://github.com/allan2coder/Vue2-SPA/blob/master/src/images/1.png)

## Features

- 采用ES6语法，组件化、模块化开发
- :checkered_flag: :rotating_light: 严格的语法检测 [Vue2(不带语法检测的版本戳这里吧- -)](https://github.com/allan2coder/VUE2-SPA-Tutorial)
- 前端控制路由
- 自动打开、刷新浏览器

- Equip with Vue2.x, ES6 & Babel 6
- Lint with JSHint.
- Build with Webpack

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm start

# build for production with minification
npm run build

# run unit tests
npm run unit

# run e2e tests
npm run e2e

# run all tests
npm test
```


# How to ues Vue-router

HTML
``` bash

import Vue from 'vue'
import VueRouter from 'vue-router'

<template>
    <!-- 使用 router-link 组件来导航. -->
    <!-- 通过传入 `to` 属性指定链接. -->
    <!-- <router-link> 默认会被渲染成一个 `<a>` 标签 -->
    <p>
      <router-link to="/foo">Go to Foo</router-link>
      <router-link to="/bar">Go to Bar</router-link>
    </p>
    <!-- 路由出口 -->
    <!-- 路由匹配到的组件将渲染在这里 -->
    <router-view></router-view>
  </div>
</template>
```

JavaScript
``` bash

// 0. 如果使用模块化机制编程，導入Vue和VueRouter，要调用 vue.use(vuerouter)

// 1. 定义（路由）组件。
// 可以从其他文件 import 进来
const Foo = { template: '<div>foo</div>' }
const Bar = { template: '<div>bar</div>' }

// 2. 定义路由
// 每个路由应该映射一个组件。 其中"component" 可以是
// 通过 Vue.extend() 创建的组件构造器，
// 或者，只是一个组件配置对象。
// 我们晚点再讨论嵌套路由。
const routes = [
  { path: '/foo', component: Foo },
  { path: '/bar', component: Bar }
]

// 3. 创建 router 实例，然后传 `routes` 配置
// 你还可以传别的配置参数, 不过先这么简单着吧。
const router = new VueRouter({
  routes // （缩写）相当于 routes: routes
})

// 4. 创建和挂载根实例。
// 记得要通过 router 配置参数注入路由，
// 从而让整个应用都有路由功能
const app = new Vue({
  router
}).$mount('#app')

// 现在，应用已经启动了！
```

# Reference Articles
* [Vue-Router](http://router.vuejs.org/zh-cn/essentials/getting-started.html)
* [ECMAScript 6入门](http://es6.ruanyifeng.com/)
* [Webpack 入门指迷](https://segmentfault.com/a/1190000002551952)
* [webpack使用优化](https://github.com/lcxfs1991/blog/issues/2)
* [vue guide](http://vuejs-templates.github.io/webpack/)
* [docs for vue-loader](http://vuejs.github.io/vue-loader)

For detailed explanation on how things work, checkout the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
