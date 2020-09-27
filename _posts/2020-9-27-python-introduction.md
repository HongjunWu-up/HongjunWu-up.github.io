---
layout: post
title: 关于Python的几点趣事
categories:Python
description: Python名字的由来、Python小诗、Python的特色
---
## 1.Python的由来 ## 
Python的创始人为荷兰人吉多·范罗苏姆（Guido van Rossum）。1989年圣诞节期间，在阿姆斯特丹，Guido为了打发圣诞节的无趣，决心开发一个新的脚本解释程序，作为ABC 语言的一种继承。之所以选中Python（大蟒蛇的意思）作为该编程语言的名字，是取自英国20世纪70年代首播的电视喜剧《蒙提.派森的飞行马戏团》（Monty Python's Flying Circus）。[参考1](https://baike.baidu.com/item/Python/407313?fr=aladdin)  
ABC语言是吉多之前为教学编写的语言，优美且强大。但是由于没有很好的开源，并未得到大范围的使用。于是吉多开始创作 Python，改进 ABC 语言存在的缺陷，并在原有基础上实现更多的功能。python 发布之后广受欢迎，之后2000年发布 Python2，2008年发布Python3。2004年之后，使用率呈线性增长，现已成为最受欢迎的编程语言之一，广泛运用在云计算、数据分析、人工智能、网络开发、游戏开发等各个领域。  
## 2.Python小诗 ##
安装好 Python 之后，在自带的 IDLE （集成开发学习环境）中输入 `import this`,会出现如下这一段非常优美的小诗，诗歌的内容反映了 Python 使用时应当遵循的一些准则。诗歌创作者是蒂姆·彼得斯（Tim Peters），他是 Python 的忠实用户，在2004年8月写成了这首颇具指导意义的小诗，并广为流传。
    
    Beautiful is better than ugly.
    Explicit is better than implicit.
    Simple is better than complex.
    Complex is better than complicated.
    Flat is better than nested.
    Sparse is better than dense.
    Readability counts.
    Special cases aren't special enough to break the rules.
    Although practicality beats purity.
    Errors should never pass silently.
    Unless explicitly silenced.
    In the face of ambiguity, refuse the temptation to guess.
    There should be one-- and preferably only one --obvious way to do it.
    Although that way may not be obvious at first unless you're Dutch.
    Now is better than never.
    Although never is often better than *right* now.
    If the implementation is hard to explain, it's a bad idea.
    If the implementation is easy to explain, it may be a good idea.
    Namespaces are one honking great idea -- let's do more of those!
**翻译如下：**[参考2](http://www.bytesea.com/1091.html)
    Python 之禅
    蒂姆·彼得斯(赖勇浩翻译)
    
    优美胜于丑陋（Python 以编写优美的代码为目标）
    明了胜于晦涩（优美的代码应当是明了的，命名规范，风格相似）
    简洁胜于复杂（优美的代码应当是简洁的，不要有复杂的内部实现）
    复杂胜于凌乱（如果复杂不可避免，那代码间也不能有难懂的关系，要保持接口简洁）
    扁平胜于嵌套（优美的代码应当是扁平的，不能有太多的嵌套）
    间隔胜于紧凑（优美的代码有适当的间隔，不要奢望一行代码解决问题）
    可读性很重要（优美的代码是可读的）
    即便假借特例的实用性之名，也不可违背这些规则（这些规则至高无上）
    不要包容所有错误，除非你确定需要这样做（精准地捕获异常，不写 except:pass 风格的代码）
    当存在多种可能，不要尝试去猜测
    而是尽量找一种，最好是唯一一种明显的解决方案（如果不确定，就用穷举法）
    虽然这并不容易，因为你不是 Python 之父（这里的 Dutch 是指 Guido ）
    做也许好过不做，但不假思索就动手还不如不做（动手之前要细思量）
    如果你无法向人描述你的方案，那肯定不是一个好方案；反之亦然（方案测评标准）
    命名空间是一种绝妙的理念，我们应当多加利用（倡导与号召）
**每句都将是今后创作的指导准则，谨记！**
## 3.Python的特色 ##  
参考:《A Byte of Python》 
### 3.1 简单易学 ###
Python是一门简单易学的语言，阅读代码就如同阅读英语文章，学习 Python 就好比学习英语文章写作，基本的单词和语法都容易，重点是看作者如何去创作一篇优美的有深度的文章。在 Python 中，单词就是运算符、表达式、控制流、数据结构等等一些基础知识。**Python 的语法体系非常简单，以至于使用者能专注于解决遇到的问题，而不用在语言本身花费太多时间。**
### 3.2 开源 ###
Python 是FLOSS （自由/开放源代码软件）的成员之一，源代码完全可见，并且可以对其做出修改，或是将其的一部分运用于一款新的自由程序中。 FLOSS 基于一个可以分享知识的社区理念而创建。 这正是 Python 为何能如此优秀的一大原因——它由一群希望看到 Python 能变得更好的社区成员所创造， 并持续改进至今。此外，网上存在大量的书籍、视频、论坛以便你能更好的学习 Python 的使用。
### 3.3跨平台 ###
由于其开放源码的特性， Python 已被移植到其它诸多平台（ 意即它们已经过改动以保证其能正常工作） 。 如果你小心地避开了所有系统依赖型的特性。 你所有的 Python 程序可以在其中任何一个平台上工作， 不必作出任何改动。你可以在 GNU/Linux、 Windows、 FreeBSD、 Macintosh、 Solaris、 OS/2、 Amiga、AROS、 AS/400、 BeOS、 OS/390、 z/OS、 Palm OS、 QNX、 VMS、 Psion、 Acorn RISC OS、 VxWorks、 PlayStation、 Sharp Zaurus、 Windows CE 以及 PocketPC 平台上运行 Python！
你甚至可以通过诸如 Kivy 一类的平台来制作可在你的电脑 以及 iPhone、 iPad 或安卓手机上运行的游戏。
### 3.4面向对象  ###
Python 同时支持面向过程编程与面向对象编程。 在面向过程的编程语言中，程序是由仅仅带有可重用特性的子程序与函数所构建起来的。 在**面向对象**的编程语言中， 程序是由**结合了数据与功能的对象**所构建起来的。
3.5其他特色
可拓展性（用C/C++编写程序运用到 Python）、可嵌入式（Python 程序用到C/C++中）、丰富的库