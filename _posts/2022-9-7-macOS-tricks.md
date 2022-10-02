---
layout:     post
title:      "macOS 使用技巧（更新中）"
subtitle:   "来自20年Windows老用户的疑惑"
date:       2022-09-07 22:00:00
author:     "泉雲清"
header-mask: 0.3
mathjax: true
tags: 
    - 杂谈
    - macOS
---
操作系统，很神奇吧。

---

# 写在前面
> macOS教会了我一件事情，不要只盯着窗口，抬头看看，导航栏在上面呢。

# 使用技巧  

## 1. 让Finder显示当前路径  
快捷键：`option`+`command`+`p`  
慢慢找：打开finder（开着窗口），点开左上角`view`，找到`Show Path Bar`，左键点击
![](/img/in-post/post-show-path-bar.png)

访达是第二时间让我觉得与Windows有差异的地方（第一个是安装应用，第一次看见一个图标，右边一个applications，然后啥指示没有，我直接黑人问号.jpg）

## 2. 显示桌面
对于习惯Windows ctrl+D的我来说苹果显示桌面竟然不能隐藏所有窗口，留一点小尾巴在桌面上简直难以忍受  
`command`+`F3`
![](/img/in-post/post-show-desktop.png)

## 3. 显示日期
调整设置的时候才发现MBA竟然因为屏幕太小而不显示日期。（虽然底下的Calendar已经告诉你今天的日期了  
`System Preference` -> `Dock & Menu Bar` -> 在左边栏找到 `Menu Bar Only` -> `Clock`  
show date -> "always"
![](/img/in-post/post-change-clock.png)

## 4. 截图
截图这一点做得比Windows要好，不需要print screen粘贴大法。  
快捷键：
1. 全屏截图：`shift`+`command`+`3`，**不是F3!!**
2. 自由截图：shift + command + `4`
3. 捕捉窗口、菜单： shift + command + `4` + `空格`
4. 一键解决，自由选择：shift + command + `5`

另外，键位可以在系统设置->键盘->快捷键->截屏里面改

## 5.设定程序启动快捷键
使用automator
1. 点击 New document
2. 点击 Quick actions 
3. 搜索栏中输入 Launch application 并双击选中
4. 在 Launch application 的选项中选择需要的应用
5. command + s 保存，记得修改名字
6. 在System Preference -> Keyboard -> shortcut 中选择 Services
7. 在Genearl中可以找到刚才保存的文件名，点击添加快捷键

## 6.xxx.app 已损坏，无法打开，你应该将它移到废纸篓/打不开 xxx，因为它来自身份不明的开发者解决方法  
<https://macwk.com/article/macos-file-damage>