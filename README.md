## 实现 Vue3 核心模块

- TDD 测试驱动开发
- [vitest](https://cn.vitest.dev/) 测试框架
-  [ChatGPT](https://ask.vuejs.news/) 编写单元测试 😄
- [excalidraw](https://excalidraw.com/) 画图



代码并没有按照源码的方式去进行组织，目的是学习、实现 vue3 响应式系统的核心，用最少的代码去实现最核心的能力，减少我们的学习负担，并且所有的流程都会有配套的图片，图文 + 代码，让我们学习更加轻松、快乐。

每一个功能都会提交一个 `commit` ，大家可以切换查看，也顺变练习练习 git 的使用。

代码地址： https://github.com/SuYxh/share-vue3 



### 安装

```
pnpm i 
```



启动

```
pnpm dev
```



测试

```
pnpm test
```



启动文档

```
pnpm docs:dev
```



### 响应式系统

#### 已实现

- [x] 响应式数据以及副作用函数
- [x] 响应式系统MVP模型
- [x] 依赖收集
- [x] 派发更新
- [x] 依赖清理
- [x] 嵌套 effect
- [x] scheduler
- [x] computed
- [x] watch



#### 系列文章

- [实现vue3响应式系统核心-MVP模型](./docs/reactive/docs/实现vue3响应式系统核心-MVP模型.md)
- [实现vue3响应式系统核心-依赖清理](./docs/reactive/实现vue3响应式系统核心-依赖清理.md)
- [实现vue3响应式系统核心-嵌套effect](./docs/reactive/实现vue3响应式系统核心-嵌套effect.md)
- [实现vue3响应式系统核心-scheduler](./docs/reactive/实现vue3响应式系统核心-scheduler.md)
- [实现vue3响应式系统核心-computed](./docs/reactive/实现vue3响应式系统核心-computed.md)
- [实现vue3响应式系统核心-watch](./docs/reactive/实现vue3响应式系统核心-watch.md)
- [实现vue3响应式系统核心-增强对象拦截](./docs/reactive/实现vue3响应式系统核心-增强对象拦截.md)
- [实现vue3响应式系统核心-合理触发响应](./docs/reactive/实现vue3响应式系统核心-合理触发响应.md)
- [实现vue3响应式系统核心-shallowReactive](./docs/reactive/实现vue3响应式系统核心-shallowReactive.md)
- [实现vue3响应式系统核心-readonly&shallowReadonly](./docs/reactive/实现vue3响应式系统核心-readonly&shallowReadonly.md)
- [实现vue3响应式系统核心-代理数组](./docs/reactive/实现vue3响应式系统核心-代理数组.md)


#### 流程图

##### 响应式数据结构

![image-20240118223902472](https://qn.huat.xyz/mac/202401182239504.png)





##### 响应式系统 MVP 模型

![image-20240118223949999](https://qn.huat.xyz/mac/202401182239017.png)



##### 依赖清理

![image-20240118224016622](https://qn.huat.xyz/mac/202401182240651.png)

##### 嵌套 effect

![image-20240118224141690](https://qn.huat.xyz/mac/202401182241712.png)

##### scheduler

![image-20240118224210357](https://qn.huat.xyz/mac/202401182242379.png)

##### computed

![image-20240118224353017](https://qn.huat.xyz/mac/202401182243042.png)



##### watch

![image-20240118224413560](https://qn.huat.xyz/mac/202401182244587.png)





### 参考

1、《vuejs 设计与实现》霍春阳