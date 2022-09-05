[Izumiunsei Blog](https://ius.shn.hk)
================================

> 此博客模版为hux blog(链接见底部)

估计也没有人会看到我的博客，除非自己推广
博客内容则是想到什么就写什么，涵盖的范围那只有老天才知道了。

[User Manual](_doc/Manual.md)
--------------------------------------------------

### Development (Build From Source)

To modify the theme, you will need [Grunt](https://gruntjs.com/). There are numbers of tasks you can find in the `Gruntfile.js`, includes minifing JavaScript, compiling `.less` to `.css`, adding banners to keep the Apache 2.0 license intact, watching for changes, etc. 

Yes, they were inherited and are extremely old-fashioned. There is no modularization and transpilation, etc.

Critical Jekyll-related code are located in `_include/` and `_layouts/`. Most of them are [Liquid](https://github.com/Shopify/liquid/wiki) templates.

This theme uses the default code syntax highlighter of jekyll, [Rouge](http://rouge.jneen.net/), which is compatible with Pygments theme so just pick any pygments theme css (e.g. from [here](http://jwarby.github.io/jekyll-pygments-themes/languages/javascript.html) and replace the content of `highlight.less`.


### Interesting to know more? Checkout the [full user manual](_doc/Manual.md)!


Other Resources
---------------
Translation
- [中文文档（有点过时）](https://github.com/Huxpro/huxpro.github.io/blob/master/_doc/README.zh.md)


License
-------

Apache License 2.0.
Copyright (c) 2022-present Izumi Unsei

IzumiUnsei Blog is derived from [Hux Blog](https://github.com/Huxpro/huxpro.github.io)
Copyright (c) 2015-present Huxpro
