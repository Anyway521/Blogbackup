---
title: VSCode-PicGo插件配置七牛云图床
tags:
  - VSCode
  - PicGo
toc: true
abbrlink: 53597
date: 2019-07-13 11:40:07
---
![qiniu.jpeg](http://cdn.anyway1314.cn/imageqiniu.jpeg)

文件存储的方式让图片耗费了大量的流量资源<br>如果你想提高网站的加载速度，图床不失为一种好的选择!
<!--more-->

# 注册七牛云
## [注册页面](https://portal.qiniu.com/signup)

![20190713133555.png](http://cdn.anyway1314.cn/image20190713133555.png)

## 新建存储空间
这里要注意，`访问控制`选择`公开空间`。

![20190713133420.png](http://cdn.anyway1314.cn/image20190713133420.png)

## 绑定域名(融合CDN加速)
七牛云为对象存储设置的测试域名是有时限的(30天后自动回收)，所以这里要绑定自己的域名(建议使用二级域名)。<br>
选择`对象存储`->`绑定域名`

![20190714131349.png](http://cdn.anyway1314.cn/image20190714131349.png)

填写相关信息

![QQ截图20190714130613.png](http://cdn.anyway1314.cn/imageQQ截图20190714130613.png)

点击绑定的域名、可以找到`CNAME`的记录值

![20190717110543.png](http://cdn.anyway1314.cn/image20190717110543.png)

在域名控制台添加子域名解析记录

![QQ截图20190714124401.png](http://cdn.anyway1314.cn/imageQQ截图20190714124401.png)

# 下载插件PicGo
## [插件链接](https://marketplace.visualstudio.com/items?itemName=Spades.vs-picgo)(或在VScode扩展安装)

![20190713134438.png](http://cdn.anyway1314.cn/image20190713134438.png)

## 插件配置
打开设置、找到插件PicGo、设置默认图床为七牛(qiniu)

![20190713134836.png](http://cdn.anyway1314.cn/image20190713134836.png)

往下找，继续设置:

![q20190713135448.png](http://cdn.anyway1314.cn/imageq20190713135448.png)

*上面的`Access/Secret Key`在七牛云，`头像`->`秘钥管理`:


![QQ截图20190713142125.png](http://cdn.anyway1314.cn/imageQQ截图20190713142125.png)

# PicGo使用
## 1、从剪贴板上传
快捷键:  Crtl + Alt + U<br>

![0a07cd8d44e9a91284c0e5aaba984d85_68747470733a2f2f692e6c6f6c692e6e65742f323031392f30342f30392f356361633137643264323236352e676966.gif](http://cdn.anyway1314.cn/image0a07cd8d44e9a91284c0e5aaba984d85_68747470733a2f2f692e6c6f6c692e6e65742f323031392f30342f30392f356361633137643264323236352e676966.gif)

## 2、从文件上传
快捷键:  Crtl + Alt + E<br>

![5cac17eea0d65.gif](http://cdn.anyway1314.cn/image5cac17eea0d65.gif)

## 3、从输入框上传
快捷键:  Crtl + Alt + O<br>

![80321c023c7ee54463695dad2e8f7da1_68747470733a2f2f692e6c6f6c692e6e65742f323031392f30342f30392f356361633137666535326138362e676966.gif](http://cdn.anyway1314.cn/image80321c023c7ee54463695dad2e8f7da1_68747470733a2f2f692e6c6f6c692e6e65742f323031392f30342f30392f356361633137666535326138362e676966.gif)
