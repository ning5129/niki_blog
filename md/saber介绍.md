# Saber:灵活、高效、可维护的移动 Web 解决方案
轻松搞定从 JavaScript 模块到 CSS 样式库，从开发、调试到构建的全过程

## 为什么选择这个框架
后期项目需求是做移动端数据搜索功能，针对此项目，前端推荐用saber

1. 面向移动场景设计，提供多种模块调用
2. 采用 ETPL 做为模板引擎　ETPL是在CMS里应用过的模板引擎，可降低学习难度
3. 提供了一个基于 Stylus 的样式工具库：rider，可简化移动端的前端样式开发工作
4. 已有团队开发同类功能，可借鉴经验



## 安装与配置
环境要求：node　edp
- node： 官网下载安装
- edp: `  npm install edp -g` 

## 生成项目结构
初始化一个单页面的移动端项目


` edpm init spa` 

> 好处是单页面应用 ，基于MVP架构，结合页面转场与路由管理，增加用户体验


![项目解说](/img/img1.png)

folder | information 
-----|------|
.edpprog    |  项目信息    
dep    |  依赖的包   
doc    |  项目文档   
node_modules　|  本地开发依赖的node的包或者模块 
src |  系统源码
test | 测试case
tool | 本地开发工具包
edp-build-config.js |  edp项目构建的配置模块
edp-rider-config.js　|  edp内置rider的配置文件
edp-watch-config.js | edp监视文件改动的配置文件
edp-webserver-config.js |  edp启动webserver配置文件
index.html |  项目入口页面
module.conf |  项目的AMD模块配置
package.json |  项目初始化配置
README |  你想在这说啥就说啥吧


## 依赖模块
![依赖模块](/img/img2.png)

API: 参考 [文档](http://ecomfe.github.io/saber/doc/)


## 添加模块
` edpm add /common/` 

#  项目具体技术
## 前端模板：ETPL
[ETPL](https://github.com/ecomfe/etpl)是一个强复用、灵活、高性能的JavaScript模板引擎，适用于浏览器端或Node环境中视图的生成。
特点:
- 强复用
- 灵活
- 高性能

API:参考github



## 前端CSS样式库：　rider
rider--是基于 Stylus 与后处理器、无侵入风格的 CSS 样式工具库。

## 安装与配置
- `npm install edp-provider-rider --save-dev`
- edpx-mobile已经内置了edp-provider-rider

## 特性
1. 高效工作流－通过 预处理器 处理样式层的抽象、复用，减少冗余；通过 后处理器 处理兼容性问题、优化输出。
2. 无侵入风格－在预处理阶段，rider 的各种功能均通过 Mixin, Function 或 Block Mixin 的方式提供，只有在主动调用时才输出代码。

## 数据： 从后台请求
> 后台开发建议使用模板，可以减少数据加载等待时间，减少白屏时间

 ## 移动端开发需要处理的问题??
 1. 环境检测
 2. 数据加载形式
 3. 历史回退

 






