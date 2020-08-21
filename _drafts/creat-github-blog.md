---
layout: post
title: Github+Jekyll模板搭建个人博客（入门教程）
categories: github blog
description: 利用GitHub page搭建个人博客
keywords: Github,Jekyll , Markdown
---
## 1.写作目的 ##
**写作意义**：本篇文章会详细的介绍如何使用Jekyll模板搭建Github个人博客，入门级教程，暂时不需要用到git、gem、jekyll指令，相应的文件和安装包也可通过文末链接下载。
**博客搭建初衷**：GitHub 作为一个面向开源及私有软件项目的托管平台，堪比程序界的Facebook。研究生准备学习CV方向，有代码托管的需求，开始了解以及使用Github。同时，为了记录学习过程中遇到的问题以及解决方法，准备搭建个人博客，不仅可以加深对知识的理解，还有利于业界人士的交流分享。
知乎、CSDN、博客园、简书等各大平台各有优缺点（[参考1](https://blog.csdn.net/grape875499765/article/details/79017906)），根据自己需要选择就好。而GitHub Pages作为一款定制性强，轻量级的博客系统，同时有利于学习GitHub的使用，自然成为博客搭建的不二选择。
## 2.Github Pages介绍 ## 
GitHub Pages 是一个静态网站托管服务，直接从github仓库托管你个人、公司或者项目页面 ，并且不需要个人额外书写任何后端语言来支持。而nodejs的hexo和ruby的jekyll 均是静态网页生成系统，生成模板中原始文本格式的文档，通过转换器（如 Markdown）和渲染器转化成一个完整的可发布的静态网站，发布在Github Pages上，进而完成博客网页的创建。
**第一步**:注册一个 GitHub 账号，然后到个人主界面里面，创建一个新的 Repository。
**注意:命名一定是用户名.github.io。** README.选项也可勾选上。
![github-pages](/images/blog/github-pages.png)
此时访问[https://用户名.github.io/]便可以看到简陋版的个人博客了。例如博主博客：https://hongjunwu-up.github.io/
## 3.Jekyll主题使用 ##
Jekyll使用Rudy语言编写，能够将纯文本转化为静态网站和博客。作为入门级别教程，本文章不讲述安装Jekyll和如何利用Jekyll生成博客，有意向者可参考[Jekyll官网](https://www.jekyll.com.cn/)，官网有相关的详细介绍。
由于自己创建的模板一般都比较简单（大佬忽略），故一般在网上寻找功能比较完善的主题模板，再通过修改，生成自己的博客主页。在此推荐几个模板途径。[参考2](https://blog.csdn.net/chen_z_p/article/details/103132625)
1.[Jkyll主题官网](http://jekyllthemes.org/):有大量的主题可供选择，点击demo可以预览。缺点就是大海捞针，难合口味。
2.[Hux Blog](https://github.com/Huxpro/huxpro.github.io)：简约，有标签，没有主题分类。
3.[码志](https://github.com/mzlogin/mzlogin.github.io)：简约、美观，有分类、目录，增加评论功能。当然就选它了。
**第二步：码志博客下载**
1.点击[码志](https://github.com/mzlogin/mzlogin.github.io)，下载博客主题。
![mz-blog-load.png](/images/blog/mz-blog-load.png)
2.解压后修改，码志主题readme.md文件里介绍了如何对主题进行修改，变成自己的博客。
![mz-blog-change.png](/images/blog/mz-blog-change.png)

## 4.markdow更新个人博客 ##
markdownpad2使用介绍