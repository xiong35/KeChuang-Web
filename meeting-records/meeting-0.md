
# 20/10/10 第 0 次组会

## web 是干嘛的

web 学习和**网络**相关的各项技术, 解决的问题主要分为:

1. 给用户呈现好看的界面(web 前端)
2. 将用户数据存放在后台, 对数据进行**增, 删, 改, 查**的操作(web 后端)

我们主要学习**前端**相关的技术, 但是也会学习必要的后端知识, 向**全栈工程师**进发

前端的技术栈大致是(包括但不限于):

0. **基础**三剑客: html, css, JavaScript(简称js)
1. 进阶**框架**三选一(排名按推荐程度降序): vue, react, angular(这个放在后面学其实更好, 但是早点学就能早点体会到前端的快乐😏)
2. 程序员**必备素养**: 数据结构, 算法, 设计模式
3. 更**深入**的理解前端: 浏览器存储, http, js 的细节知识点, css 的奇妙特性...
4. 更**高效**的css: sass, less; 更高效的js: TypeScript
5. 向**全栈**进发: node.js(一款让你能用js开发后端服务的框架), 数据库...
6. [and **more**...](https://github.com/xiong35/developer-roadmap/tree/master/translations/chinese)

👆听起来都是高大上的名词, 但是学习来只是一个个相互依赖的知识点罢了, 学好了前面的, 对后面内容的理解就更深刻. 其实都不难, 下面我直接带大家把上面的东西都走一遍, 看完之后你或许会觉得, **就这**?

## web 知识点串讲

### 从 html 讲起...

- html 是什么?
- 是一种**标记语言**, 例如 markdown 其实就是标记语言, 你按特定的格式写东西, 会有现成的工具帮你**把你的标记转换成别的信息**, 如 markdown 转换为好看的格式, html 转换成网页等. 他们不能进行运算, 只能是**声明**我要在这里放一个 标题/列表/链接 等.

### 网页内容只是**字符串**

如题, 当你用浏览器打开一个以html更格式编写的**文本文件**, 浏览器就会按 html 规范进行解析, 把其中内容渲染到浏览器界面.

不信, 可以打开百度首页, 按`ctrl`+`s`保存到桌面, 得到一个 html 文件, 这个文件就是百度首页的代码. 右键点击, 选择用记事本打开, 看到的就是 html 的标签!

> ps: 任何文件只分为两大类: 二进制文件(如图片, 应用, 音频, 视频, ppt, word等需要**解析**的文件)和文本文件(如 C语言代码, txt, markdown, html 文件, 特点是这些文件用记事本都能正常打开)

### css 也是标记语言, 用来声明html的样式

你在html界面里直接写上一些代码, 打开看会发现网站丑的惨不忍睹, 如何做出精美的网站呢? 要利用 css(cascade style sheet, 层叠样式表)对网页的样式进行修改.

### 我怎么让你看到我的网页? 总不能用 qq 发给你让你看吧?

> 看看后端的世界:

#### 服务器

后端有一台(或者好几台)**服务器**. 所谓服务器就是拥有姓名的, 没有显示器的, 放在人家机房里的 电脑.

- 拥有姓名: 电脑的姓名就是 **IP**, ip就是4个数字, 用这个数字就能找到对应的电脑. 你的笔记本没有姓名, 虽然他看上去有 ip, 但是这是路由器给你取的小名, 相当于在村里喊**二麻子**大家都知道是谁, 但是你在实名认证的时候填姓名: 二麻子, 谁知道你是谁?

测试: `win`+`r`, 输入 `cmd` 打开命令行  
输入`ping 8.8.8.8`, 就可以拍一拍谷歌的服务器(对, 谷歌服务器的编号就是这么霸气)  
输入`ipconfig`就可以看到自己电脑的ip, 肯定是形如`192.168.***.***`的, 这种 192.168 开头的 ip 都是*小名*, 别人找不到你的

好, 这台电脑在人家的机房里, **我怎么打开它**?

`ssh` 命令就是用来连接远程服务器的!

cmd 里输入`ssh 8.8.8.8`就可以连接谷歌服务器!...好吧并不能, 你以为谁都可以进入谷歌服务器??

cmd 输入`ssh root@101.133.217.104`, 就可以**以名字叫`root`的用户的身份**尝试登录我的服务器

#### 后端应用

这里我以 node.js 的后端服务为例做展示

只用在js文件里引入相关的包(就是下载并使用别人写好的工具), 调用相关的函数, 返回自己写的**字符串**, 再在浏览器请求对应的地址(比如请求 http://xiong35.cn), 后台应用就可以把网页之类的信息**以字符串形式**传给浏览器, 浏览器**根据 html 的规则解析**, 就可以看到网页了!

此外, 后端还可以根据数据库里的信息, 动态设置网页内的数据(比如说新闻网站的新闻不可能是每天写一个 html 文件吧, 如何只写一个网页, 又保证网页上的新闻是最新的呢? 可以只写好网页的框架结构, 再根据新闻的数据库里拿到的数据, 动态的插进网页里, 就得到了最新的网页)

---

好了, 这就是web的世界观, 是不是很简单呢😁

## 杂项

### 推荐工具

- c语言: dev c++(后期可以(其实是最好)转成用 **vscode** 开发)
- html, css, js: **vscode**
- 浏览器: chrome(首选)或firefox. 反对用 360, 2345等浏览器, 它们里面很多开发者功能是阉割版的
- markdown: 不嫌多下一个应用麻烦就用 typora, 不想下就用 **vscode**

### 快捷键

- `win`+`v`: 调用历史剪贴记录
- `win`+`r`: 打开命令行
- `ctrl`+`z`: 撤销(undo)
- `ctrl`+`y`: 撤销撤销(redo)
- `ctrl`+`f`: **f**ind, 界面内查找