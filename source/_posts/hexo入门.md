---
title: hexo入门
date: 2023-11-15 21:31:10
tags:
---

hexo的基本使用。

<!--more-->

## hexo安装

使用以下命令安装hexo

```
npm install -g hexo-cli
```

## 创建博客系统

```
hexo init
npm install
```

## 常用命令

- `hexo new` 创建文章
- `hexo g` 生产文章
- `hexo d ` 部署博客
- `hexo s` 启动服务器
- `hexo cl` 清楚文件

## 部署到github

在GitHub上创建一个名为**username.github.io**的仓库，然后修改根目录下的`_config.yal`文件

```yaml
# Deployment
## Docs: https://hexo.io/docs/one-command-deployment
deploy:
  type: git
  repo: git@github.com:gboomlighten/gboomlighten.github.io.git
  branch: main  
```

然后安装git部署插件

```
npm install hexo-deployer-git --save
```

通过`hexo d`即可将博客部署到GitHub，通过[https://gboomlighten.github.io/](https://gboomlighten.github.io/)访问博客。

## next主题

### next下载安装

```
npm install hexo-theme-next
```

然后修改`_config.yal`

```yaml
# Extensions
## Plugins: https://hexo.io/plugins/
## Themes: https://hexo.io/themes/
theme: hexo-theme-next
```

## 图片插入

hexo图片插入比较麻烦使用`![]()`网页无法显示图片。应该使用以下方法插入图片：

- 拖动图片到typora

- 点击缩放

- 删除文章名，仅保留图片名

- 应该还有更简单的方法

  



<img src="屏幕截图 2023-11-16 001826.png" alt="屏幕截图 2023-11-16 001826" style="zoom:40%;" />
