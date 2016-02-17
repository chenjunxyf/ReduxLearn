# ReduxLearn

## Redux开发思想

* `Redux`和`React`之间没有关系
* `Redux`的`React`绑定包含了容器组件与展示组件分离的思想
* 单项数据流
* 单一数据源`state`
* `state`只读，惟一改变`state`的方法就是触发`action`
* 使用纯函数`reducer`来执行修改`(preState, action) => newState`

## 参考

[Redux中文文档](http://camsong.github.io/redux-in-chinese/index.html)