---
title: 动漫狂爬虫
date: 2021-06-16 10:51:06
tags:
    - Golang
    - 爬虫
photos:
---

# 介绍

> 基于 `Colly` 框架的小玩具，练手用 ( 没对多线程进行任何处理 🤧

## 源码

[cartoonmad-go](https://github.com/Nzzz964/cartoonmad-go)

# 使用

[动画狂官网](https://cartoonmad.com/)

```bash
$ ./cartoonmad-amd64_linux -h

Usage of ./cartoonmad-amd64_linux:
  -p string
    	代理 如: socks5://127.0.0.1:1089
  -r string
    	Require 目标章节 如: 1-20
  -t int
    	线程数量 默认:8 (default 8)
  -u string
    	Require cartoonmad 目标URL
```

代理支持 `http` `socks` 等

# 示例

```bash
$ ./cartoonmad-amd64_linux -u https://www.cartoonmad.com/comic/1221.html -r 1-3 -t 16

[########                                          ] 17%        22/127
[##################################################]100%       127/127
```

> PS: 下载目录在当前工作目录 `downloads` 文件夹下  

# 更新

项目已经没办法使用了，待修复
