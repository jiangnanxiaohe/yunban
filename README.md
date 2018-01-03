基于NodeJs搭建的云瓣影音网站&微信端
网页端效果:
电影界面演示、音乐界面演示，或者可以访问在线地址(送的云主机，自然有些卡)

微信端效果:
用微信扫二维码可以看效果(但测试号只能有100个人关注的限制~)
效果展示  效果展示  效果展示
效果展示  效果展示效果展示
简介:

1. pc端后端搭建:

使用NodeJs的koa框架并使用了部分ES6特性完成云瓣网站后端的搭建;
使用mongodb完成数据存储,通过mongoose模块完成对mongodb数据的构建;
使用jade模板引擎完成页面创建渲染;
使用Moment.js格式化电影存储时间;

2. 项目前端搭建:

使用jQuery和Bootsrap完成网站前端JS脚本和样式处理;
使用Sass完成云瓣项目的样式编写;
使用validate.js完成对账号登录注册的判断;
使用fullpage.js完成电影宣传页面制作;
前后端的数据请求交互通过Ajax完成;
(音乐端部分模块、电影画廊部分)使用React+ES6进行组件化开发，并使用Webpack实现资源模块管理
使用canvas并调用webAudio api完成音乐播放界面的制作


3. 项目微信端搭建

使用weui框架构造详情界面
多种api接口的实现（比如地理经纬度查询、拍照、扫码、上传素材等）
调用jdk，实现语音查询电影


4. 本地开发环境搭建:

使用gulp集成jshint对JS语法检查，Sass文件编译、压缩等功能，使用mocha完成用户注册存储等步骤的简单单元测试，以及服务器的自动重启等功能。


5. 一些功能模块:


电影首页(实现了按热度、时间、评价、分类查询以及加载更多等功能模块)
部分页面针对不同分辨率做了自适应；
具有用户注册登录及管理;
电影画廊页面的实现(数据从后台获得)；
音乐播放界面实现(数据从后台获得)；
电影（音乐）可进行叠楼评论并可删除自己的评论(管理员能删除任何人);
电影（音乐）及电影院信息录入和搜索;
电影（音乐）分类添加及删除;
电影（音乐）与所属分类都是一对多的关系；
电影（音乐）海报自定义上传;
电影（音乐）可以自行上传;
列表分页处理，访客统计;
微信上通过语音或文字搜电影;
微信上实现与网页的评论同步;
微信上能访问网页端；(并把电影画廊和音乐播放作为单独的菜单独立出来)
项目页面:
电影界面:

电影宣传页:localhost:1234
电影首页:localhost:1234/movieIndex
电影画廊:localhost:1234/gallery
电影详情页:localhost:1234/movie/:id
电影搜索页:localhost:1234/movie/results?q=xx
音乐界面:

音乐首页:localhost:1234/musicIndex
音乐详情页:localhost:1234/music/:id
音乐播放界面:localhost:1234/musicPlay
音乐搜索页:localhost:1234/music/results?q=xx
用户后台页:

用户注册页面: localhost:1234/signup
用户登陆页面: localhost:1234/signin
用户详情列表页: localhost:1234/admin/user/list
电影后台页:

后台录入页:localhost:1234/admin/movie/new
列表页:localhost:1234/admin/movie/list
分类录入页:localhost:1234/admin//movie/category/new
分类页:localhost:1234/admin/movie/category/list
电影院录入页:localhost:1234/admin/city/new
电影院列表页:localhost:1234/admin/city/list
音乐后台页:

后台录入页:localhost:1234/admin/music/new
列表页:localhost:1234/admin/music/list
分类录入页:localhost:1234/admin/music/category/new
分类列表页:loclahost:1234/admin/music/category/list
热门榜单列表页:localhost:1234/admin/music/programme/list
微信界面

猜猜电影页：/wechat/movie
微信电影界面: /wechat/movie/:id
微信音乐界面：/wechat/music/:id
todo：
 后台管理界面待优化；
 增加云瓣的app端;
