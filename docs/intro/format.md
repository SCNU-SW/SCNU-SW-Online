---
title: 格式手册
author: OI-Wiki, SCNU-SW-Online
updated: 2024/08/01
date: 2024/07/09
description: 本文档列出了在华师手册编写过程中推荐使用的格式规范。
---

🎉👍 在文章开始之前，再次感谢您抽出宝贵时间为 **华师手册** 做出贡献！ 🎉👍

本页面将列出在 **华师手册** 编写过程时推荐使用的格式规范。建议在撰稿或者修正页面之前阅读，以帮助您完成更高质量的内容。

## 贡献文档要求

==当你打算贡献某部分的内容时，你应该尽量熟悉以下两部分：==

-   ==文档、图片存储的格式（必看）==
-   正文 Markdown 和 $\rm{\LaTeX}$ 公式的格式要求

### 文档图片存储的格式

-   **文件名请务必都小写，以 `-` 分割。** 例如：`file-name.md`。

-   ==请务必确保文档中引用的 **外链** 图片已经全部转存到了 **本库内** （文章对应的分类文件夹中） 对应的 `images` 文件夹中（防止触发某些网站的防盗链），建议处理成 `MD 文档名称 + 编号` 的形式（可参考已有文档中图片的处理方式）。例如：本篇文档的文件名称为 format，则文档中引用的第一张图片的名字为 `format-1.png`。==

- 文档中引用的 **外链** 文件已经全部转存到了 **本库内** （文章对应的分类文件夹中） 对应的 `files` 文件夹中

-   ==推荐使用 [图片处理工具](https://imagestool.com/zh_CN/) 对图片格式进行转换，推荐WEBP格式，若图片过大可进行压缩。==

-   请确保您的文档中的引用链接的稳定性。**不推荐** 引用 **自建** 服务中的资源。

-   ==使用 `![]()` 添加图片时，`[]` 内务必填写唯一的描述信息，以保证SEO效果，`()` 内请填写相对路径。==

### 文档的基本格式要求

#### 格式要求

由于维护人员有限，为了整站阅读感受的一致性，请按照下列要求编辑文档：

-   不要使用如 `<h1>` 或者 `# 标题` 的一级标题。

-   标题要空一个英文半角空格，例如：`## 简介`。

-   列表：
    -   列表前要有空行，新开一段。
    -   使用有序列表（如 `1. 例子`）时，点号后要有空格。

-   行间公式前后各要有一行空行，否则会被当做是行内公式。

-   使用 `???` 或 `!!!` 开头的 Details 语法时，每一行要包括在 Details 语法的文本框的文本，开头必须至少有 4 个空格。

    **即使是空行，也必须保持与其他行一致的缩进。请不要使用编辑器的自动裁剪行末空格功能。**

    ???+ success "示例"
        ```text
        ???+ warning
            请记得在文本前面添加 4 个空格。其他的语法还是与 Markdown 语法一致。
            
            不添加 4 个空格的话，文本就不会出现在 Details 文本框里了。
            
            这个`???`是什么的问题会在下文解答。
        ```
        
        ???+ warning
            请记得在文本前面添加 4 个空格。其他的语法还是与 Markdown 语法一致。
            
            不添加 4 个空格的话，文本就不会出现在 Details 文本框里了。
            
            这个 `???` 是什么的问题会在下文解答。

-   代码样式的纯文本块请使用 ` ```text`。直接使用 ` ``` ` 而不指定纯文本块里的语言，可能会导致内容被错误地缩进。

-   站内链接请去掉网站域名，并且使用相对路径链接对应 `.md` 文件。例如，在本页面（`intro/format`）中链接杂项简介（`misc`），应使用 `[黄页简介](../contact/index.md)`。可以在链接中添加 hash 来链接到某一节，例如 [`[在 GitHub 上编辑](./htc.md#在-GitHub-上编辑)`](./htc.md#在-GitHub-上编辑)，hash 的值可以通过位于每个标题右侧的按钮或者位于网页右侧的目录中的链接得到。

#### 标点符号的使用

-   请在每句话的末尾添加 **句号**。
-   请正确使用 **全角** 标点符号与 **半角** 标点符号。汉语请使用全角符号，英语请使用半角符号。中文中夹用英文时，请参考 [中文出版物夹用英文的编辑规范](https://www.nppa.gov.cn/nppa/contents/805/102791.shtml)。

-   注意区分 **顿号** 与 **逗号** 的使用。
-   注意 **括号** 的位置。句内括号与句外括号的位置不同。
-   通常使用 **分号** 来表示列表环境中各复句之间的关系。
-   对于有序列表，推荐在每一项的后面添加 **分号**，在列表最后一项的后面添加 **句号**；对于无序列表，推荐在每一项的后面添加 **句号**。

#### Markdown 格式与主题扩展格式要求

-   表示强调时请使用 `**SOMETHING**` 和 `「」`，而非某级标题，因为使用标题会导致文章结构层次混乱和（或）目录出现问题。

-   请正确使用 Markdown 的区块功能。插入行内代码请使用一对反引号包围代码区块；行间代码请使用一对 ` ``` ` 包围代码区块，其中反引号就是键盘左上角波浪线下面那个符号，行间代码请在第一个 ` ``` ` 的后面加上语言名称（如：` ```cpp`）。

    ???+ success "示例"
        ````text
        ```cpp
        // #include<stdio.h>    //不好的写法
        #include <cstdio>  //好的写法
        ```
        ````
        
        ```cpp
        // #include<stdio.h>    //不好的写法
        #include <cstdio>  //好的写法
        ```

-   「参考资料与注释」使用 Markdown 的脚注功能进行编写。格式为：

    ```markdown
    文本内容。[^脚注名]
    [^脚注名]: 参考资料内容。注意：冒号是英文冒号，冒号后面跟着一个空格。
    ```

    脚注名既可以使用数字也可以使用文本。脚注名摆放的位置与括号的用法一致。为美观起见，建议同一个页面内的脚注名遵循统一的命名规律，如：ref1、ref2、note1……

    脚注的内容统一放在 `## 参考资料与注释` 二级标题下。

    ???+ success "示例"
        ```markdown
        当 `#include <cxxxx>` 可以替代 `#include <xxxx.h>` 时，应使用前者。[^ref1]
        
        2020年1月21日，CCF宣布恢复NOIP。[^ref2]
        
        ## 参考资料与注释
        
        [^ref1]: [cstdio stdio.h namespace](https://stackoverflow.com/questions/10460250/cstdio-stdio-h-namespace)
        
        [^ref2]: [CCF关于恢复NOIP竞赛的公告-中国计算机学会](https://www.ccf.org.cn/c/2020-01-21/694716.shtml)
        ```
        
        当 `#include <cxxxx>` 可以替代 `#include <xxxx.h>` 时，应使用前者。[^ref1]
        
        2020 年 1 月 21 日，CCF 宣布恢复 NOIP。[^ref2]

-   建议使用主题扩展的 `???+note` 格式（即 [Collapsible Blocks](https://squidfunk.github.io/mkdocs-material/reference/admonitions/#collapsible-blocks)）来描述题面和参考代码。也可以用这种格式来展示其他需要补充介绍的内容。

    示例代码：

    ```text
    ??? note "标题"
        这个文本框会被默认折叠。

        推荐将 **解题代码** 放在折叠文本框内。

    ???+note "[HDOJ 的「A + B Problem」](https://vjudge.net/problem/HDU-1000)"
        标题也可以使用 Markdown 的超链接。这里的超链接是 HDOJ 的「A + B Problem」。

        而且推荐以这种方式**标注原题链接**。

        注意双引号的位置。
    ```

    效果：

    ??? note "标题"
        这个文本框会被默认折叠。
        
        推荐将 **解题代码** 放在折叠文本框内。

    ???+ note "[HDOJ 的「A + B Problem」](https://vjudge.net/problem/HDU-1000)"
        标题也可以使用 Markdown 的超链接。这里的超链接是 HDOJ 的「A + B Problem」。
        
        而且推荐以这种方式 **标注原题链接**。
        
        注意双引号的位置。

    两种格式的区别是，带 `+` 的会默认保持展开，而不带 `+` 的会默认保持折叠。

    折叠框的标题，即 `???+note` 中 `note` 后的内容应以 `"` 包裹起来。其中的内容支持 Markdown 语法。详见 [Admonition - Changing the title](https://squidfunk.github.io/mkdocs-material/reference/admonitions/#changing-the-title)。（不具备折叠功能的为一般的 Admonitions，参考 [Admonitions - Material for MkDocs](https://squidfunk.github.io/mkdocs-material/reference/admonitions)）

如果对 mkdocs-material（我们使用的这个主题）还有什么问题，还可以查阅 [MkDocs 使用说明](https://github.com/ctf-wiki/ctf-wiki/wiki/Mkdocs-%E4%BD%BF%E7%94%A8%E8%AF%B4%E6%98%8E) 和 [cyent 的笔记](https://cyent.github.io/markdown-with-mkdocs-material/)。前者介绍了 mkdocs-material 主题的插件使用方式，而后者介绍了 Markdown 传统语法和 mkdocs-material 支持的扩展语法。

#### 文本内容的格式要求

-   在页面的开头应有一段简短的文字（如「本页面将介绍……」），用于概述页面内容。

    ???+ success "示例"
        本页面将列出在 **华师手册** 编写过程时推荐使用的格式规范与编辑方针。

-   涉及到「前置知识」的页面，请在开头添加一行 **前置知识：……**，放在页面概述前。格式如下：

    `前置知识：[站内页面1](url1)、[站内页面2](url2)和[站内页面3](url3)`

    ???+ success "示例"
        前置知识：[Git](../study/dse/git.md)
        
        本页面将介绍Git的知识。

-   请注意文档结构。文档结构应当十分条理，层次清晰。请不要让诸如「五级标题」这种事情再次发生了，一篇正常的文章是用不到如此复杂的结构层次的。

-   请尽量为链接提供完整的标题、或者可被识别的提示，避免使用裸地址和「这」、「此」之类的模糊不清的描述。每一个超链接都应尽量对其加以清楚明确的描述，方便读者明白该超链接将指向何处。

    建议使用源文章或者标签页的标题。

    ???+ fail "不推荐的写法"
        ```markdown
        请参考[这个页面](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/syncing-a-fork)
        
        请参考 <https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/syncing-a-fork>
        ```
        
        请参考 [这个页面](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/syncing-a-fork)
        
        请参考 <https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/syncing-a-fork>

    ???+ success "推荐的写法"
        ```markdown
        请参考 GitHub 官方的帮助页面 [Syncing a fork - GitHub Docs](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/syncing-a-fork)
        ```
        
        请参考 GitHub 官方的帮助页面 [Syncing a fork - GitHub Docs](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/syncing-a-fork)

-   受 Markdown 格式限制，`## 参考资料与注释` 二级标题必须放在文末。

-   所有用作序号的数字建议使用中文。示例：
    -   数列的第一项。
    -   输入文件的第一行。

-   请尽量避免在标题中使用 MathJax 公式，无论是几级标题。在标题中使用公式有可能会导致目录显示错误。

-   请注意代码的可读性。
    -   代码应拥有清晰的逻辑。
    -   建议在参考代码中添加适当注释以方便读者理解。
    -   尽量避免出现影响阅读的预编译指令和宏定义。

#### LaTeX 公式的格式要求

可参考： [OI-Wiki](https://oi-wiki.org/intro/format/#latex-%E5%85%AC%E5%BC%8F%E7%9A%84%E6%A0%BC%E5%BC%8F%E8%A6%81%E6%B1%82)

#### 对数学公式的附加格式要求

可参考： [OI-Wiki](https://oi-wiki.org/intro/format/#%E5%AF%B9%E6%95%B0%E5%AD%A6%E5%85%AC%E5%BC%8F%E7%9A%84%E9%99%84%E5%8A%A0%E6%A0%BC%E5%BC%8F%E8%A6%81%E6%B1%82)

#### 伪代码格式

可参考： [OI-Wiki](https://oi-wiki.org/intro/format/#%E4%BC%AA%E4%BB%A3%E7%A0%81%E6%A0%BC%E5%BC%8F)

#### 数学符号

可参考： [OI-Wiki](https://oi-wiki.org/intro/symbol/)

## 外部链接

-   [标点符号用法（GB/T 15834—2011）](http://www.moe.gov.cn/jyb_sjzl/ziliao/A19/201001/W020190128580990138234.pdf)
-   [维基百科：格式手册/标点符号](https://zh.wikipedia.org/wiki/Wikipedia:%E6%A0%BC%E5%BC%8F%E6%89%8B%E5%86%8C/%E6%A0%87%E7%82%B9%E7%AC%A6%E5%8F%B7)
-   [中文文案排版指北（简体中文版）](https://mazhuang.org/wiki/chinese-copywriting-guidelines/)
-   [中文文案风格指南 - PDFE GUIDELINE](https://pdfe.github.io/GUIDELINE/#/others/copywriter)
-   [一份（不太）简短的 LATEX2ε 介绍或 106 分钟了解 LATEX2ε](https://github.com/CTeX-org/lshort-zh-cn/releases)
-   [中文出版物夹用英文的编辑规范](https://www.nppa.gov.cn/nppa/contents/805/102791.shtml)

## 参考资料与注释

[^ref1]: [cstdio stdio.h namespace](https://stackoverflow.com/questions/10460250/cstdio-stdio-h-namespace)

[^ref2]: [CCF 关于恢复 NOIP 竞赛的公告 - 中国计算机学会](https://www.ccf.org.cn/c/2020-01-21/694716.shtml)

---

致谢：本页面内容参考并借鉴了 [OI-Wiki](https://oi-wiki.org) ，以帮助更好地呈现相关信息。