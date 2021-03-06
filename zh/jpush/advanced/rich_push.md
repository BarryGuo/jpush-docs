# Rich Push 开发指南

### 概述

Rich Push，即富媒体推送，允许开发者推送 Web 页面、图片、声音等除普通文本之外更丰富的内容。

应用开发者可以利用“富文本推送”功能推送如新闻、优惠券、活动信息等更加丰富的内容，也可以使用“富媒体文件推送” 使已有的 IM 类沟通功能得到扩展。

JPush 从终端用户使用体验的角度出发，充分考虑到国内的网络环境特点，Rich Push 功能上做了些特别的设计：    
1）Portal 上准备资源时，都保存到 JPush 的服务器上；    
2）JPush SDK 展示推送前预加载媒体文件。    
这样保证了一个富文本推送页面展示时是一定可见的、完整的。    


### 功能说明

功能上分为信息流模板推送和 URL 富媒体链接推送二个部分。详细使用，请参考文档[富媒体推送](../guideline/intro/#rich_push)


#### 信息流模板推送

+ 推送 Web 页面（富文本）
+ Portal 上提供推送工具，来快捷地创建富文本页面
+ 富文本作为通知推送到客户端
+ 客户端点击通知，自动展示该富文本页面


#### URL推送

+ 推送页面的 URL，点击通知栏消息后跳转 URL 指定的页面。

### 开发步骤

#### 下载支持 Rich Push 的 JPush Android SDK

+ 根据相关文档集成到 Android App 里
+ 手动集成需将压缩包 res 中的资源放到项目的对应文件夹，并按照示例 AndroidManifest 配置 PushActivity 组件
+ Android 6.0 以上需要申请动态权限 WRITE_EXTERNAL_STORAGE，请参考[申请权限接口](../client/Android/android_api/#android-60)


### SDK 支持

Rich Push 需要相应 SDK 版本配合支持

+ JPush Android SDK 1.8.0 及以上
+ JPush iOS SDK（暂不支持）


