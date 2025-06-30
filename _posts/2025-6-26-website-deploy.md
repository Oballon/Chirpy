---
title: "Github pages & Jekyll 部署"
categories: [技术,网站]
pin: true
---

## 方案分析

### 介绍
Github无需成本，允许用户免费建站。

[Jekyll](https://jekyllcn.com/)  为Github官方支持的静态网页生成器，可将Markdown文本转化为静态博客网站。

Ruby为jekyll、bundle的编程语言，安装Ruby后执行以下指令即可安装jekyll、bundle
```Ruby
gem install bundler jekyll
```
执行以下指令即可根据Gemfile安装项目所需的依赖
```Ruby
bundle install
```


### 关键文件介绍
_config.yml：项目总体配置，更改需重新build，文章变动无需重新build
index.html：

工作区间目录功能：
/commons：网站所需图片、文件等
/posts：文章所需图片、文件等


