---
layout:     post
title:      "网站建设可能会用到的资源与教程（重制中）"
subtitle:   " 在学了在学了"
date:       2022-09-05 12:00:00
author:     "泉雲清"
header-img: "img/post-bg-2015.jpg"
tags:
    - 网站
    - 资源
    - 教程
---
博客是建立起来了，毕竟是套用现成的模版，还是有万千知识等着学习。~~后期应该会拆成两部分~~。  
## 更新履历
**2022.10.2** 重新安排架构

# 前言  
本post旨在囊括有关网站建设的资源，但重点在于编程语言如HTML的学习网站与相关工具如GitHub的使用。对于工具的具体操作步骤此处会有详细的讲解，语言的具体细节（也就是代码）不会出现在此篇post中。  
# 本体  
## HTML  
### 入门教程  

## Markdown

## css

## Javascript

## Git

## GitHub

## Jekyll 
### 官网  

### 安装  

### 具体细节  

## 正则表达式
---

原版分割线  

---

## 基础知识
### SSH keys & GPG
1. 一台电脑配置多个SSH keys
    <https://support.huaweicloud.com/codehub_faq/codehub_faq_0002.html>
    <https://www.jianshu.com/p/c30e1f787b92>
    <https://juejin.cn/post/7117182814310629390>
2. Mac下安装GPG
    ```bash
    brew install gpg
    ```
3. macOS生成GPG keys

    <https://docs.github.com/cn/authentication/managing-commit-signature-verification/generating-a-new-gpg-key>
3. macOS生成SSH keys

    <https://www.jianshu.com/p/63b82385c519>
    <https://blog.csdn.net/wangjunling888/article/details/51115659>
4. Windows下生成SSH keys  
    这个可以参考GitHub docs相应章节  

生成，添加完了之后记得要用
```zsh
ssh -T git@github.com  # 检查与GitHub的连接
```

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
3. 添加了SSH keys依旧显示 Permission denied(publickey)  
    这种事常发生在想添加多个ssh keys的情况，因为第一个ssh keys一般是默认的，而之后的ssh keys需要改名，
    避免与之前的名字重合。而git（或者ssh？）似乎只识别特定名称的key，比如id_rsa，id_ed25519。如果起了如github之类的名字是认不出来的。还要注意ssh keys需要挪到.ssh目录下才能识别，因为生成key的位置是terminal当前的位置。

### GitHub desktop相关
1. 如何登出  
    快捷键：`ctrl` + `，`  
    不那么快的方法：  
    For Mac  
        Top Left corner of the screen, next to Mac symbol->`Github desktop`->`Preference`->Accounts->signout
    
    For Windows   
        Inside github, Right side next to Sync->Settings symbol->options->log out

### 命令行相关
1. 我在用的是哪个shell
    <https://www.moncefbelyamani.com/which-shell-am-i-using-how-can-i-switch/>
2. tree命令
    <https://segmentfault.com/a/1190000009962072>


### Jekyll相关
1. macOS安装Jekyll
    <https://zhuanlan.zhihu.com/p/350462079>

## 会用到的网站
1. kramdown语法
    <https://kramdown.gettalong.org/syntax.html#links-and-images>
2. Jekyll官网  
    中文： <https://www.jekyll.com.cn>  
    英文： <https://jekyllrb.com>
3.  GitHub markdown语法  
    <https://docs.github.com/cn/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax>
4. Markdown 学习  
    <https://xianbai.me/learn-md/index.html>
5. git教程
    <https://runoob.com/git/git-tutorial.html>
5. html & css教程

6. 正则表达式