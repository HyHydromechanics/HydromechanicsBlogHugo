---
title: "Hugo的创建"
date: 2022-07-15T17:43:21+08:00
draft: true
# weight: 1
# aliases: ["/first"]
tags: ["blog"]
author: "Me"
# author: ["Me", "You"] # multiple authors
showToc: true
TocOpen: false
draft: false
hidemeta: false
comments: false
description: "Blog set up"
canonicalURL: "https://canonical.url/to/page"
disableHLJS: true # to disable highlightjs
disableShare: false
disableHLJS: false
hideSummary: false
searchHidden: true
ShowReadingTime: true
ShowBreadCrumbs: true
ShowPostNavLinks: true
ShowWordCount: true
ShowRssButtonInSectionTermList: true
UseHugoToc: true
cover:
    image: "<image path/url>" # image path/url
    alt: "<alt text>" # alt text
    caption: "<text>" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: true # only hide on current single page
editPost:
    URL: "https://github.com/<path_to_repo>/content"
    Text: "Suggest Changes" # edit text
    appendFilePath: true # to append file path to Edit link
---
# **Hugo Blog 创建**

### 下载:
这里用mac做例子, 使用来进行下载

```dos
brew install hugo
```
> brew的具体下载可以看另外一篇文章

Hugo官网: [https://www.gohugo.cn/](https://www.gohugo.cn/)

> windows可以直接去官网下载安装包

安装结束后输入:

```dos
hugo version
```

如果返回:

```dos
hugo v0.101.0+extended darwin/arm64 BuildDate=unknown
# 版本号不一样没事
```

则安装完成

# 初始化blog site

终端中输入:
```dos
hugo new site <name of your blog>
```

此时进入blog根目录, 可以看到以及生产了部分文件夹:

![截屏2022-07-15 17.50.29](./pic/%E6%88%AA%E5%B1%8F2022-07-15%2017.50.29.png)

# 添加主题:

1. 访问[themes.gohugo.io](https://themes.gohugo.io)来获取并查看可用的主题列表 (笔者使用的是papermode主题)
2. 每个主题都写好了对应的安装步骤, 对应步骤一步一步来就好(需要使用git来clone主题包)
3. 随后, 在`config.yml`中添加主题的配置信息: 

```
theme = <your theme>
```

# 填写内容
你可以在content中自己创建markdown文件并且自行加入metadata来工作, 但是笔者在这里更推荐使用new命令来辅助
```dos
hugo new posts/your-fist-post.md
```

新创建的文件会自动带上标题, 日期, 以及draft的true/false

# 启动服务器

```dos
hugo sever -t <your-theme-name> --buildDrafts
```

随后, 你就可以去[https://localhosts:1313](https://localhosts:1313)来访问你的博客了

# 自定义主题文件:
根据自己的需求更改config.yml文件
这里大家就按照自己的喜好来随便更改啦


