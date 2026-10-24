---
title: PCL2 解除下载限制
date: 2026-10-24 16:30:00
keywords: PCL-Unlock-Download
tags: Tutorial
categories: Tools
top_img: img/default-top-bg.jpg
copyright_author: https://github.com/tooplick
copyright_author_href: https://github.com/tooplick
copyright_url: https://ygking.top/PCL-Unlock-Download/
---

# PCL2 解除下载限制

## 背景

PCL2（Plain Craft Launcher 2）是一款广受欢迎的 Minecraft 启动器。

自 v2.99.0.0 起，PCL 内置了 Minecraft 下载功能限制，新版本无法正常下载游戏本体。

如果你也遇到了这个问题，有两种解决方法：

1. **保留新版，用补丁工具解除限制**
2. **换回 v2.14.0.0 及更早的历史版本**

本站已经整理了官方历史版本的[下载页](https://ygking.top/pcl/)（共 7 个版本 + 补丁工具），两种方法用到的文件都可以在那里找到。

## 方法一：使用补丁工具解除

补丁工具名为 **PCL Download Patch**，由本人开源。它直接修改官方原版 exe 中与下载限制相关的代码，不需要安装任何依赖。

### 1. 下载补丁工具

获取网址：[https://ygking.top/pcl/](https://ygking.top/pcl/)

也可以使用下面的直链（经 gh-proxy.org 加速）：

- [PCL Download Patch.exe](https://gh-proxy.org/https://raw.githubusercontent.com/tooplick/pcl2/main/PCL%20Download%20Patch.exe)（加速下载）
- [源码仓库](https://github.com/tooplick/pcl2)

### 2. 准备官方 PCL

补丁作用于**官方原版 exe**，版本 v2.99.0.0 及以上：

- 已经在用新版 PCL 的，直接用它现有的 exe 即可
- 还没有的也可以选择到[下载页](https://ygking.top/pcl/)下载

> Tips:
>
> 下载页的所有安装包均取自 PCL 官方仓库的历史提交，原样存档、未做任何修改

### 3. 打补丁

1. 双击运行 `PCL Download Patch.exe`
2. 把 PCL 的 exe 拖进工具窗口（或点击中央卡片选择文件）

提示成功后，用这个 exe 正常启动 PCL，下载功能就恢复了。

### 补丁原理简述

补丁工具基于 Mono.Cecil 对 exe 做 IL 级别的模式匹配修改，只动下载限制相关的代码，其余部分保持原样。

## 方法二：使用历史版本

下载限制是 v2.99.0.0 才引入的，**v2.14.0.0 及更早版本本身不存在这个限制**，不需要打任何补丁。

操作很简单：

1. 打开本站[下载页](https://ygking.top/pcl/)
2. 推荐选择 **v2.14.0.0**（这是是最后一个无限制的版本）
3. 下载后直接双击运行即可

> Tips:
>
> 旧版本首次打开需要断网并关闭自动更新。否则可能被自动更新到 v2.99.0.0+，下载限制会随之回来。


## 分发许可

PCL 的复制与分发遵循《PCL 分发有限许可》，补丁后的 exe 自行使用，请不要用于商业用途。

## 相关链接

- PCL2 下载页：[https://ygking.top/pcl](https://ygking.top/pcl/)
- 补丁工具源码：[https://github.com/tooplick/pcl2](https://github.com/tooplick/pcl2)
- PCL 官方仓库：[https://github.com/Meloong-Git/PCL](https://github.com/Meloong-Git/PCL)
- 《PCL 分发有限许可》：[https://github.com/Meloong-Git/PCL/blob/main/LICENCE](https://github.com/Meloong-Git/PCL/blob/main/LICENCE)

