
# web 学习路线指北

> 推荐教程是我目前找到的对新手最友好, 最清晰的教程, 都是我自己学的时候看过的, 推荐你学每项技术的时候**至少**看完我的**每一个**推荐教程  
> 每一项最后都有 check points, **最好**完成相应要求后再继续学习

## lv 0 任何程序员的必备技能

### Markdown

是你看这篇教程有良好体验的基础🌚也是程序员交流的通用格式(程序员用 word 文档就是拉跨), 轻巧, 美观, 功能强大

推荐教程:

- [菜鸟教程: markdown](https://www.runoob.com/markdown/md-tutorial.html)

**check point**: 看懂这篇教程的所有语法

### git & github

git 是**全世界每一个**程序员都要用到的工具, 它可以帮助你 管理/分享 代码.  
github 是基于 git 的, 全世界最大的<del>同性交友</del>程序员社区, 有无数顶尖程序员在上面公开自己的项目/小工具, 你随时可以在上面找到自己想要的代码来*参考*(我会告诉你们上面还有老华科学长分享的大学四年的编程作业吗?)

推荐教程:

- [廖雪峰 git](https://www.liaoxuefeng.com/wiki/896043488029600/896067008724000)
- [B站up code sheep 的 github 分享](https://www.bilibili.com/video/BV1d4411L7Jk)

**check point**: 创建自己的 github 账号, 创建一个学习笔记的仓库, 上传 git 的学习笔记(md 格式)

### 学习如何学习

当你编程遇到问题, 你该如何解决? 想学新的技术, 该在哪找教程? 这些是你整个生涯都会遇到的问题.

#### 解决代码运行问题的方案(排名分先后)

1. 看清楚**报错**信息, 绝大多数时候编译器报错都不会乱报, **把他的英文提示看懂**, 检查一下自己代码有没有他说的问题, 比如你写了这样的程序:

    ```c
    #include <stdio.h>

    int mian(void)
    {
        printf("hello world")

        return 0;
    }
    ```

    报错如下:

    ```bash
    test.c:6:26: error: expected ';' before 'return'
    ```

    塑料英语翻译: 在`return`前期望看到`;`  
    这时候你懂了, `printf`结尾少写了一个`;`, 加上去, 问题解决!

2. 如果真的看不懂报错, 请直接复制整段报错信息, 在**百度里直接搜索**, 如, 你写了这样一段程序:

    ```c
    #include <stdio.h>

    int mian(void)
    {
        printf("hello world");

        return 0;
    }
    ```

    报错如下:

    ```bash
    crt0_c.c:(.text.startup+0x2e): undefined reference to `WinMain'
    ```

    虽然你看不懂这是啥, 但是你知道后面一句```undefined reference to `WinMain'```是关键, 你把他直接粘贴到百度上, 多看几个回答(不要直接看了一个回答就信了他, 可能你们说的根本不是一件事), 找到问题: `main`写成了`mian`, 问题解决!

3. 如果百度还不能解决问题, 请用**必应**试试(其实必应才应该是你的首选搜索引擎, 又不用翻墙, 又比百度牛逼)
4. 如果必应还不行, 请科学上网上**谷歌**查查(关于谷歌, 我后面可能会讲怎么简单的访问到)
5. 如果都不行, 你可以来问我, 我长期在线. 但是你要尽量自己学会如何解决问题, **至少先百度一下**. 要是你来问我个问题, 我发现只要百度一下就有答案了, 我会把你锤爆💩(好吧其实也没啥, 但是我会觉得你在调戏我🌚)

#### 怎么学新技术(排名分先后)

1. 决定学一项技术前, 你可以先考虑考虑这项技术值不值得学. 推荐先上**知乎**搜索一下这个关键词, 多看看相关的话题, 作为参考(而不是决定性因素)
2. 确定了要学之后, 先上 **B站** 查查这个技术的关键词, 看播放量最多的视频作为入门. 好处如下: 弹幕大神可能会给你指路, 避免踩坑 / 看视频较为轻松愉快. 看视频*推荐(但不强求)* **至少开 1.5 倍速看**, 没看懂的地方可以回看, 讲的慢浪费的时间可回不来, 而且光看视频只是让你有个整体印象, 真正要学还得后面自己动手, 所以看视频草率一点其实也还好
3. 看完视频后, 买一本相应的书看(或者上[鸠摩搜书](https://www.jiumodiary.com/)下载电子版). 怎么找好书呢, 首先如果是**O’Reilly**系列的书(特点是封面上画着一只特别的动物, 又叫动物书), 那基本都是好书, 其次淘宝搜关键词, 卖的最好的基本也还行, 最后, 你还是可以随时来问我, 我给你推荐最适合你的书
4. 看完书, **最好动手实践**一下
5. 后期学习难一点的东西, 还可以去过一遍**官方文档**

**check point**(什么?! 这也有检查点? 这不是科普吗?): 没事多看看 B站 up [code sheep](https://space.bilibili.com/384068749/video)的视频(没有夹带私货, 这人讲的是真的很好), 比如睡觉前? 他讲了很多编程新手会问的问题, 只挑你也想了解的部分看就好(比如说上面那个介绍github的视频), 也有很多视频是讲的比较难的, 可以不看/延后看. 建议 1.5 倍速, 节省时间🌚

## to be continued...