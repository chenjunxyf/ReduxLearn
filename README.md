# ReduxLearn

## Redux开发思想

* 单项数据流
* `Redux`和`React`之间没有关系
* `Redux`的`React`绑定包含了容器组件与展示组件分离的思想
* 单一数据源`state`
* `state`只读，唯一通知改变`state`的方法就是触发`action`
* 使用纯函数`reducer`来表示如何修改`(preState, action) => newState`
* `reducer`可以拆分，每个`reducer`只负责管理全局`state`中它负责的一部分。每个`reducer`的`state`参数都不同，分别对应它管理的那部分`state`数据
* 单一`store`，`store`对象将`action`和`reducer`对象连接到一起，提供`dispatch(action)`方法更新`state`
* `createStore()`的第二个参数可以设置初始状态，可以用于把服务器端生成的`state`转变后在浏览器端传给应用
* `react-redux`提供的`connect()`方法将包装好的组件连接到`Redux`
* 任何一个从`connect()`包装好的组件都可以得到一个`dispatch`方法作为组件的`props`，以及得到全局`state`中所需的任何内容

## 使用

```
cd 工程根目录
npm start
```

## demo目录说明

- ReduxLearn --------------------- 项目目录
    + actions  ------------------- 事件：通知改变state
    + components ----------------- UI组件
    + containers ----------------- 容器组件
    + reducers ------------------- reducers：如何改变state
    + dist ----------------------- webpack文件打包目录
    + store ---------------------- redux devtool配置
    + node_modules --------------- node依赖库
    - package.json --------------- 工程配置说明
    - index.html ----------------- demo入口页面
    - index.js ------------------- demo入口js
    - webpack.config.js ---------- webpack配置
    - server.js ------------------ 本地调试浏览服务器
    - .babelrc ------------------- babel配置
    - .gitignore ----------------- git提交忽略文件
    - README.md ------------------ help文档

## 注意

* `import`一个目录时，目录内部需要有`index.js`入口文件

## 参考

* [Redux中文文档](http://camsong.github.io/redux-in-chinese/index.html)
* [redux管理应用](http://www.cnblogs.com/Leo_wl/p/4780750.html)
* [redux-devtools-extension](https://github.com/zalmoxisus/redux-devtools-extension)