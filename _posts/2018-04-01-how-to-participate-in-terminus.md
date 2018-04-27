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

从 2018 年 1 月至今，端点星网站已有 43 篇文章备份，以微信平台围绕社会热点事件的被删文章为主。尤其在 4 月份近期，有关沈阳事件、武汉理工的新闻报道、评论、倡议行动文章不断被删。

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
- 熟悉 Markdown 文本编辑器（可选项）：这两个工具适用于对 Markdown 语法不熟悉的协作者
  - [MarkdownPad](http://markdownpad.com/)
  - [Atom](https://atom.io/)
- 熟悉 GitHub 平台使用（可选项）

### 协作步骤说明

1. 注册并登录 [GitHub](https://github.com/) 帐号

2. 访问 [端点星计划](https://github.com/Info-cn/Terminus) GitHub页面，点击进入 [_posts](https://github.com/Info-cn/Terminus/tree/master/_posts) 文件夹。

3. 创建备份文章的 markdown 文档，有两种方式

    ![step3](https://i.imgur.com/JSTxYEj.png)

    - 第一种：点击 **Create new file** 在线编辑

    ![step3-1](https://i.imgur.com/gvRxBfm.png)

      1. 文件命名：在 _posts/ 后面的框内输入文件名及后缀，以`2018-01-01-biao-ti.md`的格式
      2. 在下方 Edit new file 空白区区以 markdown 编辑文章
      3. 点击 Preview 可预览效果

    - 第二种：**Upload files**

    ![step3-2](https://i.imgur.com/tPU5I3q.png)

      1. 点击 Upload files
      2. 从本地将编辑好的 markdown 格式备份文档上传

4. 提交 **commit changes**

    在下方填写 commit changes ，简单说明提交的修改是什么

    ![step4](https://i.imgur.com/Ed5t4w3.png)

5. 创建 **pull request** 请求

    点击 **Creat Pull requests**，将刚才新建并进行的分支修改提交到 master 主项目，发起合并请求

    ![step5](https://i.loli.net/2018/04/11/5acdcba0a3813.png)

6. 编辑 pull 请求

    点击 **Create pull request** 之后，在新的页面 **open a pull request** 编辑请求说明

    ![step6-1](https://i.imgur.com/Etexqop.png)

    检查分支与 master 是否存在冲突，若无冲突，则可以合并，经创建者同意，可把分支新增内容加入到 master 主项目中。

    如下图，显示 **This branch has no conflicts with the base branch**，则表示提交的分支请求和 master 无冲突。

    ![step6-2](https://i.imgur.com/ochMeTR.png)

7. 合并请求同意后，会显示紫色

    ![step7](https://i.imgur.com/MFRdDLK.png)

### 协作的文档编辑格式要求

1. 每篇备份 markdown 文章，开头都需要说明文章的标题、时间、标签、简单描述说明。格式如下：

    ```
    ---
    layout: post
    title:  一女生实名指控曾受沈阳性骚扰
    date:   2018-04-09
    categories: Archive
    tags: 沈阳
    description: 这位女生名叫许红云，她希望更多被沈阳侵扰的女生勇敢地站出来，勇敢地面对过去和现在，才能看到未来。
    ---
    ```

    需要修改的是 title、date、tags、description .

2. 正文前面需要注明文章出处及作者，前后用 `---`符号与上下隔开。如下：

    ```
    ---
    原文：~~[财新网:一女生实名指控曾受沈阳性骚扰](http://china.caixin.com/2018-04-09/101231834.html)~~

    [王敖豆瓣广播截图](https://www.douban.com/people/2011446/status/2141828634/)

    ---
    ```

3. 正文小标题，使用 h2 或 h3。

4. 图片使用 [https://sm.ms](https://sm.ms) 或 [https://imgur.com](https://imgur.com) 图床平台生成链接。
