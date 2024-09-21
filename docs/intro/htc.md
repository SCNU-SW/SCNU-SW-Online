---
author: OI-Wiki, SCNU-SW-Online
updated: 2024/08/01
date: 2024/07/09
---

🎉👍 首先，感谢您抽出宝贵时间为 **华师手册** 做出贡献！ 🎉👍

这篇文章将主要叙述参与 **华师手册** 编写的写作过程。请您在撰稿或者修正页面之前，仔细阅读以下内容，以帮助您完成更高质量的内容。

## 参与协作

我们建议您在编辑前先考虑以下几点：

1.  **选择您熟悉的领域**：请优先编辑那些与您的专业知识、学习背景或兴趣爱好相关的条目。这有助于您创作出高质量的内容。
2.  **谨慎对待新领域**：如果您对某个主题还处于初学阶段或不太了解，建议您先通过阅读、学习加深理解，待有一定把握后再动手编辑。
3.  **查阅相关资料**：为条目添加内容或进行修订时，建议您先查阅权威文献和资料，确保信息准确无误。也欢迎您在我们的社区提出问题，与其他编者交流讨论。

## 参与方式

**如果您不太了解 Markdown 语法，或者没有 Github 账号，可以通过以下方式提交。**

1. 邮件提交

	发送邮件到 support@scnusw.online

2. 代理提交

	提交规范编写的 Word 图文给管理员，由管理员整理上传。

建议格式为：`.md` Markdown 文件或 `.docx` Word 文档，通过以上方式提交不要忘了留下你的署名哦。

**如果您想直接编辑，则需要在 Github 上提交，以下是详细的教程。**

#### 为什么要在 Github 上编辑

-   **版本控制**：使用 Git 作为版本控制系统，可追踪更改记录，还可以在需要时回滚版本，确保文档的质量和一致性。
-   **协作性强**：通过 pull request 和 issues，团队成员可以轻松地讨论、审查、修改和合并文档的更改。
-   **持续集成与部署**：支持自动化测试、构建和部署，贡献者 pull request 后可自动构建，实现预览，通过管理员审核后可自动构建整站。

### 在 GitHub 上编辑

参与 **华师手册** 的编写 **需要** 一个 GitHub 账号（可以前往 [GitHub 的账号注册页面](https://github.com/signup) 页面注册），但 **不需要** 高超的 GitHub 技巧，即使你是一名新手，只要按照下面所述的步骤操作，也能够 **非常出色** 地完成编辑。

???+ tip
    在你的更改被合并到 **华师手册** 的主仓库之前，你对 **华师手册** 的内容所作出的修改均不会出现在 **华师手册** 的主站上，所以无需担心你的修改会破坏 **华师手册** 上正在显示的内容。
    
    如果还是不放心，可以查看 [GitHub 的官方教程](https://skills.github.com/)。

#### 编辑单个页面内的内容

1.  在 **华师手册** 上找到对应页面；
2.  点击正文右上方（目录左侧）的 **:material-pencil:「编辑此页」** 按钮，在确认您已经阅读了本页面和 [格式手册](./format.md) 后点击按钮根据提示（ Fork 本项目）跳转到 GitHub 进行编辑；
3.  在编辑框内编写你想修改的内容。请注意，在修改和接下来的提交过程中，请 **关闭您的自动翻译软件**，因为它可能产生不必要的麻烦（例如您修改的文件有时会被其错误改名，从而影响目录结构）；
4.  编写完成后滚动到页面下方，按照本文中 [Commit 信息格式规范](#Commit-信息格式规范) 填写 commit 信息，之后点击 **Propose changes** 按钮提交修改。点击按钮后，GitHub 会自动帮你创建一份 **华师手册** 仓库的分支，并将你的提交添加到这个分支仓库。
5.  GitHub 会自动跳转到你的分支仓库的页面，此时页面上方会显示一个绿色的 **Create pull request** 按钮，点击后 GitHub 会跳转到一个创建 Pull Request 页面。向下滚动检查自己所作出的修改没有错误后，按照本文中 [Pull Request 信息格式规范](#Pull-Request-信息格式规范) 一节中的规范书写 Pull Request 信息，然后点击页面上的绿色的 **Create pull request** 按钮创建 Pull Request。
6.  不出意外的话，你的 Pull Request 就顺利提交到仓库，等待管理员审核并合并到主仓库中即可。

在等待合并的时间里，你可以给他人的 Pull Request 提意见、点赞或者点踩。如果有新消息，会在网页右上角出现提示，并附有邮件提醒（取决于个人设置中配置的通知方式）。

#### 编辑多个页面内的内容

如果你需要同时编辑互相无关联的多个页面的内容，请按照上方的 [编辑单个页面内的内容](#编辑单个页面内的内容) 一节一次修改所有页面。

1.  打开 [SCNU-SW/SCNU-SW-Online](https://github.com/SCNU-SW/SCNU-SW-Online) 仓库，点击键盘上的<kbd>.</kbd>按钮（或者将 URL 中的 `github.com` 更改为 `github.dev`）[^ref1]，进入 GitHub 的网页版 VS Code 编辑器；
2.  在编辑器中作出对页面源文件的更改，可以使用页面右上方的预览按钮（或按下<kbd>Ctrl+K</kbd><kbd>V</kbd>快捷键）在右侧打开预览界面；
3.  修改完成后使用左侧的 Source Control 选项卡，并按照本文中 [Commit 信息格式规范](#Commit-信息格式规范) 填写 commit 信息并提交，提交时会提示是否创建此仓库的分支，点击绿色的 **Fork Repository** 按钮即可。
4.  提交后会在网页上方的中央弹出一个提示框，在第一次的提示框内填写标题，第二次的提示框内填写此提交要提交到的仓库内分支名称，之后右下角会弹出一个提示框，内容类似于 `Created Pull Request #1 for SCNU-SW/SCNU-SW-Online.`，点击蓝字链接即可查看该 Pull Request。

#### 新增内容

1.  打开 [SCNU-SW/SCNU-SW-Online](https://github.com/SCNU-SW/SCNU-SW-Online) 仓库，点击键盘上的<kbd>.</kbd>按钮（或者将 URL 中的 `github.com` 更改为 `github.dev`）[^ref1]，进入 GitHub 的网页版 VS Code 编辑器；
2. 在您想要新增内容的分类文件夹中新建 markdown 文档，将文档内容粘贴到网页编辑器上。（或直接上传 markdown 文档）
3. 将 Markdown 文档内引用的图片上传到该分类的 `images` 文件夹中，注意在文档内引用的路径用相对路径如 `![](./images/format-1.png)` 。
4.  在编辑器中作出对页面源文件的更改，可以使用页面右上方的预览按钮（或按下<kbd>Ctrl+K</kbd><kbd>V</kbd>快捷键）在右侧打开预览界面；
5.  修改完成后使用左侧的 Source Control 选项卡，并按照本文中 [Commit 信息格式规范](#Commit-信息格式规范) 填写 commit 信息并提交，提交时会提示是否创建此仓库的分支，点击绿色的 **Fork Repository** 按钮即可。
6.  提交后会在网页上方的中央弹出一个提示框，在第一次的提示框内填写标题，第二次的提示框内填写此提交要提交到的仓库内分支名称，之后右下角会弹出一个提示框，内容类似于 `Created Pull Request #1 for SCNU-SW/SCNU-SW-Online.`，点击蓝字链接即可查看该 Pull Request。

#### 向 Pull Request 追加更改

1.  打开 [SCNU-SW-Online 的 Pull Request 列表](https://github.com/SCNU-SW/SCNU-SW-Online/pulls)，找到您提交的 Pull Request 并点击。
2.  Pull Request 页面的标题下方将会有一段例如 `<您的ID> wants to merge x commits into SCNU-SW-Online:main from <您的ID>:patch-1` 的文字，点击 `<您的ID>:patch-1` 部分。
3.  您应该会被重定向到您的分支仓库中，而且文件列表左上角的分支名称是你提交 Pull Request 的分支名称（在本示例中应为 `patch-1`）。
4.  进行您需要的更改。
    -   如果您需要编辑单个文件或多个互相无关联的页面的内容，请直接找到你要的文件并进行更改，更改完成后滚动到页面下方，按照本文中 [Commit 信息格式规范](#Commit-信息格式规范) 填写 commit 信息，之后点击 **Commit changes** 按钮提交修改。
    -   如果您需要编辑多个文件，点击键盘上的<kbd>.</kbd>按钮（或者将 URL 中的 `github.com` 更改为 `github.dev`）[^ref1]，进入 GitHub 的网页版 VS Code 编辑器并作出更改。然后使用左侧的 Source Control 选项卡，并按照本文中 [Commit 信息格式规范](#Commit-信息格式规范) 填写 commit 信息并提交修改。
5.  这时你的更改会被自动追加在您的 Pull Request 中。

### 在构建的网页中预览变更

在 Pull Request 页面下方的 Check box 提示 preview 构建完成后（一分钟左右），可访问 [preview.scnusw.online](https://preview.scnusw.online) 页面预览效果。

### 使用 Git 在本地进行编辑

???+ warning
    对于一般用户，我们更推荐使用上方所述的 GitHub 的 Web 编辑器进行编辑。

虽然大多数情况下您可以直接在 GitHub 上进行编辑，但对于一些较为特殊的情况（如需要使用 GPG 签名），我们更推荐使用 Git 在本地进行编辑。

大致流程如下：

1.  将主仓库 Fork 到自己的仓库中；
2.  将 Fork 后的分支仓库克隆（clone）到本地；
3.  在本地进行修改后提交（commit）这些更改；
4.  将这些更改推送（push）到你克隆的分支仓库；
5.  提交 Pull Request 至主仓库。

详细的操作方式可以参考 [Git](../study/dse/git.md) 页面。

#### 向 Pull Request 追加更改

在 clone 下来的本地分支仓库中继续进行修改，并提交（commit）以及推送（push）这些更改即可。你的更改会被自动追加在 Pull Request 中。

### 对于目录和引用的变更

通常情况下，如果您需要添加一个新页面，或者修改已有页面在目录中的链接，您就需要对 [`mkdocs.yml`](https://github.com/SCNU-SW/SCNU-SW-Online/blob/master/mkdocs.yml) 文件作出改动。

添加新页面可以参考既有的格式。但除非是进行重构或修正名词，否则 **我们不建议对既有页面的引用链接进行修改**，Pull Requests 中不必要的修改也将被驳回。


### Commit 信息格式规范

对于提交时需要填写的 commit 信息，请遵守以下几点基本要求：

1.  commit 摘要请简要描述这一次 commit 改动的内容。注意 commit 摘要的长度不要超过 50 字符，超出的部分会自动置于正文中。
2.  如果需要进一步描述本次 commit 内容，请在正文中详细说明。

对于 commit 摘要，推荐按照如下格式书写：

```text
<修改类型>(<文件名>): <修改的内容>
```

修改类型分为如下几类：

-   `feat`：用于添加内容的情况。
-   `fix`：用于修正现有内容错误的情况。
-   `refactor`：用于对一个页面进行重构（较大规模的更改）的情况。
-   `revert`：用于回退之前更改的情况。

### Pull Request 信息格式规范

对于 Pull Request，请遵守以下几点要求：

1.  标题请写明本次 PR 的目的（做了 **什么** 工作，修复了 **什么** 问题）。
2.  内容请简要叙述修改的内容。如果修复了一个 issue 的问题，请在内容中添加 `fix #xxxx` 字段，其中 `xxxx` 代表 issue 的编号。
3.  请您仔细阅读 [贡献指南](https://github.com/SCNU-SW/SCNU-SW-Online/blob/master/.github/CONTRIBUTING.md) 和 [社区公约](https://github.com/SCNU-SW/SCNU-SW-Online/blob/master/CODE_OF_CONDUCT.md)，并在同意后勾选 PR 模板中的框，表示您同意了以上指南和公约。

对于 Pull Request 的标题，推荐使用如下格式书写：

```plain
<修改类型>(<文件名>): <修改的内容> (<对应 issue 的编号>)
```

修改类型分为如下几类：

-   `feat`：用于添加内容的情况。
-   `fix`：用于修正现有内容错误的情况。
-   `refactor`：用于对一个页面进行重构（较大规模的更改）的情况。
-   `revert`：用于回退之前更改的情况。

示例：

-   `fix(ds/persistent-seg): 修改代码注释使描述更清晰`
-   `fix: tools/judger/index 不在目录中 (#3709)`
-   `feat(math/poly/fft): better proof`
-   `refactor(ds/stack): 整理页面内容`

## 参考资料与注释

[^ref1]: [Web-based editor - GitHub Codespaces - GitHub Docs](https://docs.github.com/en/codespaces/developing-in-codespaces/web-based-editor)

---

致谢：本页面内容参考并借鉴了 [OI-Wiki](https://oi-wiki.org) ，以帮助更好地呈现相关信息。