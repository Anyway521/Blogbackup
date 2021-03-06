---
title: 让你的VSCode清新脱俗
tags: VSCode
toc: true
abbrlink: 10762
date: 2019-05-16 08:42:38
---

![001.jpg](http://cdn.anyway1314.cn/image001.jpg)

VSCode是Microsoft推出的一款轻量级的编辑器
集成了语法高亮，热键绑定，括号匹配以及代码片段收集功能
是新一代的“编程利器”，下面说一些VSCode的使用优化。
<!--more--> 
# 主题美化
## 1 主题
VSCode自带的主题基本上可以满足一部分人的需求,这里推荐一款用着比较舒服的主题——[“Atom One Dark Theme”](https://marketplace.visualstudio.com/items?itemName=akamud.vscode-theme-onedark)

![at.png](http://cdn.anyway1314.cn/imageat.png)

下载安装扩展后点击左下角设置->颜色主题，选择“Atom One Dark”切换主题。

![y.png](http://cdn.anyway1314.cn/imagey.png)

## 2 图标
左侧栏的图标都是清一色的"黄包包"，看起来会不会太枯燥，推荐扩展[“vscode-icons”](https://marketplace.visualstudio.com/items?itemName=vscode-icons-team.vscode-icons)

![009.png](http://cdn.anyway1314.cn/image009.png)

是不是看起来舒服多了(*^▽^*)~

## 3 背景
不想要单调的黑白色，来点花里胡哨？
推荐扩展[“background”](https://marketplace.visualstudio.com/items?itemName=shalldie.background)

![0078.png](http://cdn.anyway1314.cn/image0078.png)

这个扩展安装后会提示“Code可能已损坏”,不必在意，忽略就行。

安装后在设置里搜索“background”,打开配置文件：

![0056.png](http://cdn.anyway1314.cn/image0056.png)


修改、添加代码：
``` json
"background.useDefault": false,
    "background.customImages":["file:///D:/wc.png"],
    "background.style": {
        "content": "''",
        "pointer-events": "none",
        "position": "absolute",
        "z-index": "99999",
        "width": "100%",
        "height": "100%",
        "background-position": "100% 100%",
        "background-repeat": "no-repeat",
        "opacity": 2
```

完成！（这里用的透明背景图片，所以看起来像是右下角只有一只喵~)

![ao.png](http://cdn.anyway1314.cn/imageao.png)

当然，如果你实在受不了最上方的"不受支持"(比如我)，或者背景确实影响到了你敲代码的心情，可以这样去掉背景：
1、关闭插件
2、在设置打开json文件，注释掉那些关于"background"的代码：

![xiu.png](http://cdn.anyway1314.cn/imagexiu.png)

3、官网重下安装包，覆盖安装（会保留之前的所有配置）。
# 代码扩展
既然是写代码，必然少不了编写各类代码的环境，网上的教程已经有很多了，这里列出一些：

## C/C++ ：
[配置C、C++环境/编写运行C、C++（Windows）](https://blog.csdn.net/bat67/article/details/81268581)
## Java : 
[Win10 配置JDK11](https://blog.csdn.net/qq_40922859/article/details/88078862)

[VSCode 简单配置运行Java](https://www.cnblogs.com/skyball/p/9968170.html)
## Python
[百度经验-Win10配置Python3](https://jingyan.baidu.com/article/3ea51489bebde652e61bbad3.html)

# 实用技巧
## 1 安装扩展龟速？为什么不试试离线安装？
相信很多人和我一样，初次安装扩展的时候，看着软件底部的进度百分比，和扩展上的“正在安装”一直发呆...

其实完全可以用“离线安装”的方式，取代直接在软件上安装的方式。

——>前往 [VisualStudio-Market](https://marketplace.visualstudio.com/vscode)

![vsmap.png](http://cdn.anyway1314.cn/imagevsmap.png)

——>搜索自己需要的扩展，下载离线文件("Download Extension")

![003.png](http://cdn.anyway1314.cn/image003.png)

——>打开VSCode,左上角点击“扩展” -> “...” -> “从VSIX安装”

![kuo.png](http://cdn.anyway1314.cn/imagekuo.png)




