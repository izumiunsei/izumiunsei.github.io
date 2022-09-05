---
layout:     post
title:      "网站建设可能会用到的资源与教程"
subtitle:   " 在学了在学了"
date:       2022-09-04 12:00:00
author:     "泉雲清"
header-img: "img/post-bg-2015.jpg"
tags:
    - 网站
    - 资源
    - 教程
---
博客是建立起来了，毕竟是套用现成的模版，还是有万千知识等着学习。后期应该会拆成两部分。
## 基础知识
### SSH keys & GPG
1. 一台电脑配置多个SSH keys
    https://support.huaweicloud.com/codehub_faq/codehub_faq_0002.html
    https://www.jianshu.com/p/c30e1f787b92
    https://juejin.cn/post/7117182814310629390
2. Mac下安装GPG
    ```bash
    brew install gpg
    ```
3. macOS生成GPG keys
    https://docs.github.com/cn/authentication/managing-commit-signature-verification/generating-a-new-gpg-key
3. macOS生成SSH keys
    https://www.jianshu.com/p/63b82385c519
    https://blog.csdn.net/wangjunling888/article/details/51115659

### git 相关
1. git 修改远程仓库地址
    ```bash
    git remote rm origin
    git remote add origin [url]
    ```
2. git 推送远程仓库标准流程
    ```bash
    git init # 初始化git
    git add . # 添加当前文件夹下所有内容
    git commit -m “工作内容总结，自由填写” # commit可作“递交“解
    git remote add origin [url] # 在repo主界面点击绿色的“code”即可复制相应repo的url
    git branch -M main
    git push -u origin main # 別push了，再push我都要寄了
    ```

### GitHub desktop相关
1. 如何登出
    快捷键：ctrl + ，
    不那么快的方法：
    For Mac
        Top Left corner of the screen, next to Mac symbol->==Github->Preference->Accounts->signout==
    
    For Windows 
        Inside github, Right side next to Sync->Settings symbol->options->log out

### 命令行相关
1. 我在用的是哪个shell
    https://www.moncefbelyamani.com/which-shell-am-i-using-how-can-i-switch/
2. tree命令
    https://segmentfault.com/a/1190000009962072


### Jekyll相关
1. macOS安装Jekyll
    https://zhuanlan.zhihu.com/p/350462079

## 会用到的网站
1. kramdown语法
    https://kramdown.gettalong.org/syntax.html#links-and-images
2. Jekyll官网
    中文： https://www.jekyll.com.cn
    英文： https://jekyllrb.com

