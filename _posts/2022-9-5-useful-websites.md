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
**2022.10.26** 初步整理，估计这几天能够整理好，后续应该会慢慢加进来新的资源
# 前言  
本post旨在囊括有关网站建设的资源，但重点在于编程语言如HTML的学习网站与相关工具如GitHub的使用。对于**工具**的具体操作步骤（及代码）此处会有详细的讲解，**语言**的具体细节（也就是代码）不会出现在此篇post中。
  
# 本体 
[Travis CI - Test and Deploy with Confidence](https://app.travis-ci.com/signin?redirectUrl=https%3A%2F%2Fapp.travis-ci.com%2Faccount%2Fplan%3FbillingStep%3D3)
[ssh-agent - 小 楼 一 夜 听 春 雨 - 博客园](https://www.cnblogs.com/kex1n/p/5229493.html)

[github - fatal: could not create work tree dir 'kivy' - Stack Overflow](https://stackoverflow.com/questions/16376035/fatal-could-not-create-work-tree-dir-kivy)

## HTML  
  ### 入门教程  

--- 

## Markdown

--- 

## css

--- 

## Javascript

--- 

## Git
  ### Git命令汇总    
[git 常用命令总结 - Xheldon Blog](https://www.xheldon.com/tech/git-command.html)  
[❤ 💻 Git - git config - error: could not lock config file - Permission denied - Dirask](https://dirask.com/posts/Git-git-config-error-could-not-lock-config-file-Permission-denied-Kj825D)  

--- 

## GitHub
### 本地项目的推拉  
由于GitHub基本是自己在用，没有什么合作的需求，所以此处并不放上分支操作。b站上有视频教程，有需要的自行搜索  
- 参考资料：
[本地项目推送到远程仓库gitHub上（超详细） - 知乎](https://zhuanlan.zhihu.com/p/90168946)  
[如何将本地的项目推送至git仓库_qq61273bb7ae980的技术博客_51CTO博客](https://blog.51cto.com/u_15345018/3654464) 

- 具体步骤（待补充） 
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

生成、添加完了之后记得要用
```zsh
ssh -T git@github.com  # 检查与GitHub的连接
```

### GitHub desktop相关
1. 如何登出  
    快捷键：`ctrl` + `，`  
    不那么快的方法：  
    For Mac  
        Top Left corner of the screen, next to Mac symbol->`Github desktop`->`Preference`->Accounts->signout
    
    For Windows   
        Inside github, Right side next to Sync->Settings symbol->options->log out


--- 

## Jekyll 
### 官网  

### 安装  
 macOS安装Jekyll  <https://zhuanlan.zhihu.com/p/350462079>  

### 具体细节  

--- 

## 正则表达式

--- 

## 命令行
我在用的是哪个shell  <https://www.moncefbelyamani.com/which-shell-am-i-using-how-can-i-switch/>  
tree命令  <https://segmentfault.com/a/1190000009962072>

## 其他  
[个人博客搭建教程 | 爱扑bug的熊](https://blog.cuijiacai.com/blog-building/)  
[将hexo个人博客部署到github上公开使用。_hello_cmy的博客-CSDN博客](https://blog.csdn.net/hello_cmy/article/details/104658452)  
[将 Hexo 部署到 GitHub Pages - Google Search](https://www.google.com/search?client=safari&rls=en&q=%E5%B0%86+Hexo+%E9%83%A8%E7%BD%B2%E5%88%B0+GitHub+Pages&ie=UTF-8&oe=UTF-8)  
[node.js - 使用Hexo框架搭建博客，并部署到github上_个人文章 - SegmentFault 思否](https://segmentfault.com/a/1190000018250408)  
[One-Command Deployment | Hexo](https://hexo.io/docs/one-command-deployment#Bip)  
[将 Hexo 部署到 GitHub Pages | Hexo](https://hexo.io/zh-cn/docs/github-pages)  
[Jekyll / Hugo / Hexo Comparison | The Coding Notes](https://lexcao.io/posts/jekyll-hugo-hexo/)  


---

原版分割线  

---

### git 相关




### 命令行相关



### Jekyll相关


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