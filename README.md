# Mac_CPP_Developer

## Table of Contents

1. [macOS](#1-macos)

   - [功能键](#功能键)
   - [其他快捷键](#其他快捷键)
   - [设置 Trackpad 轻点来点按](#设置-trackpad-轻点来点按)
   - [词典](#词典)
   - [Dock Position](#dock-position)
   - [Remove Dock icons](#remove-dock-icons)
   - [三指拖动](#三指拖动)
   
2. [常用工具](#2-常用工具)

   - [Homebrew](#homebrew)
   - [Oh My Zsh](#oh-my-zsh)
   - [MacDown](#macdown)
  
   
3. [配置开发环境](#3-配置开发环境)
     
   - [XCode](#XCode)
   - [Qt5.15](#Qt5.15)
   - [Clion](#Clion)
   - [Java三件套](#Java三件套)
       - [SDK:AndroidStudio](#SDK:AndroidStudio)
       - [JDK:Java8](#JDK:Java8)
       - [NDK:从Qt配置](#NDK:从Qt配置)


## 1. macOS

本节介绍操作系统本身的一些设置。

### 功能键

默认情况下，F1-F12 都是特殊功能，比如调节屏幕亮度。而当你需要键入 F1-F12 时（比如在使用 IntelliJ IDEA 的快捷键时），需要同时按住 Fn。这对于开发人员来说是非常不方便的。

把 F1-F12 改成标准功能键：选择`System Preferences` > `Keyboard`，在`Keyboard`标签页中选中`Use F1, F2, etc. keys as standard function keys`。


### 其他快捷键

让双手尽量多的键盘和快捷键，少使用鼠标和触摸板，可以大大提高效率。

- [Mac keyboard shortcuts](https://support.apple.com/kb/HT201236)

  苹果官方文档。当你在写代码，怎么通过快捷键让光标转移到行首、行尾、向上翻页或者将光标移左移一个词？都在这篇文档里。

- [Mac keyboard shortcuts for accessibility features](https://support.apple.com/kb/HT204434)

  苹果官方文档。回车触发蓝底按钮，空格触发蓝边按钮，都出自这里。

### 设置 Trackpad 轻点来点按

默认情况下按下触摸板才是点按（click）。我喜欢设置成用轻点作为点按：

选择`System Preferences` > `Trackpad`，在`Point & Click`标签页中选中`Tap to click`。

### 词典

macOS 自带了词典（Dictionary）。你几乎可以在任何应用中通过重按触摸板来现实对应单词的释义。如果你更喜欢三指轻拍触摸板，可以在`System Preferences` > `Trackpad`，在`Point & Click`标签页中把`Look up & data detectors`改成`Tap with three fingers`。

也可以打开 Dictionary 应用来查找单词。

可以在 Dictionary 应用中添加英汉汉英词典。

### Dock Position

默认 Dock 在屏幕下方。我们的屏幕一般都是 16:10，Dock 在屏幕下方的话会占据本来就不大的垂直空间。建议把 Dock 放到右边或者左边。

选择`System Preferences` > `Sidecar`，在`Show Sidebar`中选择不同的位置。

### Remove Dock icons

默认情况下 Dock 被一堆系统自带的应用占据着，每个图标都会被挤得很小，我会把 Dock 上没用的图标都删掉。

### 三指拖动

我习惯于三指拖动窗口。设置方法：选择`System Preferences` > `Accessibility`，选中左边`Pointer Control`菜单，打开`Trackpad Options…`，选中`Enable dragging`和`three finger drag`。

## 2. 常用工具

本节介绍一些常用的，跟开发没有直接关系的第三方应用及其设置。

### [Homebrew](http://brew.sh)

包管理工具，官方称之为`The missing package manager for macOS`。

安装命令：
`/bin/zsh -c "$(curl -fsSL https://gitee.com/cunkai/HomebrewCN/raw/master/Homebrew.sh)"`。
PS:安装过程中，有任何问题可以查看：[Homebrew国内如何自动安装](https://zhuanlan.zhihu.com/p/111014448)

有了 Homebrew 以后，要下载工具，比如 git、Wget、Gradle、Maven 等工具，就不需要去网上下载了，只要一行命令就能搞定：

```sh
brew install git wget gradle maven
```

```
brew install --cask alfred sourcetree visual-studio-code
```


### [iTerm2](https://iterm2.com/)

iTerm2 是最常用的终端应用，是 Terminal 应用的替代品。提供了诸如`Split Panes`等[一群实用特性](https://iterm2.com/features.html)。它默认的黑色背景让我毫不犹豫的抛弃了 Terminal。

安装：[iterms](https://iterm2.com/downloads.html)

### [Oh My Zsh](http://ohmyz.sh)

默认的 Bash （Catalina 已经默认使用 Zsh）是黑白的，没有色彩。而 Oh My Zsh 可以带你进入彩色时代。Oh My Zsh 同时提供一套插件和工具，可以简化命令行操作。后面我们会看到很多介绍，你会看到我爱死这家伙了。

安装方法：。

### MacDown

MacDown 是 Markdown 编辑器。由于 Mou 一直不支持代码高亮，我就转向了 MacDown。完美支持 [GFM](https://help.github.com/articles/github-flavored-markdown/)。

我特别喜欢 [Markdown](https://daringfireball.net/projects/markdown/)，我用 Makdown 来写文章（包括本文），写幻灯片（[reveal.js](https://github.com/hakimel/reveal.js/)）。Markdown 可以让我专注于内容本身，而无需花精力在排版和样式上。

安装：[macdown](https://macdown.uranusjr.com)

安装显示按钮软件
`brew install --cask keycastr`

## 3. 配置开发环境
### XCode
从AppStore中安装

### [Qt5.15](https://www.qt.io/blog/qt-5.15-released)

### [Clion](https://www.jetbrains.com/clion/)

### Java三件套
#### SDK:[AndroidStudio](https://developer.android.google.cn/studio/)
#### JDK:Java8
`brew install --cask adoptopenjdk8`
#### NDK:从Qt配置
在Qt中创建一个项目，点击“设备”，选择“Android”，自动安装以下工具：

* cmdline-tools;latest
* build-tools;30.0.2
* ndk;21.3.6528147

## 参考资料

- [强迫症的 Mac 设置指南](https://github.com/macdao/ocds-guide-to-setting-up-mac#oh-my-zsh)
