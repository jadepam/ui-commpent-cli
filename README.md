# ui-commpent-cli
前端UI组件库架构

## 前端组件系统设计思路及模式
- 设计先行原则:对于组件库实现是一方面,但具体样式的设计一定要与业务相结合。
- 详细设计接口:这里以 form 为例,讲解一下作为一个合格的组件库,我们需要设计哪些接口。
  form组件设计需要注意的内容:校验(async-validator)\API 设计(高阶组件封装 API)
## 组件库开发、管理及调试模式
- 组件库一般会搭配 lerna(包管理) 、 babel-plugin 或者一些可视化工具来进行设计、开发和管理

- 在不支持 tree-shaking 的打包环境下,我们就可以使用babel 插件 import,实现按需加载

- css:css-in-js

- 依赖控制:peerDependiencies

- 暴露webpack config: npm run eject