### 微前端
微前端的概念是由ThoughtWorks在2016年提出的，它借鉴了微服务的架构理念，核心在于将一个庞大的前端应用拆分成多个独立灵活的小型应用，每个应用都可以独立开发、独立运行、独立部署，再将这些小型应用融合为一个完整的应用，或者将原本运行已久、没有关联的几个应用融合为一个应用。微前端既可以将多个项目融合为一，又可以减少项目之间的耦合，提升项目扩展性，相比一整块的前端仓库，微前端架构下的前端仓库倾向于更小更灵活。

它主要解决了两个问题：

- 1、随着项目迭代应用越来越庞大，难以维护。
- 2、跨团队或跨部门协作开发项目导致效率低下的问题。

![microfroentend](https://img13.360buyimg.com/imagetools/jfs/t1/182098/24/20562/94562/6123569cE7a4b5bc3/f135ab0912746bd6.png ':size=750')

### 关于micro-app
  `micro-app`包含`js`沙箱、样式隔离、元素隔离等特性，并借鉴了`WebComponent`的思想，通过`CustomElement`将`micro-app`封装成一个类`WebComponent`组件，从而实现了微前端的组件化渲染。

  ##### 概念图
  ![image](https://img10.360buyimg.com/imagetools/jfs/t1/168885/23/20790/54203/6084d445E0c9ec00e/d879637b4bb34253.png ':size=750')


### micro-app的优势
  #### 1、使用简单
  我们将所有功能都封装到一个类WebComponent组件中，从而实现在基座应用中嵌入一行代码即可渲染一个微前端应用。
  
  同时`micro-app`还提供了`js沙箱`、`样式隔离`、`元素隔离`、`预加载`、`数据通信`、`静态资源补全`等一系列完善的功能。

  #### 2、零依赖
  `micro-app`没有任何依赖，这赋予它小巧的体积和更高的扩展性。

  #### 3、兼容所有框架
  为了保证各个业务之间独立开发、独立部署的能力，`micro-app`做了诸多兼容，在任何技术框架中都可以正常运行。