KuGouMusic API

酷狗音乐 NodeJS 版 API

## 灵感来自

[Binaryify/NeteaseCloudMusicApi](https://github.com/Binaryify/NeteaseCloudMusicApi)

## 工作原理

跨站请求伪造 (CSRF), 伪造请求头 , 调用官方 API

## 免责声明

> 1. 本项目仅供学习使用，请尊重版权，请勿利用此项目从事商业行为及非法用途!
> 2. 使用本项目的过程中可能会产生版权数据。对于这些版权数据，本项目不拥有它们的所有权。为了避免侵权，使用者务必在 24 小时内清除使用本项目的过程中所产
>    生的版权数据。
> 3. 由于使用本项目产生的包括由于本协议或由于使用或无法使用本项目而引起的任何性质的任何直接、间接、特殊、偶然或结果性损害（包括但不限于因商誉损失、停
>    工、计算机故障或故障引起的损害赔偿，或任何及所有其他商业损害或损失）由使用者负责。
> 4. **禁止在违反当地法律法规的情况下使用本项目。** 对于使用者在明知或不知当地法律法规不允许的情况下使用本项目所造成的任何违法违规行为由使用者承担，本
>    项目不承担由此造成的任何直接、间接、特殊、偶然或结果性责任。
> 5. 音乐平台不易，请尊重版权，支持正版。
> 6. 本项目仅用于对技术可行性的探索及研究，不接受任何商业（包括但不限于广告等）合作及捐赠。
> 7. 如果官方音乐平台觉得本项目不妥，可联系本项目更改或移除。

### 安装

```shell
$ git clone git@github.com:MakcRe/KuGouMusicApi.git
$ cd KuGouMusicApi
$ npm install
```

### 运行

```shell
$ npm run dev
```

### 使用接口为概念版

> 复制 .env.example 为 .env，并且把里面的 `platform` 改为 lite

服务器启动默认端口为 3000, 若不想使用 3000 端口 , 可使用以下命令 : Mac/Linux

```shell
$ PORT=4000 npm run dev
```

windows 下使用 git-bash 或者 cmder 等终端执行以下命令 :

```shell
$ set PORT=4000 && npm run dev
```

windows 下使用 PowerShell 等终端执行以下命令 :

```shell
$ $Env:PORT=4000; npm run dev
```

服务器启动默认 host 为 localhost,如果需要更改, 可使用以下命令 : Mac/Linux

```shell
$ HOST=127.0.0.1 npm run dev
```

windows 下使用 git-bash 或者 cmder 等终端执行以下命令 :

```shell
$ set HOST=127.0.0.1 && npm run dev
```

windows 下使用 PowerShell 等终端执行以下命令 :

```shell
$ $Env:HOST=127.0.0.1; npm run dev
```

## Vercel 部署

### 操作方法

1. fork 此项目
2. 在 Vercel 官网点击 `New Project`
3. 点击 `Import Git Repository` 并选择你 fork 的此项目并点击 `import`
4. 点击 `PERSONAL ACCOUNT` 的 `select`
5. 直接点 `Continue`
6. 若需要部署版本为概念版（不需要该步骤可以跳过），在 `Environment Variables` 添加 `key` 为 platform，`Value (Will Be Encrypted)` 为 然后点击 `Add`
7. `PROJECT NAME`自己填,`FRAMEWORK PRESET` 选 `Other` 然后直接点 `Deploy` 接着等部署完成即可

## 功能特性

### 不同版本的平台的 token 是不通用的。

1. 登录
2. 刷新登录
3. 发送验证码
4. dfid 获取
5. 获取用户歌单
6. 获取用户最近听歌历史
7. 收藏歌单
8. 取消收藏歌单
9. 对歌单添加歌曲
10. 对歌单删除歌曲
11. 新碟上架
12. 专辑信息
13. 专辑详情
14. 专辑音乐列表
15. 获取音乐 URL
16. 获取歌曲高潮部分
17. 搜索
18. 综合搜索
19. 热搜列表
20. 歌词搜索
21. 获取歌词
22. 歌单分类
23. 歌单
24. 主题歌单
25. 音效歌单
26. 获取歌单详情
27. 获取歌单所有歌曲
28. 获取歌单所有歌曲（新版）
29. 获取主题歌单所有歌曲
30. 获取主题音乐
31. 获取主题音乐详情
32. 歌曲推荐
33. 获取歌手和专辑图片
34. 获取歌手图片
35. 获取音乐相关信息
36. 获取音乐详情
37. 获取音乐专辑/歌手信息
38. 私人 FM(对应手机和 pc 端的猜你喜欢)
39. banner
40. 乐库 banner
41. 乐库电台
42. 乐库
43. 推荐频道
44. 频道
45. 频道图片
46. 频道歌曲
47. 编辑精选
48. 编辑精选数据
49. 编辑精选歌单
50. 编辑精选专区
51. 编辑精选专区详情
52. 领取 VIP（需要登陆，该接口为测试接口）
53. 获取歌手详情
54. 获取歌手专辑
55. 获取歌手单曲
56. 获取歌手 MV
57. 获取视频 url
58. 获取视频相关信息
59. 获取视频详情
60. 新歌速递
61. 场景音乐列表
62. 场景音乐详情
63. 获取场景音乐讨论区
64. 获取场景音乐模块 Tag
65. 获取场景音乐歌单列表
66. 获取场景音乐视频列表
67. 获取场景音乐音乐列表
68. 每日推荐
69. 历史推荐
70. 风格推荐
71. 排行列表
72. 排行榜推荐列表
73. 排行榜往期列表
74. 排行榜信息
75. 排行榜歌曲列表
76. 歌曲评论
77. 歌曲评论-根据分类返回
78. 歌曲评论-根据热词返回
79. 楼层评论
80. 歌单评论
81. 专辑评论

## License

[The MIT License (MIT)](https://github.com/MakcRe/KuGouMusicApi/blob/main/LICENSE)
