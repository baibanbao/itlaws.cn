---
title: "简码预览"
slug: "shortcodes-preview"
date: 2018-07-18
lastmod: 2018-07-18
draft: false
tags: ["hugo", "shortcodes", "Jane"]
categories: ["IT", "软件",]

menu:
  main:
    parent: "docs"
    weight: 2
---


## 简码是什么

Markdown 很精简，以至于用户有时候需要使用原生 HTML 标签实现某些内容，例如视频的 `<iframes>`。

Hugo 创建 **简码** 来克服 Markdown 过于精简的问题。

Hugo 在内容页面遇到简码（shortcodes）时会使用预设的模板去渲染。需要注意的是，模板文件使用简码是没有效果的。

更多内容，请见：https://gohugo.io/content-management/shortcodes/

<!--more-->

## 区块引用

正常的区块引用：
{{< blockquote >}}
  This is a simple quote.
{{< /blockquote >}}

作者的区块引用：
{{< blockquote author="Author2" >}}
  This is a quote with only an Author named Author2.
{{< /blockquote >}}

作者与来源的区块引用：
{{< blockquote author="Author3" source="Source" >}}
  This is a quote from Author3 and source "source."
{{< /blockquote >}}

作者与链接的区块引用：
{{< blockquote author="Author4" link="https://www.google.com" >}}
  This is a quote from Author4 and links to https://www.google.com.
{{< /blockquote >}}

作者、链接与名称的区块引用：
{{< blockquote author="Author5" link="https://www.google.com" title="Google" >}}
  This is a quote from Author5 and links to https://www.google.com with title "Google."
{{< /blockquote >}}

作者与链接超过32个字符的话，超出的部分会被省略，例如：
{{< blockquote author="Author6" link="https://twitter.com/CryptoGangsta/status/716427930126196737" >}}
  This is a quote from Author5 and links to https://twitter.com/CryptoGangsta/status/716427930126196737 which is longer than 32 characters.
  <br>And this is a new line in the quote with the HTML br tag.
{{< /blockquote >}}

Octpress 区块引用的测试在：http://octopress.org/docs/plugins/blockquote/
{{< blockquote author="@allanbranch" link="https://twitter.com/allanbranch/status/90766146063712256" >}}
  Over the past 24 hours I've been reflecting on my life & I've realized only one thing. I need a medieval battle axe.
{{< /blockquote >}}


## 音乐

{{% music "3950552" %}}

## git 代码段（gist）

可将 URL 的 用户名和 gist ID 嵌入到页面，例如：

```
{{</* gist spf13 7896402 */>}}
```

显示为：

{{< gist spf13 7896402 >}}


## Youtube

{{< youtube w7Ft2ymGmfc >}}


## Vimeo

{{< vimeo 146022717 >}}

## Youku

{{< youku XMzQ0ODUxMjM2NA >}}