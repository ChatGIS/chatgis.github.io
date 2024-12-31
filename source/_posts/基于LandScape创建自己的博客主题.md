---
title: Hexo-基于LandScape创建自己的博客主题
date: 2024-12-29 23:42:18
tags:
    - Hexo
---
## 1. 下载主题LandScape
```
git clone git@github.com:hexojs/hexo-theme-landscape.git themes/landscape
```
## 2. 管理主题源码
删除下载主题文件夹中的`.git`文件夹，并将主题文件夹重命名为`space`。  
这样就可以基于在自己的git管理新主题啦。

## 3. 调用主题space
在文件`_config.yml`中找到增加配置
```
theme: space
```
## 4. 修改Banner
直接找到主题中的`themes/space/source/css/images/banner.jpg`文件，替换为自己的图片即可，命名保持不变。
