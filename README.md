#[点我快速安装脚本](https://nightlyfantasy.github.io/Bili_Fix_Player/bili_fix_player.user.js)

脚本新手若观看下面教程无法理解如何安装，可以火狐吧发帖或者博客留言

### Bili_Fix_Player|修复B站播放器

#### 功能:修复B站播放器,黑科技,列表页、搜索页弹窗,破乐视限制,提供高清、低清晰源下载,弹幕下载;注意： 遇到无法播放问题请关闭脚本 

### USO已经挂了，项目托管于github
### [源码地址](https://github.com/NightlyFantasy/Bili_Fix_Player)

### 项目主页【安装地址界面】为
### [项目页面](https://nightlyfantasy.github.io/Bili_Fix_Player/)

脚本地址：
### 地址1[推荐]：[github安装](https://nightlyfantasy.github.io/Bili_Fix_Player/bili_fix_player.user.js)

地址2：[greasyfork](https://greasyfork.org/scripts/740-bili-fix-player)

地址3[已经丢弃]：USO已经挂了，无法更新代码3.5.2，请使用下面的地址，顺便吐槽下USO，真是越来越垃圾

#### 当前最新版本为2014-07-23更新的版本3.6.4
你造吗？使用Github通道将最先获得最新版本

#### 出现无法播放情况先关闭自动修复
> 2014-07-23修复多数BUG

> 2014-07-20修复小BUG，增加评论区移除和谐娘功能 当出现[此楼层已被用户隐藏 点击查看]时，自动展开，需要到脚本设置页面设置

> 2014-07-13你造吗？您可以使用一个海外的代理并将http://interface.bilibili.com/playurl?*作为代理规则加入到代理列表中即可弹窗播放爱奇艺视频（来自田生大神）

> 	  修复弹窗播放时，点击B站FLASH播放器后，若直接点击关闭弹窗，会造成鼠标滚轮无效的问题

> 	  修复360浏览器在脚本设置的时候，被视频君挡住无法设置的问题，方案是（设置的时候先让视频君去火星，设置后再放回来）

> 2014-06-30按照田生大神建议，增加与其脚本匹配id,在弹窗标题增加打开播放页面的按钮，补充，发现BUG，在弹窗播放时，点击B站FLASH播放器后，若直接点击关闭弹窗，会造成鼠标滚轮无效的问题，这BUG作者暂时无修复方法

> 	  并且使用了田生大神分支里面的弹窗播放器支持网页全屏功能，感谢

> 2014-06-21修复搜索页面因为作者正则匹配错误（B站把域名换成com但在a标签还是tv域名，坑爹）的问题

> 2014-06-18修复B站更换域名的BUG，在田生大神的建议下，将所有api域名换成com，弹窗播放器增加收藏按钮

> 2014-06-08修复小部分bug(样式冲突、弹窗冲突)

> 2014-06-03增强弹窗播放器，[拖动窗口标题可移动播放器，拖动右下角可改变播放器大小，设置后自动保存宽高和位置]

> 2014-05-25感谢吧友lzgptdgj提供BUG，在小型播放器下，屏蔽规则会无效的问题，已经修复

> 2014-05-14增加首页弹窗播放，基本实现全站可弹窗（首页新番专题列表除外等）

> 2014-05-13增加搜索页面的弹窗播放，并且支持多P和显示当前P，增加模糊画质下载按钮

> 2014-05-11还是基佬要求，增加弹窗播放器分P效果，增加弹幕下载功能，在吧友大神田生的建议下，正则表达式加强匹配

> 2014-05-10收益于自己的B站追番计划(http://v.myacg.ga或者http://weiyun.jd-app.com)，代码逻辑重构(不再区分视频源再解析视频)，并重写UI

> 2014-05-10受诸多基佬要求，增加除首页外其他分类页面的弹窗播放(初衷是为了弹窗乐视源)

> 2014-03-28增加下载视频按钮

> 2014-01-23替换优酷、爱奇艺、搜狐为B站播放器

> 2013-12-14修复B站播放器无法在火狐魔镜弹窗播放

> ------------以下信息提供给开发者-----------

> //https://static-s.bilibili.tv/play.swf---新版播放器

> //http://static.hdslb.com/play.swf---旧版播放器

> //https://static-s.bilibili.tv/play_old.swf---考古级别播放器

> //使用https连接的播放器可以获得屏蔽列表

-------------------------------------------
### 脚本功能：
0:概述功能{

![github](http://bilili.ml/wp-content/uploads/2014/07/bilifix1.png "github")

}

{包含功能：提供高清画质和低品质画质视频下载，提供xml弹幕下载，可自由切换是否启用脚本和播放器大小，评论区分页悬浮，评论区去和谐}

1：提供高清画质和低品质画质视频下载，提供xml弹幕下载，可自由切换是否启用脚本和播放器大小

如上图，直接在视频播放页面点击脚本里面的所需功能区域字符即可，可以

【自动替换外站播放器为B站播放器（如优酷、搜狐等，爱奇艺和乐视需要使用弹窗播放，详细看下面2介绍）】

【高清画质和低品质画质视频下载，提供xml弹幕下载】

【可自由切换是否启用脚本和播放器大小】

【评论区分页悬浮，评论区去和谐】

2：提供二级页面的弹窗播放效果，可以自由弹窗播放，如新番页面，MV页面和音乐页面（多P支持并显示当前播放P），附带分P列表
乐视番弹窗即可破解，

爱奇艺番【可以使用一个海外的代理并将http://interface.bilibili.com/playurl?*作为代理规则加入到代理列表中即可弹窗播放爱奇艺视频】然后搜索所需的弹窗即可破解，

![github](http://bilili.ml/wp-content/uploads/2014/07/bilifix3.png "github")

3：评论区域分页悬浮

当想要迅速分页查看评论时每次都需要滚动到页底部？本功能帮助你【需要到步骤1那里设置打开】，实现分页栏悬浮，快速翻页

![github](http://bilili.ml/wp-content/uploads/2014/07/bilifix2.png "github")

4：评论区域去和谐
2333每次都会看到这种情况？

![github](http://bilili.ml/wp-content/uploads/2014/07/bilifix4.png "github")

本功能帮助你【需要到步骤1那里设置打开】，实现评论去和谐，快速浏览信息

OK，打开该功能后，

![github](http://bilili.ml/wp-content/uploads/2014/07/bilifix5.png "github")

#### 脚本的安装方法，以下只简单介绍安装方法，如果有不明白的，可以去百度火狐吧贴吧提问，或者在本博下面回复，我们尽量帮您
### 概况安装方法：
		火狐浏览器用户，在安装Greasemonkey扩展后安装该脚本即可使用
		chrome浏览器（包括chrome壳子的诸如360，猎豹，搜狗等等的极速模式）用户，在安装Tampermonkey扩展后安装该脚本即可使用；

### 详细脚本的安装:
		火狐浏览器{
		1.在这个地址安装addons.mozilla.org/zh-CN/firefox/addon/greasemonkey安装这个扩展；
		2.重启火狐；
		3.在本页，点击install即可在B站使用
		}
		chrome(包括chrome壳的浏览器：包括chrome壳子的诸如360，猎豹，搜狗等等的极速模式){
		1.在谷歌应用商店搜索安装Tampermonkey扩展，然后同上；
		2.（chrome壳：包括chrome壳子的诸如360，猎豹，搜狗等等的极速模式）
		在应用商店搜索安装Tampermonkey扩展，然后同上；
		如果搜索不到，那么谷歌搜索Tampermonkey扩展，下载到本地，然后拖到扩展管理器安装扩展即可；
		}

出现无法播放情况先关闭自动修复

感谢各位大神和B站爱好者的支持，跑路搬砖走起

### [BUG反馈地址](http://bilili.ml/361.html)