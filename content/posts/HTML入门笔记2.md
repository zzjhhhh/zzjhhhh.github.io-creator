---
title: "HTML入门笔记2"
date: 2020-01-16T12:13:09Z
draft: false
---

## a 标签

- 作用 <br>
  跳转到外部页面 <br>
  跳转到内部锚点 <br>
  跳转到邮箱或电话

- 属性

  - href

    - 网址 <br>
      https://google.com <br>
      http://google.com <br>
      //google.com

    - 路径 <br>
      /a/b/c 或 a/b/c <br>
      index.html 或 ./index.html

    - 伪协议 <br>
      JavaScript 伪协议 <br>
      mailto:邮箱 <br>
      tel:手机号

    - id
      herf=#xxx

  - target
    - \_self
    - \_blank
    - \_top
    - \_parent
    - window 的 name
    - iframe 的 name
  - download <br>
    下载页面
  - rel=noopener

## table 标签

- 相关标签

  - `<table>`
  - `<thead>`
  - `<tbody>`
  - `<tfoot>`
  - `<tr>`
  - `<th>`
  - `<td>`

- 相关样式
  - table-layout: auto; 单元格宽度取决于其包含的内容<br>table-layout: fixed; 某一列宽度取决于首行单元格的内容
  - border-collapse: collapse; 合并 border
  - border-spacing: 0; border 间距

## img 标签

- 作用 <br>
  发出 get 请求，展示一张图片

- 属性

  - alt - alternative 图片加载失败时的提示文字
  - height/width - 图片高度和宽度，只写一个图片大小自适应，都写图片会变形
  - src - 图片路径

- 事件 <br>
  onload/onerror - 图片加载成功/失败

- 响应式 <br>
  max-width: 100%; 手机响应式页面

- 可替换元素

## form 标签

- 作用 <br>
  发送 get 或 post 请求，然后刷新页面

- 属性 <br>

  - action - 请求页面的地址
  - method - 请求方法 GET / POST
  - autocomplete - 是否自动填充
  - target - 提交的页面

- 事件 <br>
  onsubmit - 用户点击提交按钮后触发的事件

- 注意事项 <br>
  form 标签中必须含有 type="submit"的标签, type 默认值为"submit"<br>
  `<input type="submit">` <input type="submit" value="搞起"><br>
  `<button type="submit"></button>`
  <button type="submit">搞起</button><br>
  button 中可包含其他内容如图片，可自定义按钮内容

## input 标签

- 作用 <br>
  使用户输入内容

- 属性 <br>
  类型 type="text"/"color"/"password"/"radio"(单选)/"checkbox"(多选)/"file"/"hidden"等等

- 事件 <br>
  onchange / onfocus / onblur

- 验证器

- 注意事项 <br>
  form 里的 input 要有 name

- 其他输入标签
  - textarea
  - select + option
  - label

## 其他标签

- video
- audio
- canvas
- svg
