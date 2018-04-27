---
layout: post
title: 如何访问 Terminus 以及帮助其他人访问
date:   2018-04-23 18:00
categories: sticky
tags: 参与
description: 成为一个节点，参与有时候很简单。
---

## 背景

基于 GitHub Page 的 <https://info-cn.github.io/Terminus> 已经被定向屏蔽，而目前删贴技术已经到了令人发指的程度，有微信公众号文章在预览阶段就已经 [404](https://github.com/Info-cn/Terminus/issues/64)，在删贴对象上，更是连北大校长的[访谈](https://github.com/Info-cn/Terminus/issues/54)也不放过。这种中心化的发布方式已经不奏效了。

## 解决方案

### 访问

下载 Beaker 浏览器（<https://beakerbrowser.com/docs/install/>），打开

```
dat://d390b864e937859e742a061e7f00936eb27436e2a045054916d5f16269c22cc8/
```

到这里就可以正常访问了。但是希望您能帮助更多的人访问。打开之后，你会在地址栏右边看到一个带有数字的符号，点击之后，会出现这个选项：

![](https://i.loli.net/2018/04/26/5ae1af5916a72.png)

为了帮助更多的人访问，希望您能成为其中一个节点。

### 程序员

如果您是程序员，并且有自己的云服务器，希望您能作出自己一份特殊的贡献。可以按照下述方法，但推荐优先查看教程 [Host outside of Beaker](https://beakerbrowser.com/docs/tutorials/host-outside-of-beaker.html)。

在服务器上创建`~/.dathttpd.yml`文件，填入以下内容：

```bash
letsencrypt:
  email: 'bob@foo.com' # replace this value with your email address
  agreeTos: true
sites:
  mydatsite.com: # replace this key with your server’s hostname，可以不管
    url: dat://d390b864e937859e742a061e7f00936eb27436e2a045054916d5f16269c22cc8
```

然后安装依赖

```bash

# install build dependencies
sudo apt-get install libtool m4 automake make g++

# install dathttpd (https://docs.npmjs.com/getting-started/fixing-npm-permissions)
npm install -g dathttpd

# give node perms to use ports 80 and 443
sudo setcap cap_net_bind_service=+ep `readlink -f
  which node
    `
    # start dathttpd
    dathttpd
```
