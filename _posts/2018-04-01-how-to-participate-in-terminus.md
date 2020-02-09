---
layout: post
title:  "如何协作参与端点星计划"
date:   2018-04-01
categories: sticky
tags: 参与
description: Terminus 端点星计划，是在 GitHub 开放平台搭建的一个站点，以去中心化的方式备份微信、微博等平台被删文章。
---

## 端点星计划是什么

Terminus 端点星计划，是在 GitHub 开放平台搭建的一个站点，用于备份微信、微博等平台被删文章。防火墙外也有像 [中国数字时代](https://chinadigitaltimes.net/chinese/)、[GreatFire](https://zh.greatfire.org/)、[自由微博](https://freeweibo.com/)、[自由微信](https://freewechat.com/)、[墙与书](https://wallsandbooks.wordpress.com) 这样的网站做文章备份，但不便于墙内网络传播。

2018年1月发起，以备份微信订阅号、媒体报道社会热点事件的被删文章为主。

## 抵抗404，需要公众参与新方法

在严重依赖微信、朋友圈的情况下，抵抗 404，保证文章传播阅读的持久有效性，现在比较常见的方法有：

- 订阅号菜单栏的非正式群发
- 订阅号小号
- 文字保存为长图片
- 借助有道云笔记

可以发现，这些备份方法并没有很好地使用超链接、微信之外的网站平台，它们有时候也会意想不到的消失，就像断断续续的水滴。

公众参与抵抗404，需要开辟新的方法，重新捡起超链接、网站，再加上开源开放的协作平台。

端点星计划正是出于这样的原因与目的而产生。

## 如何参与端点星计划

### 需要的基本技能

- 熟悉使用 Markdown 基本标记语法
- 熟悉 Markdown 文本编辑器（可选项）：这些工具适用于对 Markdown 语法不熟悉的协作者
  - [MarkdownPad](http://markdownpad.com/)
  - [Atom](https://atom.io/)
  - html 转成 markdown：浏览器插件「[简悦](http://ksria.com/simpread/)」
- 熟悉 GitHub 平台使用

### PR 步骤说明

1. 注册并登录 [GitHub](https://github.com/) 帐号

2. fork 端点星 仓库到自己的 GitHub: 访问[端点星计划](https://github.com/Terminus2049/Terminus2049.github.io) GitHub页面，点击右上角 **Fork** 按钮。

3. 认领备份：查看[端点星 issues](https://github.com/Terminus2049/Terminus2049.github.io/issues)，在标记为 404、help-wanted 的 issue 中发布评论，表示认领该备份文章编辑。

4. 编辑文章备份：在自己帐号里面的 Terminus2049.github.io 仓库，编辑添加备份的文章。

    - 第一种方式：直接在线编辑添加
      1. 点击进入 `_posts/` 文件夹，点击上面的 **Create New File**
      2. 命名文章标题：统一格式为「Year-Month-Day-title.md」，例如 `2018-01-01-biao-ti.md`
      3. 在下方 **Edit new file** 空白区域编辑内容，编辑格式看下方[备份格式编辑要求](#备份格式编辑要求)
      4. 点击 **Preview** 可预览效果
        ![add_new_post.png](https://i.loli.net/2020/02/09/uhZUAWm6yr3MJ4I.png)

    - 第二种方式：从本地上传已编辑的 md 文档
      1. 点击进入 `_posts/` 文件夹，点击 **Upload files**
        ![drag_files.png](https://i.loli.net/2020/02/09/Be21nogCdw4pJlE.png)
      2. 从本地选择要上传的 md 文档

5. 填写 **commit new file**
  ![commit_new_file.png](https://i.loli.net/2020/02/09/fCs72X3pBYgSkT8.png)

6. 向原仓库提交 PR
    
    在自己的仓库页面，点击 **new pull request**，再点击 **create pull request**，填写 PR 描述并提交。
    ![new_pull_request.png](https://i.loli.net/2020/02/09/mONEWGFJwXod1ep.png)

7. 等待 Terminusbot 查看 PR ，符合要求的内容会 merge(合并）。

### 备份格式编辑要求

1. 头部格式：

    ```
    ---
    layout: post
    title:  一女生实名指控曾受沈阳性骚扰
    date:   2018-04-09
    categories: Archive
    tags: 沈阳
    image_feature: ""
    description: 这位女生名叫许红云，她希望更多被沈阳侵扰的女生勇敢地站出来，勇敢地面对过去和现在，才能看到未来。
    ---
    ```
    - layout: post 保持不变
    - title: 用备份文章的标题
    - date: 被删日期
    - categories: Archive 保持不变
    - tags: 标签（在端点星查看是否已有相关标签）
    - image_feature: "如果文章有合适的图片可作为封面图，图片链接填在这里，若无则不填写"
    - description: 可用文章的导语做简述

2. 来源说明格式

    ```
    ---
    原文来自公号名称/网站名称：~~[文章标题](原文链接)~~
    
    作者：XXX
    ---
    ```

3. 正文小标题，使用 h2 或 h3。

4. 图片编辑
  1. 使用 [https://sm.ms](https://sm.ms) 或 [https://imgur.com](https://imgur.com) 图床平台生成链接。
  2. 图注用 `<center>图注</center>` 居中。
