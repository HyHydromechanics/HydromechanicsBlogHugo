---
title: "Hugo_Deploy"
date: 2022-07-15T18:05:48+08:00
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
# Hugo博客的部署

 - 这部分需要使用到一个叫做github page的东西，是GitHub提供的一个网页寄存服务，可以寄存静态页面，这个特性就特别适合博客的搭建。

首 - 先再Github上创建一个 Repository，命名为Github名字.http://github.io，譬如我的仓库caecarxu.github.io，这样就可以生成一个用户页面

 - 在hugo server调式页面完成后，使用命令hugo生成hugo静态页面。

```yml
baseURL = "https://caecarxu.github.io/"
hugo  
```

 - 在命令执行后，出现一个public文件夹，里面就是网站的静态页面文件

 - 进入public文件夹，使用git上传文件

```dos
cd public
git init    ##初始化仓库
git remote add origin https://github.com/<你的用户名>/<你的仓库名字>.git    ##链接远程仓库
git add .
git commit -m "first commit"
git push -u origin master
```

 - 在此之后更新文章，使用hugo生成新的静态页面，并使用git push进行同步



```dos
cd public
git add .
git status
git commit -m "你想提交的信息"
git push
```

### 或者

```dos
hugo --theme=PaperMod --baseUrl="https://HyHydromechanics.github.io" --buildDrafts
```
在创建public文件夹后:
1. 进入public文件夹: git init
2. git add .
3. git commit -m "aggdwyf"
4. git remote add origin https://github.com/HyHydromechanics/HyHydromechanics.github.io.git
5. git push -u origin master

到第五步可能会让你输入username和密码, 但是注意, 密码不是你注册的那个密码, 而是token, 需要去另外注册一个

g