---
title: Edit landing
author: 
updated: 2024/08/01
date: 2024/07/09
---

## 编辑前须知

首先，感谢您愿意为 **华师手册** 做出贡献。



???+ 敬请留意
	- 请您记得在文件头的 author 字段后方留下你的署名

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

