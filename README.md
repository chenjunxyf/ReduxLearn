# ReduxLearn

## Redux开发思想

* `Redux`和`React`之间没有关系
* `Redux`的`React`绑定包含了容器组件与展示组件分离的思想
* 单项数据流
* 单一数据源`state`
* `state`只读，惟一改变`state`的方法就是触发`action`
* 使用纯函数`reducer`来执行修改`(preState, action) => newState`

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