---
title: git基本使用流程
toc: true
date: 2023-03-06 16:54:38
updated: 2023-03-06 16:54:38
excerpt: git基本使用流程
cover: /images/cover/640.png
thumbnail: /images/cover/640.png
categories:
- git
tags:
- git
---

### 配置代理（科学上网）

```shell
# 设置 HTTP/HTTPS 代理
git config --global http.proxy http://127.0.0.1:7890
git config --global https.proxy http://127.0.0.1:7890

# 取消代理
git config --global --unset http.proxy
git config --global --unset https.proxy

# 查看当前代理配置
git config --get http.proxy
git config --get https.proxy

# 查看所有 git 配置
git config --list
```

> ⚠️ 注意：部分情况下 https 代理可能无效，建议优先设置 http 代理。

### 配置正确显示中文路径

```shell
git config --global core.quotepath false
```

### 克隆代码

```shell
git clone git@github.com:ShawayL/HexoBlog.git
```

### 拉取代码

```shell
git pull
```

### 添加暂存区

```shell
git add .
git add [file1] [file2] ...
git add [dir]
```

### 提交暂存区文件

```shell
git commit -m "message"
```

### 推送本地提交到远程仓库

```shell
git push
```

