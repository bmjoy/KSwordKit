# 概述
这是一套完整的 Unity 框架方案，提供 UI，热更新，资源管理等，多线程、数据处理、定时器、解压缩等功能完备的工具集。

目的是为了提高生产力，方便业务开发。

未来的预期中也将加入更多游戏技术，比如帧同步等。

# 目前框架并不完整，刚开坑，欢迎大家查指正
刚开始构思这个框架，正好公司项目也在做优化，所以在这里开坑造轮子了，希望大家给出宝贵的意见。

# 当前框架内可用模块
1. [资源管理器](资源管理器)
2. [增强协程](增强协程)

## 当前框架内正在开发的模块
1. Lua管理器
2. 数据处理器
3. 多线程
4. 项目文件管理器
5. 定时器
6. UI管理器

# 框架部件的独立无依赖原则
框架内将提供很多种部件，设计模式、功能和依赖都会不尽相同。但这些部件都需要遵循同一个原则：**独立无依赖**

**每个部件应当是独立的，以便可以直接单独复制到别的项目就可以直接使用的，这就要求自身没有任何对外部的依赖**。这样可以方便开发者根据需求自定义增减内容，框架更包容，不排他。

>部件：有的人叫做组件，有的则被叫做工具，有的则被称为插件，在这里它们都被称为框架的部件。

如有朋友设计并实现了某部件，想给本仓库提交PR，提交之前请让您的代码遵循该原则即可。
