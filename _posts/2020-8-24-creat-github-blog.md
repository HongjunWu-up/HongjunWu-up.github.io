---
layout: post
title: GitHub+Jekyll 模板搭建个人博客（入门教程）
categories: Blog
description: 利用 GitHub Pages 搭建个人博客
keywords: GitHub,Jekyll , Markdown
---
## 1.目的 ##

GitHub 作为一个面向开源及私有软件项目的托管平台，堪比程序界的Facebook。而GitHub Pages作为一款定制性强，轻量级的博客系统，同时有利于学习GitHub的使用，自然成为博客搭建的选择之一。本篇文章会详细的介绍如何使用 Jekyll 模板搭建 GitHub 个人博客，**入门级教程，暂时不需要用到 git、gem、jekyll 指令**，相应的文件和安装包下载链接文章会给出。
## 2.GitHub Pages介绍 ## 
GitHub Pages 是一个静态网站托管服务，直接从 GitHub 仓库托管你个人、公司或者项目页面 ，并且不需要个人额外书写任何后端语言来支持。而 nodejs 的 hexo 和 ruby 的 jekyll 均是静态网页生成系统，生成模板中原始文本格式的文档，通过转换器（如 Markdown ）和渲染器转化成一个完整的可发布的静态网站，发布在Github Pages上，进而完成博客网页的创建。  
**第一步**:注册一个 GitHub 账号，然后到个人主界面里面，创建一个新的 Repository。    
**注意:命名一定是用户名.github.io。** README 选项也可勾选上。    
![github-pages](/images/blog/github-pages.png)
此时访问 https://用户名.github.io/ 便可以看到简陋版的个人博客了。例如博主博客： [https://hongjunwu-up.github.io/](https://hongjunwu-up.github.io/)
## 3.Jekyll主题使用 ##
Jekyll 使用 Rudy 语言编写，能够将纯文本转化为静态网站和博客。作为入门级别教程，本文章不讲述安装Jekyll 和如何利用 Jekyll 生成博客，有意向者可参考[Jekyll官网](https://www.jekyll.com.cn/)，官网有作详细介绍。  
由于自己创建的模板一般都比较简单（大佬忽略），故一般在网上寻找功能比较完善的主题模板，再通过修改，生成自己的博客主页。在此推荐几个模板途径。[参考](https://blog.csdn.net/chen_z_p/article/details/103132625)    
1.[Jkyll 主题官网](http://jekyllthemes.org/):有大量的主题可供选择，点击demo可以预览。缺点就是大海捞针，难合口味。    
2.[Hux Blog](https://github.com/Huxpro/huxpro.github.io)：简约，有标签，没有主题分类。  
3.[码志](https://github.com/mzlogin/mzlogin.github.io)：简约、美观，有分类、目录，增加评论功能、网页浏览量统计。不错的选择！  
**第二步：码志博客主题下载及修改**  
1.点击[码志](https://github.com/mzlogin/mzlogin.github.io)，下载博客主题。也可使用`git clone <url>` 指令下载到本地，此处不作介绍。（GitHub 下载速度极慢，建议fork到码云下载或者是通过文末链接下载。）    
![mz-blog-load.png](/images/blog/mz-blog-load.png)  
2.解压后得到的文件，可参考[ Jekyll 官网模板结构的介绍](https://www.jekyll.com.cn/docs/structure/)，了解每个文件的作用。  
![Jekyll-file-function1.png](/images/blog/Jekyll-file-function1.png)
![Jekyll-file-function2.png](/images/blog/Jekyll-file-function2.png)   
3.码志主题 readme.md 文件里介绍了如何对主题进行修改，从而变成自己的博客。**主题里的关键性配置都在 _config.yml 文件中，**建议使用notepad打开文件再进行修改。其中 gittalk 帐号和 Google 账号请自行申请。（如果不知道如何修改，先跳过本步，完成第三步更新博客，浏览原博客页面布局，加深理解后，再返回修改模板文件。）
![mz-blog-change.png](/images/blog/mz-blog-change.png) ** 
url、基本信息修改：**
![config-change1.png](/images/blog/config-change1.png)  
**gittalk 帐号和 Google 账号请自行申请然后修改 ID 和密码：**
![config-change2.png](/images/blog/config-change2.png)
![config-change3.png](/images/blog/config-change3.png)   
**注意：**需创建 blog-comments repository，存放评论，否侧会出现 `gittalk error：not found`警告。创建库时请参考：[https://blog.csdn.net/qing_gee/article/details/100133060](https://blog.csdn.net/qing_gee/article/details/100133060)
## 4.使用 GitHub Desktop 完成文件上传  ##
如果没有 Git 的基础，可选择 GitHub Desktop 更新博客，无需指令，简单易懂。  
**第三步：使用 GitHub Desktop 更新博客主题**  
1.下载 [GitHub Desktop](https://desktop.github.com/)，官网下载极慢，文末提供百度云链接。  
2.客户端登陆 GitHub 账号，clone 用户名.github.io仓库到本地，如下图。  
![GitHub-Desktop.png](/images/blog/GitHub-Desktop.png)  
3.找到上图仓库克隆文件位置，删除所有文件。并将第二步中下载并修改后的码志博客文件全部复制到该位置。  
![copy-mz-blog.png](/images/blog/copy-mz-blog.png)  
4.进入 GitHub Desktop，左边会显示文件夹更改的内容，按照下图操作即可。  
![push-blog-change.png](/images/blog/push-blog-change.png)  
![push-blog-change2.png](/images/blog/push-blog-change2.png)    
push 成功后便可以访问[https://用户名.github.io/]查看自己的博客了。（若安装了Jekyll，使用`jekyll s`指令可以实现本地访问，参考 [Jekyll 官网](https://www.jekyll.com.cn/)）。  
## 5.markdow 编辑器写博文 ##
上文中提到 Jekyll 支持 markdown，那什么是 Markdown 呢？Markdown 是一款面向 web 作者的文本到 html 转换工具。Markdown 允许您使用易于阅读、易于编写的纯文本格式进行编写，然后将其转换为结构上有效的XHTML(或HTML)。Markdown 编辑器众多，可自行搜索根据优缺点选择。博主使用的是 MarkdownPad2 写文章，windows 用户较多，可实现实时预览。  
**第四步：使用 MarkdownPad2 写文章**
1.下载 MarkdownPad2 安装包，Win10 要实时预览还需额外安装组件 awesomium_v1.6.6_sdk_win，安装包和组件下载链接见文末。[安装教程参考](https://www.jianshu.com/p/1745a7f53404  )  
2.由于 MarkdownPad2 默认的 Processor 和 GitHub 不太一样，故需设置成 GitHub 风格。设置路径为：工具->选项，再按照下图操作。
![markdownpad2-setting2.png](/images/blog/markdownpad2-setting2.png)    
若预览页面显示 MarkdownPad2 无法使用gihub Markdown在线风格，提示“请求被中止: 未能创建 SSL/TLS 安全通道”，请安装.Net Framework 4.5以上版本。[解决方法参考此博客。](https://blog.csdn.net/qq18938308968/article/details/86243272)  
3.到此为止，MarkdownPad2 的环境搭建完成，[点击熟悉 markdown 的语法](https://www.jianshu.com/p/e9840793d8c2)。此时便可以专心码字，创作属于你的博文了。
记住文章命名为 year-month-day-blog name.md,放入_posts文件夹,使用 GitHub Desktop push 到 GitHub，便可以看到更新的博文了。细节性的处理还需各位慢慢摸索，希望对你有帮助。

**文档下载链接：**
码志博客链接：https://pan.baidu.com/s/1dbYX7HUfwR-ENxA5cq0zjQ  提取码：mgww  
notepad 安装包链接：https://pan.baidu.com/s/1wWGy6l45HsVsdjh1MM9eig   提取码：uflm  
GitHub Desktop链接：https://pan.baidu.com/s/1D5BPMSLtoFal9PF-nsrCPg   提取码：14ta  
MarkdownPad2相关文件（安装包、组件、.Net Framework 4.7）链接：https://pan.baidu.com/s/1HpQ8Ix8gOGBMGL4tmayM2g   提取码：96lx
Git 安装包（使用 git 指令的可下载）链接：https://pan.baidu.com/s/1z25Jb0djqTntVGNkGrRtgQ  提取码：b6fs

