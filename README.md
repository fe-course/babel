# Babel

## Babel基础

`babel-cli` 执行babel编译的CLI命令
`babel-core` babel核心的API，用于使用babel API编程
`babel-register` 文件中引入babel-register即可运行babel方法编译，不适合生成环境
`babel-node` 用于支持node cli来运行代码

## 配置`.babelrc`

1.`.babelrc`文件中需要这样来预设

```
{
  "presets": [],
  "plugins": []
}
```

## 常用插件说明

1.预设插件
`babel-preset-react` 编译react预设
`babel-preset-es2015` 编译es2015预设
`babel-preset-stage-2` 编译es2015的新提案预设

2.兼容
`babel-polyfill` 让浏览器可以运行新的es2015 API（babel默认是转换es2015语法）

Babel默认不转码的API非常多，详细清单可以查看babel-plugin-transform-runtime模块的definitions.js文件。

3.让生成的代码保持整洁
`babel-plugin-transform-runtime`
`babel-runtime`
