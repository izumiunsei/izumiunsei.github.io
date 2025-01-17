---
layout:     post
title:      "网站之Markdown语法要点（随时添加）"
subtitle:   ""
date:       2022-09-05 13:00:00
author:     "泉雲清"
header-mask: 0.3
tags:
  
  
    - 教程
---
本人常使用obsidian，本文为其与GitHub markdown与kramdown的不同点，及一些共通语法知识(以及一堆废话)

## 正常文本高亮
相较于obsidian的==高亮，GitHub markdown采用的是\`\`高亮。注意是引用代码块的符号\`   
如`这里是高亮文本`  
## 换行，段落与缩进
由于markdown本身的特点，很难实现普通文本的缩进，因为一个tab四个空格的缩进直接让其变成了代码块。将空格变为全角应该能解决这个问题，但在Mac自带输入法上不易实现。obsidian在这里做得极其糟糕，相比之下typora能很好地支持tab缩进与空格缩进，符合正常写作的习惯。虽然可以通过改动css，或者加上`&nbsp;`或`&emsp;`的办法实现首行缩进，但一是麻烦，二是习惯了word的逻辑。所以对缩进有强迫症的人可以选择typora，或者放弃markdown。

obsidian对于换行与起一个段落的逻辑也是比较混乱的，原版markdown做得就还好。编辑器里换行在实际观看时还是连在一起的，需要在结尾打上两个空格，回车才能换行，比如这样：  
新起一个段落需要空出一行，latex的逻辑也是一样的，

比如这样，与word稍有不同，并不是所见即所得。

## URL超链接  
URL两端用`<>`括起即可实现超链接。  
也可用
```markdown
[name](url) <!-- 注意方括号和圆括号中间没有空格 --> 
```
这种只会显示方括号中的内容

## obsidian中块链接/引用
在通常的`[[]]`引用中添加`^`即可。

## 图片引用  
跟超链接很相似，只是多加了个感叹号
```markdown
![name](/img/404-bg.jpg) <!-- name可以空着，效果为纯放图片，地址跟自己设定有关 -->  
```

## obsidian中find&replace快捷键
`command`+`option`+`F`
