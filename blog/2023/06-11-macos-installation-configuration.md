---
slug: 2023-06-11-macos-installation-configuration
title: macOS 装机配置
authors: [abangfundi]
tags: [macOS]
---

上次（2023.06.07）说了自己重新在 MacBook Pro 2015 上重新安装了 macOS 10.15 ，所以又重新折腾了一番

作为一个程序员我的 macOS 配置还是比较简单的，网上有比较多的教程是 `iTerm2 oh-my-zsh Powerlevel10k` 等，配置出来会比较实用/花哨/美观/护眼等，大家可以上网搜索，然后根据自己的喜好来设置，这个后续我有时间，也会再完善，目前只能完成最基本的配置。

1. 第一步从 App Store 下载应用，这是最简单的，不会出什么幺蛾子，如果是新用户，下载一些必备的 app， 如果是老用户，点击左下角的用户名，进入的就是账户，里面最主要的内容就是 `Purchased` 你自己的已经安装过的 应用列表，从这里直接找到你之前用的软件是最快的。像我降级老版本 macOS，正常的 app 详情页安装时，提示系统不支持，（也只能？）在这里才能安装旧版本支持当前系统的软件；从 App Store 安装的软件有
   * XCode
   * WeChat, QQ, QQMusic
   * Pages, Numbers, Keynote, The Unarchiver
   * OneDrive, OutLook
   * XMind
   * Sequel Ace (一款免费的 MySQL 客户端)
   * iShot 截图软件
   * Magnet 一键调整 App 窗口大小
   * Manico 一键打开/切换 App
2. [安装 Edge 浏览器](https://www.microsoft.com/en-us/edge/download)
3. [安装 iTerm](https://iterm2.com)  下载解压后拖进 `/Applications`
4. Command Line Tools for Xcode 在 iTerm 中执行 `xcode-select --install` （可选，下一步安装 HomeBrew 的过程中，也会安装 Command Line Tools for Xcode）
5. [安装 HomeBrew](https://brew.sh/)
6. 然后使用brew 安装必要的开发软件
   1. `brew install python python@3.10 python@3.8` ...安装自己需要的版本
   2. `brew install go go@1.19 go@1.18` ...安装自己需要的版本
   3. `brew install node@18 node@16` ...安装自己需要的版本
   4. `brew install ruby@2.7` ...安装自己需要的版本
   5. `brew install git`   一般就是最新版
7. [安装 Oh My ZSH](https://ohmyz.sh/)
8. [安装 VSCode](https://code.visualstudio.com/download) 下载解压后拖进 `/Applications`
9. 安装 git 可视化工具： [GitUp](https://gitup.co/)  或者 [SourceTree](https://www.sourcetreeapp.com) 等，下载解压后拖进 `/Applications`
10. 配置 git alias 别名，已然习惯了缩写 `g s`, `g c` 等，[参考](https://github.com/GitAlias/gitalias)

差不多就这些，比较基础，没有啥花里胡哨的，以后再补充。

顺便说一下我对于盗版软件的看法

作为一个 software developer ，不希望自己的软件被盗用、网站被攻击，将心比心，我也是别人的劳动成果的。
很久以前确实使用过一些盗版软件，比如盗版Windows、VC6.0、AutoCAD 等，这些大型软件实在也买不起，用的也不多；后来（毕业后吧）所有软件都是有授权才使用的，免费或者付费购买的。
我感觉部分付费软件定价超过了它本身的价值，虽然不爽，但是我尊重人家的劳动成功、定价和版权，大不了就不用呗。
比如 JetBrains 全家桶, Adobe PhotoShop, Navicat 等；
使用替代方案就是 VSCode, Pixelmator Pro, Sequel Ace, DBeaver 等。

就这样

Peace And Love.
