
# meeting-2 真实的前端项目是什么样的

> 你们以后可能要做大创, 就可以参考这个模式来

## 开始项目之前

### 真的需要做这个项目吗

需要分析市场上的竞品有哪些, 为什么认为我们的项目能做的比他们好, 要是不能把某个方面做的更好, 还要不要继续做下去

### 前期设计

讨论出以下内容: 

- 核心 feature
- 大致功能
- UI 风格
- 目标群体
- 进行用户调研(一般是发问卷)
- 后期可以迭代升级的地方
- 技术实现的难点
- 分工接锅(包括拉人和分工两部分)

讨论好了才方便后面开始干活

### 写文档

写好文档比写好代码还重要!!!  
写出了一个好的文档, 任务就完成了七成了, 剩下的就是按着文档打代码就好

文档实例: [线上狼人杀文档](https://github.com/xiong35/techtrainingcamp-h-fe-3/tree/master/docs)

文档一般分为两大部分, 需求文档和api文档

- 需求文档就是 todo list, 只要按着他说的把每个功能都实现了, 项目也就基本做完了
- API 文档是为了<del>避免前后端吵架</del>前后端协作而定的, 大家都按照文档写代码/测试, 谁和文档不一样就是谁的锅

写文档的人需要头脑清醒, 经验丰富, 因为文档就是标准, 写出个逻辑不自洽的文档是很麻烦的一件事...

## 创建项目

一般就是创建一个项目然后推到github上, 然后添加合作者(进到repo->settings->manage access->invite a collaborator), 这样大家就都能往同一个库提交代码了

当然也可以自己配置 gitlab, 这个更加私密

### 技术栈

#### 原生

目录结构一般是这样的:

```
|
+---assets
|   |
|   +---img
|   +---font
|   +---data
|
+---docs
+---js
+---css
+---html
|
+---.gitignore
+---.editorconfig
```

#### 框架

vue

```bash
npm install -g @vue/cli-init
vue init webpack my-project
```

react

```bash
npx create-react-app my-app
```

框架产生的代码浏览器是不能直接读懂的, 需要对应的编译工具把他变成原生js/html/css, 但是这些往往都由框架帮你完成, 想了解内部原理可以看看 webpack 和 babel

## 分工合作

现在才是大家最喜欢的打代码环节.

其实就没啥说的了, 找设计要图, 对着文档写功能, 就很轻松很快乐, 注意代码规范和 commit 写清楚就好

[git network](https://github.com/ahabhgk/techtrainingcamp-h-fe-3/network)

## 持续集成

> 针对用了框架的项目

每次更新代码, 都要在部署环境上 pull, 编译, 打包, 发布, 刷新服务, 重复的工作太多了!!

运用 CI (Continuous Integration)框架(用的最多的是 Jenkins)可以自动化完成上述工作, 每次 commit 之后都会自动部署最新的代码

## 随时待命改 bug

...如题
