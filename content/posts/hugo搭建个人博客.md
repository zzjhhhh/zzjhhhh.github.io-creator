---
title: "如何使用hugo搭建个人博客(mac os)"
date: 2020-01-14T14:05:25Z
draft: false
---

### 第一步：安装hugo
```
    brew install hugo
    hugo version
``` 
&nbsp;

### 第二步：创建新站点
```
    hugo new site username@github.io
```
&nbsp;

### 第三步：添加主题
* 下载主题并添加到theme文件夹
```
    cd username@github.io
    git init
    git submodule add https://github.com/budparr/gohugo-theme-ananke.git themes/ananke
    echo 'theme = "ananke"' >> config.toml
```
* 设置主题
```
    echo 'theme = "ananke"' >> config.toml 
```
&nbsp;
### 第四步：创建博客
```
    hugo new posts/my-first-post.md
```
新博客包含如下信息：

``` 
---
    title: "My First Post"
    date: 2019-03-26T08:47:11+01:00
    draft: true
---
```
&nbsp;
### 第五步：开启hugo服务器
``` 
    hugo server -D
```
&nbsp;
### 第六步：自定义主题

打开`config.toml`文件, 可修改语言，标题和主题。
```
    baseURL = "https://example.org/"
    languageCode = "en-us"
    title = "My New Hugo Site"
    theme = "ananke"
```
&nbsp;
### 第七步：搭建静态页面
``` 
    hugo -D
```
注意完成博客后修改头部为 `draft: false`