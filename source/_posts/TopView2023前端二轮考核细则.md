---
title: TopView2023前端二轮考核细则
date: 2023-07-11 10:47:12
comments: true #是否可评论
toc: true #是否显示文章目录
categories:  #分类
    - 考核细则
tags:   #标签
    - TopView
    - 考核
---

## 1. 考核题目

“这里是哪里？”

“这里是【β世界线】，2023年4月4日，年轻人”

一位叫做cherry的年轻人回答了刚刚醒来的韶葱师兄

“我为什么会在这里...”

“我还能回到之前的世界线吗...”

韶葱师兄模糊不清地问道

“当然可以”

“但你得先帮我做一件事，小伙子”

名为cherry的年轻人似乎早已预料到韶葱师兄的问题

“什么事情，是你把我带到这个世界线的吗...”

此时cherry笑了一笑

“是的，我把你带过来的目的便是让你帮我写一个【视频网站】”

“为什么...”

韶葱师兄不解

“因为我在这个世界线轮回了无数次，这个世界线终究会向【绝望乡】的终点收束”

“而我找到唯一能改变的方法，便是选择合适的【观测者】，并创造出一个视频网站”

“然后我将承诺这个网站可能会倒闭，但绝不会变质。这样世界线将会走向【幻想乡】的收束点”

下面是cherry准备的【视频网站需求】

[Bilibili 网页版](https://www.bilibili.com/)（内测版）
![image.png](https://cdn.nlark.com/yuque/0/2023/png/25611084/1680886037266-32e67aa0-3e97-447f-ad52-ed15d4921f1e.png#averageHue=%23867b45&clientId=udefb64f3-23ad-4&from=paste&height=1000&id=u12b4a8ba&name=image.png&originHeight=1750&originWidth=3200&originalType=binary&ratio=1.75&rotation=0&showTitle=false&size=3746952&status=done&style=none&taskId=u1b1ab00b-8a75-498d-b4ac-484a99da296&title=&width=1828.5714285714287)

> - 在网页右下角选择内测版
> - [内测版与新版的区别](https://www.sohu.com/a/637218106_121654364)，根据此文章判断自己现在是不是内测版

## 2. 考核需求
### 2.1 页面布局
顶部栏 + 内容区（放缩页面 50%~150% 布局不错乱，注意未登录和登录后的界面区别）
### 2.2 首页

- 基本页面布局+样式
- 实现懒加载效果
- 实现瀑布流无限加载效果（视频从接口请求，接口提供十个视频，重复使用即可）
- 鼠标悬停自动开始播放视频，播放的同时要展示视频水印（bilibili的logo + UP主名称，默认在视频**画面**右上角，注意横屏视频与竖屏视频的水印均要在视频**画面**的右上角），移出暂停并隐藏视频水印
- 鼠标悬停自动开始播放该视频的弹幕（进阶）
- 点击视频进入视频详情页

**视频详情页**

   - 基本页面布局+样式
   - 右边侧边栏实现样式即可，视频可用图片代替可以自找或者用背景色代替，文字、播放量、弹幕数、UP主、视频时长自定义
   - 实现点赞，投币，收藏功能（统计点赞数、投币数与收藏数），收藏的作品可在个人主页展示，无需实现关注功能
   - 使用账号在视频播放页面下添加评论、删除评论，显示评论时间
   - 其他账号可点赞和回复评论（进阶）
   - 不依赖原生 video 标签的控件，自定义控件，例如：播放暂停，进度条，音量控制，倍速播放，宽屏模式，网页全屏，进入全屏等（进阶）
   - 实现视频水印功能（bilibili的logo + UP主名称，默认在视频**画面**右上角，注意横屏视频与竖屏视频的水印均要在视频**画面**的右上角）
   - 实现一键三连功能（长按后点赞、投币、收藏）
   - 实现普通滚动弹幕功能（统计弹幕数，实现视频右边的弹幕列表）（进阶）
   - 实现高级弹幕功能，可以自己找视频测试该功能（注意弹幕列表中高级弹幕与普通弹幕之间的区别）（终极）
![image.png](https://cdn.nlark.com/yuque/0/2023/png/25611084/1679755970999-62bcc496-aa0d-48c8-a5b0-a8e8ef274d9f.png#averageHue=%23b7cdd4&clientId=u64916657-1bd1-4&from=paste&height=850&id=ue1c83cf9&name=image.png&originHeight=1487&originWidth=2933&originalType=binary&ratio=1.75&rotation=0&showTitle=false&size=896108&status=done&style=none&taskId=u905692d3-caf9-4efe-88ac-37d4fad5270&title=&width=1676)
![image.png](https://cdn.nlark.com/yuque/0/2023/png/25611084/1681372483588-41626367-215b-4eba-b21e-bd5f6083577d.png#averageHue=%23f3f5f7&clientId=uece46559-ca7f-4&from=paste&height=284&id=ub64c79bb&name=image.png&originHeight=355&originWidth=504&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=40293&status=done&style=none&taskId=udabd8943-d4af-4f38-94ca-6c3b8a7c758&title=&width=403.2)
### 2.3 登录注册

- 实现**多账号**的注册、登录、退出登录，**账号密码式，不要求短信登陆**
- 登录后可进入个人主页

**个人主页**

   - 基本页面布局+样式
   - 点击投稿按钮上传视频文件（视频自找），选择好视频文件上传后弹出要求输入视频标题的模态框，输入完点击确认后可在作品栏显示并可以点击播放（点击后不用跳转页面，直接上传文件即可）这个不用刷新保存（首页不用实现这个功能，实现样式即可）
![image.png](https://cdn.nlark.com/yuque/0/2023/png/25611084/1680880707360-50266029-7a3d-4a40-bc83-71044be2747a.png#averageHue=%23b8d3af&clientId=u971de8b8-c951-4&from=paste&height=74&id=u8291f56c&name=image.png&originHeight=130&originWidth=371&originalType=binary&ratio=1.75&rotation=0&showTitle=false&size=8089&status=done&style=none&taskId=ud02cf773-a2ea-4c67-b13a-1a126b83fe1&title=&width=212)
   - 收藏的作品实现按UP主或视频标题模糊搜索，实现按收藏数、收藏日期（最近收藏）和视频时长排序（PS：可以在收藏的视频下方加显示收藏数的字样）
![image.png](https://cdn.nlark.com/yuque/0/2023/png/25611084/1681372205375-3efb63ee-47f5-41c7-a4fc-6544f83b9685.png#averageHue=%236f6c43&clientId=uece46559-ca7f-4&from=paste&height=278&id=u01ae0da3&name=image.png&originHeight=347&originWidth=461&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=131010&status=done&style=none&taskId=ub2ffe064-0850-4745-aaed-0e6380d5a0e&title=&width=368.8)
   - 更换头像功能，点击头像直接选择文件上传更换头像（只支持和你们名字拼音缩写相同的用户名账号，所以实现一个账号的更换头像功能即可，其他账号的头像可自找），详情请看 API 文档（进阶）
   - 实现收藏夹功能（新建收藏夹，编辑收藏夹（设置收藏夹名称以及设置公开状态），删除收藏夹，拖拽收藏夹更换顺序）（进阶）
- 实现 刷新 页面后该账号仍然登录，个人主页收藏的视频以及所有视频的播放量，弹幕数，点赞数，投币数，收藏数，评论以及该评论的回复和点赞数仍然还在（进阶）
### 2.4 终极需求

- 实现 Bilibili 网页版（内测版）的其他功能
- 根据自己的一些想法来进行优化，期待师弟师妹优秀的用户交互与设计

**提示：所有页面刷新不丢失数据的需求可用 localStorage 实现**
## 3. 考核 API 说明

1. 获取首页视频

请求URL

- `https://frontend.exam.aliyun.topviewclub.cn/api/getHomePageVideo`

请求方式

- GET

Query 请求参数

- 无

返回参数格式 `JSON`（最外层结构为：`Object`）

- 参数名：`data` 类型：`[object]` 必含：`是` 说明：返回的视频列表信息
| 参数名 | 类型 | 必含 | 说明 |
| --- | --- | --- | --- |
| videoSrc | [string] | 是 | 视频 |
| authorAvatarSrc | [string] | 是 | 视频UP主头像 |
| author | [string] | 是 | 视频UP主 |
| title | [string] | 是 | 视频标题 |
| describe | [string] | 是 | 视频简介 |
| uuid | [string] | 是 | 视频id |

2. 获取头像

请求URL

- `https://frontend.exam.aliyun.topviewclub.cn/api/getAvatar`

请求方式

- POST

Query 请求参数

| 参数名 | 类型 | 必填 | 说明 |
| --- | --- | --- | --- |
| username | [string] | 是 | UP主昵称 |

返回参数格式`blob`

3. 更换头像

请求URL

- `https://frontend.exam.aliyun.topviewclub.cn/api/changeAvatar`

请求方式

- POST

Query 请求参数 格式：Form-data

| 参数名 | 类型 | 必填 | 说明 |
| --- | --- | --- | --- |
| avatarFile | File | 是 | 头像图片 |
| username | string | 是 | UP主昵称 |

返回参数格式 JSON（最外层结构为：Object）

| 参数名 | 类型 | 必含 | 说明 |
| --- | --- | --- | --- |
| message | [string] | 是 | 状态信息 |

测试接口建议下载 `postman` 进行测试
网页版（[点此访问](https://www.postman.com/)）
应用版（[下载地址](https://www.postman.com/downloads/)）
## 4. 考核注意事项

- **考核时间： 4.15 00:00 至 5.17 23:29**
- **考核作品不允许使用任何框架，也不允许使用** `JQuery` **和** `axios` **，请使用原生的** `xhr` **进行** ajax **请求**（如果觉得已经掌握了 **ajax** 和 **ES6** 的 **promise** 可用 **fetch**）
- 考核期间通过 Git 提交你们的代码，平时在 dev 上开发。以合并到 master 分支上一次视为一次提交，最多可合并到 master 分支上三次（即三次提交）。超过三次合并的以最后一次合并的代码为准。前两次合并到 master 分支上的代码，师兄师姐会给予反馈。
- 项目可以有多个html文件，页面该怎么切换请参考 Bilibili 官网
- 考核期间第一周和第三周, 周四**[4.20，5.4]**晚上22:00通过提 issue 撰写周记。
- 考核期间第二周周四**[4.27]**晚分享会。
## 5. 资源及建议

- [MDN 网址](https://developer.mozilla.org/zh-CN/)
- 巧用搜索引擎
- 一物换一物、demo 换技术
- 如果对考核茫然，可以先学习 JS 以及 ajax 请求的内容，但是要注意时间的有限；然后对考核的内容**捋一遍思路与逻辑**，什么功能该做什么，dom 元素应该怎么展示，接口什么时候请求，请求什么，数据应该怎么走；对考核作品多思考，规定好计划，相信各位师弟师妹们都能做出优秀的作品，加油捏👍

