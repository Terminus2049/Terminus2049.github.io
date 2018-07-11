## Terminus
离银河中心最远的行星。

## 端点星计划是什么

Terminus 端点星计划，是在 GitHub 开放平台搭建的一个站点，用于备份微信、微博等平台被删文章。防火墙外也有像 [中国数字时代](https://chinadigitaltimes.net/chinese/)、[GreatFire](https://zh.greatfire.org/)、[自由微博](https://freeweibo.com/)、[自由微信](https://freewechat.com/)、[墙与书](https://wallsandbooks.wordpress.com) 这样的网站做文章备份，但不便于墙内网络传播。

同时，我们运营一个无需手机号和邮箱即可注册的论坛 2049bbs（<https://2049bbs.xyz/>，已被墙，可以通过 <https://45.77.134.176/> 免翻墙访问），欢迎前去自由讨论。

## 如何参与端点星计划

### 如何帮助整理 404 文章

详见置顶文章 [如何参与端点星计划](https://github.com/Terminus2049/Terminus2049.github.io/blob/master/_posts/2018-04-01-how-to-participate-in-terminus.md)

### 如何帮助打破封锁

由于官方 GitHub Page 已经被墙，你可以轻松做一个可直连的网站：

方法：
1. 注册 GitHub
2. fork <https://github.com/Terminus2049/Terminus2049.github.io>
3. 在 setting 中打开 GitHub Page，source 选择“master branch”
4. 在 setting 中将项目名称改为 Terminus
5. 修改 fork 后的仓库，将 `_config.yml` 中第 68 行 `baseurl: # /Terminus` 中的 “#” 去掉，并将 62 行 `url: https://Terminus2049.github.io` 改为 `url: https://<username>.github.io`

然后就可以通过 `https://<username>.github.io/Terminus` 访问。

但是，这些镜像内容无法自动同步，你可以通过设置 [backstroke-bot](https://backstroke.co/) 机器人或者设置定时任务自动同步，详见 [自动更新镜像](https://github.com/Terminus2049/Terminus2049.github.io/issues/106)。

#### 有效镜像

* <https://cmmei.github.io/Terminus/> （同步较快，推荐）
* <https://tsai1993.github.io/Terminus/> （同步较快，推荐）
* <https://scisheiko.github.io/Terminus/>（同步较快，推荐）
* <https://terminus.coding.me/> （微信无法访问）

## 致谢

### 开源程序

- 博客模板 [kiko-now](https://github.com/AWEEKJ/kiko-now)
- 字体方案 <http://cosx.org>
- 分享组件 [Share.js](https://github.com/overtrue/share.js)
- [GitHub Corners](http://tholman.com/github-corners/)
- [pangu.js](https://github.com/vinta/pangu.js)

### 服务

免费可靠的图床 [sm.ms](https://sm.ms/)

### 贡献者

@cmmei @TerminusBot @Tsai1993 @b614103080 @IchiroArisugawa @annfish @Kurocoppla @DarioMeeker @billy3321 @Jephen @scisheiko

特别致谢 [IchiroArisugawa](https://github.com/IchiroArisugawa) 设计的好看 [LOGO](https://github.com/Terminus2049/Terminus2049.github.io/tree/master/images)。

具体贡献可在 [这里](https://github.com/Info-cn/Terminus/graphs/contributors) 和 [这里](https://github.com/Terminus2049/Terminus2049.github.io/graphs/contributors) 查看。

## 版权

### 建站程序版权

本站建站程序来源于 [kiko-now](https://github.com/AWEEKJ/kiko-now)。博客模板文件版权继承并遵循 MIT License。字体选择方案参考了 <http://cosx.org/>。

### 文章版权

[_posts](https://github.com/Terminus2049/Terminus2049.github.io/tree/master/_posts) 文件夹内的文章版权归原作者所有，本站只是防止微信、微博等平台删贴，出于善意原则。如果侵犯了您的权益，请提交 [issue](https://github.com/Terminus2049/Terminus2049.github.io/issues)，我们将在第一时间予以删除。
