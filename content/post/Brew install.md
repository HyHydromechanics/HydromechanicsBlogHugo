---
title: "Brew的下载"
date: 2022-07-15T16:25:03+08:00
draft: true
# weight: 1
# aliases: ["/first"]
tags: ["brew"]
author: "Me"
# author: ["Me", "You"] # multiple authors
showToc: true
TocOpen: false
draft: false
hidemeta: false
comments: false
description: "brew installation"
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
# **Brew的下载与配置**

### Homebrew国内源

[知乎文章地址：https://zhuanlan.zhihu.com/p/111014448](https://gitee.com/link?target=https%3A%2F%2Fzhuanlan.zhihu.com%2Fp%2F111014448)

- 苹果电脑标准安装脚本：（推荐 优点全面 缺点慢一点）

  ```
  /bin/zsh -c "$(curl -fsSL https://gitee.com/cunkai/HomebrewCN/raw/master/Homebrew.sh)"
  ```

- 苹果电脑极速安装脚本：（优点安装速度快 缺点update功能需要命令修复 ）

  ```
  /bin/zsh -c "$(curl -fsSL https://gitee.com/cunkai/HomebrewCN/raw/master/Homebrew.sh)" speed
  ```

- Linux 标准安装脚本：

  ```
  rm Homebrew.sh ; wget https://gitee.com/cunkai/HomebrewCN/raw/master/Homebrew.sh ; bash Homebrew.sh
  ```

- 苹果电脑卸载脚本：

  ```
  /bin/zsh -c "$(curl -fsSL https://gitee.com/cunkai/HomebrewCN/raw/master/HomebrewUninstall.sh)"
  ```

- Linux卸载脚本：

- ```
  rm HomebrewUninstall.sh ; wget https://gitee.com/cunkai/HomebrewCN/raw/master/HomebrewUninstall.sh ; bash HomebrewUninstall.sh
  ```

  

**---Brew介绍**

macOS 和 Linux 缺失软件包的管理器

**---Homebrew 能干什么?**

使用 Homebrew 安装 Mac（或Linux）没有预装但你需要的东西。

**--Homebrew自身如何使用**

知道软件包具体名称，直接 `brew install 软件包名` 只知道一小部分名称，用 `brew search 小部分名称` 查询即可 例如`brew search chrome`就会把带chrome的软件包全部列出

> 如果遇见任何问题, 直接卸载后重新安装, 大概率是之前安装的缓冲与现在安装的相互影响

