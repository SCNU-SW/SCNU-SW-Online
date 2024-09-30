---
title: Edit landing
author: 
updated: 2024/09/29
date: 2024/07/09
description: 编辑华师手册前需要了解的注意事项和步骤。
---

## 编辑前须知

首先，感谢您愿意为 **华师手册** 做出贡献。

请您在提交拉取请求（Pull Request）前，我们需要您了解并熟知 **[如何参与](./intro/htc.md)** 和 **[格式手册](./intro/format.md)** 里的内容。

如果有关内容**尚未完成**，请考虑先新建 issue 或本次作为 draft pr 提交。

如果内容**已经完成**，您无需新建 issue ，但仍需要核对 **[格式手册](./intro/format.md)** 提到的基本格式要求。在 **[预览网页](https://preview.scnusw.online)** 构建完成后，建议您检查实际效果，并持续跟进审核或修改意见。

在提交 pull request 时，确保**您已知晓**：

+ 请在回应建议、问题或 pull request 之前仔细阅读，并详细说明自己的看法，以免引起不必要的误会。

+ 请跟进您的 pull request。如您的 pull request 长时间没有回应修改请求，可能会被直接关闭。

在阅读完之后，请点击下方的按钮，然后开始在 Github 上编辑。

???+ 敬请留意
	- 请您记得在文件头的 author 字段后方留下你的署名
	- 在致谢页 `ack.md` 中的贡献者部分，可附上指向您个人的链接

<a id="btn-startedit" style="padding: 0.75em 1.25em; display: inline-block; line-height: 1; text-decoration: none; white-space: nowrap; cursor: pointer; border: 1px solid #6190e8; border-radius: 5px; background-color: #6190e8; color: #fff; outline: none; font-size: 0.75em;">开始编辑</a>


<script>
	function getQueryVariable(name, dft)
	{
		var reg = new RegExp('(^|&)' + name + '=([^&]*)(&|$)', 'i');
		var r = window.location.search.substr(1).match(reg);
		if (r != null)
		{
			return unescape(r[2]);
		}
		return dft;
	}
	document.getElementById("btn-startedit").href = "https://github.com/SCNU-SW/SCNU-SW-Online/edit/main/docs" + getQueryVariable("ref", "");
</script>

