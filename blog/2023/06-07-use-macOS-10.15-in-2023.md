---
slug: 2023-06-07-use-macOS-10.15-in-2023
title: 在 2023 年又重新用上 macOS 10.15
authors: [abangfundi]
tags: [macOS]
---

今天是2023年06月07日，高考的日子，祝天下所有的考生考试顺利～～

2015年买的 MacBook Pro 15 英寸，本来想装一个 Windows 系统做备用机，但实在用不习惯了，感觉也没什么用处，装回了 macOS ，但是记得之前用macOS 11 or 12 感觉有点儿卡，所以这次装回了 macOS 10.15 Catalina，用起来感觉还不错。

<!-- truncate -->

* 操作很流畅，比 macOS 11 或 12 更流畅，发热也轻一些，电池也更耐用
* 风格也还行，比较喜欢的小圆角设计，从 Big Sur 开始的圆角有些太大了
* 新的软件版本有一些不支持了，不过从 App Store 的购买记录里，可以下载历史版本
* 而没上架应用商店的第三方 app 一般都是支持10.15的，所以问题不大
* 除了做 iOS/macOS 等 app 开发的需求不太能满足，其他的开发 web、后端开发都能满足

目前感觉唯一的缺憾是 `HomeBrew`，每次使用都会提示

```bash
Warning: You are using macOS 10.15.
We (and Apple) do not provide support for this old version.
It is expected behaviour that some formulae will fail to build in this old version.
It is expected behaviour that Homebrew will be buggy and slow.
Do not create any issues about this on Homebrew's GitHub repositories.
Do not create any issues even if you think this message is unrelated.
Any opened issues will be immediately closed without response.
Do not ask for help from Homebrew or its maintainers on social media.
You may ask for help in Homebrew's discussions but are unlikely to receive a response.
Try to figure out the problem yourself and submit a fix as a pull request.
We will review it but may or may not accept it.
```

然后按照应用的时候，都会在本地编译构建安装，着实费时，也让电脑发热严重。比如，安装个 `Node.js`，耗时一个多小时

或许这能治好我乱装东西的毛病，也挺好🤣

```bash
$ brew install node@18

...

==> Fetching dependencies for node@18: python@3.11, brotli, cmake, c-ares, icu4c, libnghttp2, m4, autoconf, automake, libtool, docutils, pygments, sphinx-doc and libuv

...
/usr/local/Cellar/python@3.11/3.11.3:  8121 files, 193.6MB,     built in 11 minutes 24 seconds
/usr/local/Cellar/cmake/3.26.4:  3188 files, 50.3MB,            built in 12 minutes 27 seconds
/usr/local/Cellar/c-ares/1.19.1: 87 files, 661.4KB,             built in  0 minutes 31 seconds
/usr/local/Cellar/icu4c/72.1: 263 files, 78MB,                  built in  3 minutes
/usr/local/Cellar/libnghttp2/1.53.0: 13 files, 720.9KB,         built in  0 minutes 27 seconds
/usr/local/Cellar/sphinx-doc/7.0.1:  4019 files, 70.3MB,        built in  5 minutes 55 seconds
/usr/local/Cellar/libuv/1.45.0: 47 files, 3MB,                  built in  0 minutes 30 seconds
/usr/local/Cellar/node@18/18.16.0:  2341 files, 56MB,           built in 35 minutes 34 seconds

```
