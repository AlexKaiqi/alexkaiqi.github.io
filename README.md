## 自己写的一款jekyll博客主题

使用bootstrap4 和 sass

参考了一些其它博客样式

适合喜欢自己折腾的, bootstrap布局起来还是很方便的

## 效果


## 功能介绍

集成了一些方便的功能

- 自动适应不同设备
- 简单的搜索, 可通过标题, 标签, 内容进行搜索
- 自动生成博客目录, 固定于右侧, 方便阅览
- disqus 讨论 

## 使用

    cd {博客路径}
    bundle install (可能花些时间)
    bundle exec jekyll serve (启动)
    
## 配置

多数配置只需要通过修改`_config.yml`文件即可.
具体可参考网上教程


## 样式修改

样式文件存放于`_sass/`以及`assets/css/`目录中.

在`_sass`中新增样式文件时, 注意在`assets/css/style.css`中导入.

## 艺术字生成

先使用在线工具生成艺术字, 然后
[去除背景](https://onlinepngtools.com/create-transparent-png)

## 其它

我不大清楚对搜索引擎的优化, 这部分是从其它模仿博客主题的, 
如果对此有要求, 可能需要自己动手调整.

