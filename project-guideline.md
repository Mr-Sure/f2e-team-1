# 口袋高校前端团队项目规范：

## 本文档将由口袋高校前端团队全体成员持续修订  

    V-1.0.0  Date：2016.10.17

## 基础文件引入

* 原则上所有js/css/font等文件的引用路径均为static.pocketuniversity.cn 后期可解析出对应的京台服务器域名，进行CDN加速与前端开发调试。

* 注意：目前 images/css/font/js等静态文件引用路径为http://www.pocketuniversity.cn/static  路径下,以项目名/版本号/静态资源目录/详细名称作为索引。

* eg:http://www.pocketuniversity.cn/static/bangdan/1.0/js/manager/bundle.js 后期可在项目名下级加入版本号。

## PC 项目

* 原则上每个页面需引入 http://static.pocketuniversity.cn/base/css/1.0/reset.css 初始化样式（视项目而定，可选）。
  
## 微信-WebAPP项目
* meta 引用示例：

  <meta charset="UTF-8">
  <meta content="telephone=no" name="format-detection" />
  <meta content="yes" name="apple-mobile-web-app-capable" />
  <meta name="author" content="Sure" email="Sure@tuiyilin.com">
  <meta content="black" name="apple-mobile-web-app-status-bar-style" />
  <meta name="viewport" content="width=device-width,initial-scale=1,minimum-scale=1,maximum-scale=1,user-scalable=no">
	    
* 基本依据VueJS + Webpack项目规范,个别项目可灵活选取js库，基本原则：轻量。(可使用Zepto/JQuery等)。

* 所选框架需在index.html页面，通过CDN加速中作为全局引入，以减少WebPack编译负载（Vue模板文件编译后原则不超过100K）。

## 版本控制

  1.原则上之后所有前端文件均需在SVN做归档(内网：https://desktop-igt33re/svn/svnTest)。

  2.部分可使用Git的项目，在每次发布线上前需在SVN上进行提交。

  
