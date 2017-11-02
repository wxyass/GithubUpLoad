---
title: OSS域名绑定
date: 2017-06-28 11:17:49
tags: [OSS]
categories: [OSS]
---

在存储空间上传对象(图片、视频等)后，可获取的对象的url地址,url地址由两个部分组成：OSS 域名地址和对象文件名。
为了避免业务中可能涉及的跨域或者安全问题，建议您使用自定义域名方式访问OSS；
域名绑定成功后，为了使用域名正常访问 OSS，还需要添加 CNAME 记录指向存储空间对应的外网域名。

您绑定的域名需在工信部备案，否则域名访问将会受到影响。
每个存储空间最多可以绑定 20 个域名。
自定义域名绑定成功后，您 OSS 中存储文件的访问地址会使用自定义域名。

<!--more-->

OSS域名绑定详情如下:

#### 1 登录阿里云OSS控制台, 打开控制台
链接<https://www.aliyun.com/product/oss>

![0628](http://images.wxyass.com/wxyass/images/20170628112230.png)

#### 2 选择欲绑定Bucket, 打开Bucket属性,添加域名

![0628](http://images.wxyass.com/wxyass/images/20170628101241.png)

#### 2  输入要绑定的域名, 注意添加前缀oss.(另外域名要提前备案)

![0628](http://images.wxyass.com/wxyass/images/20170628101049.png)

#### 3 手动添加,然后确定

![0628](http://images.wxyass.com/wxyass/images/20170628101353.png)

#### 4 复制外网域名, 将会作为记录值添加到域名解析

![0628](http://images.wxyass.com/wxyass/images/20170628101734.png)

#### 5 到域名商添加解析

![0628](http://images.wxyass.com/wxyass/images/20170628101644.png)

#### 6 绑定成功,测试一下.

<http://wxyass-com.oss-cn-beijing.aliyuncs.com/wxyass/images/20170622141857.png>

<http://oss.wxyass.com/wxyass/images/20170622141857.png>


