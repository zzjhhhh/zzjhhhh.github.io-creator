---
title: "HTML入门笔记1"
date: 2020-01-15T19:39:46Z
draft: false
---

### HTML 的诞生

Tim Berners-Lee 李爵士在 1990 年发明了 HTML (HyperText Markup Language)，WWW, HTTP 和 URL

### HTML 起手式

! + <kbd>tab</kbd> 在 vscode 中自动生成

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
</head>
<body>

</body>
</html>
```

- `DOCTYPE` - 文档类型
- `lang="en"` - 语言,可改为中国中文 "zh-CN"
- `charset="UTF-8"` -文件的字符编码，UTF-8 支持所有语言
- `<title></title>` - 网页标题

### 常用的章节标签

- `<h1>`~`<h6>` - 标题
- `<section>` - 章节
- `<article>` - 文章
- `<p>` - 段落
- `<header>` - 头部
- `<footer>` - 脚部
- `<main>` - 主要内容
- `<aside>` - 旁支内容
- `<div>` - 划分

### 常用的全局属性

所有标签都有的属性

- `class` - 标签分类
- `contenteditable` - 使内容可编辑
- `hidden` - 隐藏元素
- `id` - 标签的 id，id 必须唯一且不能等于 windows 下属性
- `style` - 文本样式，优先级高于 CSS
- `tabindex` - 默认为 0，可为负值，正值或 0

  - 负值，元素可聚焦，但不能通过<kbd>tab</kbd>访问该元素。
  - 正值，元素可聚焦，可以通过<kbd>tab</kbd>访问该元素，相对顺序按照按照 tabindex 的数值递增而滞后获焦，如果多个元素拥有相同的值，它们的相对顺序按照他们在当前 DOM 中的先后顺序决定。
  - 0 值，元素可聚焦，可以通过键盘导航来聚焦到该元素，它的相对顺序取决于当前处于的 DOM 结构。
  - 值为 0 、非法值、或者没有 tabindex 值的元素应该放置在 tabindex 值为正值的元素后面。

- `title` - 鼠标悬浮时可见，表示元素的相关信息，当元素过长带有省略号时可用于显示元素完整内容。

### 内容标签

- `<ol>` + `<li>` - Ordered list 有序列表
- `<ul>` + `<li>` - Unordered list 无序列表
- `<dl>` + `<dt>` + `<dd>` - Description list 描述列表; Description term 描述性元素，父元素为`<dl>`; Description definition 描述解释列表里的 dt，处于 `<dt>`之后，父元素为`<dl>`。
- `<pre>` - 显示文本中的空白符（空格，换行）。
- `<hr>` - Horizontal rule 水平线
- `<br>` - Break rule 换行符
- `<a href="">` - Anchor 超链接
- `<em>` - emphasis 表示语气强调
- `<strong>` - 表示内容强调
- `<code>` - 用于显示代码，使字体等宽，可与`<pre>`一起使用显示多行代码。
- `<quote>` - 内联引用
- `<blockquote>` - 块级引用
