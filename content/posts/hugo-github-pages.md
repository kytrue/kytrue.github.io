+++
title = "用hugo在github上建立个人博客"
date = 2021-03-29T16:28:28+08:00
images = []
tags = ["hugo", "markdown"]
categories = []
draft = false
+++

hugo把markdown写的博客文章，转换成html静态网页。将这些静态网页推送到github pages，就可以轻松建立个人博客。现在的这篇文章就是这样生成的。

查看hugo的文档到[这里](https://gohugo.io/getting-started/quick-start/)，可以快速了解hugo的使用。

hugo需要选用一个主题，这里使用的是[kiera](https://themes.gohugo.io/hugo-kiera/)。

快速入门这个主题，可以查看hugo-kiera下的exampleSite目录，参考里面的示例来进行配置。

## hugo配合github pages的设置

hugo编译后，默认生成的是public目录。在config.toml文件里添加

```
publishDir = "docs"
```

把生成目录改为docs，在github的项目设置里面，把github pages的根目录改为docs，这样就可以看到github pages了。