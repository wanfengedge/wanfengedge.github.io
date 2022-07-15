---
title: "Gitattributes作用详细讲解"
description: "gitattributes作用详细讲解"
#keywords: "gitattributes作用详细讲解"

date: 2022-07-15T16:04:40+08:00
lastmod: 2022-07-15T16:04:40+08:00

categories:
  - git
tags:
  - git

# 原文作者
# Post's origin author name
#author:
# 原文链接
# Post's origin link URL
#link:
# 图片链接，用在open graph和twitter卡片上
# Image source link that will use in open graph and twitter card
#imgs:
# 在首页展开内容
# Expand content on the home page
#expand: true
# 外部链接地址，访问时直接跳转
# It's means that will redirecting to external links
#extlink:
# 在当前页面开启或关闭评论功能
# Switch to enabled or disabled comment plugins in this post
#comment:
#  enable: false
# 开启文章目录功能
# Enable table of content
toc: false
# 绝对访问路径
# Absolute link for visit
url: "gitattributes作用详细讲解.html"
# 开启文章置顶，数字越小越靠前
# Sticky post set-top in home page and the smaller nubmer will more forward.
#weight: 1
---

## .gitattributes介绍

.gitattributes 是一个文本文件，文件中的一行定义一个路径的若干个属性，主要用于定义每种文件的属性，以方便 git 帮我们统一管理。

.gitattributes 文件格式如下
```plain
要匹配的文件模式 属性1 属性2 ...
```

在.gitattributes文件的一行中，一个属性（以text属性为例）可能有4种状态：

- 设置text
- 不设置-text
- 设置值text=string
- 未声明，通常不出现该属性即可；但是为了覆盖其他文件中的声明，也可以!text

## .gitattributes 文件中可以定义的属性

**text**
用于控制行尾的规范性。如果一个文本文件是规范的，则Git库汇总该文件（git 服务器上的文件）的行尾总是LF。对于工作目录，除了text属性之外，还可以设置eol属性或core.eol配置变量。

**eol**
设置行末字符。

- eol=lf ，[回车] ：入库时将行尾规范为LF，检出时行尾不强制转换为 CRLF
- eol=crlf，[换行、回车] ：入库时将行尾规范为LF，检出时将行尾转换为CRLF

>补充：CRLF 和 LF
>GRLF 和 LF都是用来表示文本换行的方式。CR代表回车，对应字符 \r。LF 表示换行，对应字符 \n。不同操作系统文本使用的换行符各不相同。Windows系统使用的是 CRLF，Unix系统（包括Linux，MacOS近些年的版本）使用的是 LF。

>补充：为什么需要去关心行尾是什么
>事实上，可能并不是所有的开发者用的环境都完全一样，比如有的开发者使用 Windows 环境开发，他们的文本文件的换行符是 ‘\r\n’（CRLF）；而有的开发者使用 MacOS 环境开发，这些开发者文本文件的换行符是 ‘\n’（LF）。为了使得不同系统环境的开发者能开发同一个git项目，便出现了这个。

**diff**
我们知道 git 主要是用来跟踪文件版本的，跟踪文件版本自然离不开比较差异，而diff 就是用来告诉 git 声明文件需要比较版本差异的。
diff属性影响Git对特殊文件生成差异的方式。它可以告诉Git是否为路径生成文本补丁还是将路径视为二进制文件。它也可以影响在hunk头部显示的@@ -k,l +n,m @@，告诉Git使用外部命令来生成差异，或者是在生成差异之前让Git将二进制文件转换为文本文件。

- diff
强制视为文本文件，即使它包含一些通常从不会出现在文本文件的字节值，例如NUL。

- !diff
表示为非文本文件，没有设置diff属性的路径会生成differ二进制文件（如果启用了二进制补丁，会生成二进制补丁）。

- 未定义
未指明diff属性的路径首先会检查其内容，如果它看起来像文本文件并且小于大文件阈值（`core.bigFileThreshold`），则将其视为文本文件，否则将生成differ二进制文件。

>core.bigFileThreshold：所有平台上的默认值为512MiB。大于此大小的文件将被缩减，而不会尝试增量压缩。

**differ 规则**
diff 是使用指定的 diff 驱动程序显示的。每个驱动程序可以指定一个或多个选项。

- 如何自定义一个外部的diff驱动程序？
diff驱动程序的定义是在gitconfig中完成的，并不是在gitattributes文件中，所以严格来说，这里并不适合谈论它。

## .gitattributes 示例
以两个例子快速熟悉.gitattributes文件

### 示例1
以下是 Spring 仓库的 .gitattributes 文件

```plain
# Declare files that will always have LF line endings on checkout.
*.cpp text eol=lf
*.h text eol=lf
*.c text eol=lf
*.hpp text eol=lf
*.cmake text eol=lf
*.sh text eol=lf
*.py text eol=lf
```

可以看到 Spring 仓库的 .gitattributes 文件中定义了几种不同语言源码文件的行尾换行符（eol 的含义是 End Of Line，即行尾的意思），表示git命令操作的这几类文件都需要以。

### 示例2
下面以一个更详细的规则来介绍

```plain
*           text=auto  
# 文件的行尾自动转换。如果是文本文件，则在文件入Git库时，行尾自动转换为LF。如果已经在入Git库中的文件的行尾是GRLF，则文件在入Git库时，不再转换为LF。

*.txt       text  
# 对于.txt文件，标记为文本文件，并进行行尾规范化。

*.jpg       -text  
# 对于`.jpg`文件，标记为非文本文件

*.vcproj    text eol=crlf 
# 对于.vcproj文件，标记为文本文件，在文件入Git库时进行规范化，行尾转换为LF。在检测到出工作目录时，行尾自动转换为GRLF。

*.sh        text eol=lf  
# 对于sh文件，标记为文本文件，在文件入Git库时进行规范化，即行尾为LF。在检出到工作目录时，行尾也不会转换为CRLF（即保持LF）。

*.py        eol=lf  
# 对于py文件，只针对工作目录中的文件，行尾为LF。
```

## .gitattributes生效顺序
在一个Git库中可以有多个.gitattributes 文件，不同.gitattributes 文件中，属性设置的优先级(从高到低)如下：

- /myproj/info/attributes 文件
- /myproj/my_path/.gitattributes 文件
- /myproj/.gitattributes 文件
- 同一个.gitattributes 文件中，遵循覆盖原则，即后面的行会覆盖前面的设置，如果一个文件的某个属性被多次设置，则后设置的优先，类似 int a = 1; a = 2; 最终结果 a == 2。

## 使用

### 为新的Git库设置统一的.gitattributes文件：

在仓库的根目录下创建名为 .gitattributes 的文件。

```plain
touch .gitattributes
vi .gitattributes
```

编辑这个文件并输入希望的设置，demo 如下：

```plain
*.sh text eol=lf
```

把该文件提交并推送到服务器上。

```plain
git add .
git commit -m "add.gitattributes"
git push
```

### 为已有Git库设置统一的.gitattributes文件（重置 GitAttributes）：

在上一步的基础上（确保仓库根目录下已经存在.gitattributes文件）

```plain
git rm --cached -r
git reset --hard
```

上面的命令就会根据文件 .gitattributes 中的定义，更新文件的结尾行。

任何变更都会自动使用指定文件的文件结尾行格式。

下一步，可以通知团队成员或者协作者去执行 Git 属性重置的命令即可。

### 为所有Git库设置统一的.gitattributes文件：

```plain
git config --get core.attributesFile
git config --global --get core.attributesFile
```

参考：<https://git-scm.com/docs/gitattributes>