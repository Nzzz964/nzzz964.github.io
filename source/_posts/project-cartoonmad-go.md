---
title: cartoonmad爬虫
date: 2021-06-16 10:51:06
tags:
    - golang
    - crawler
photos:
    - /images/20210616-project-cartoonmad-go.png
---

## 介绍

> 基于**Colly**框架的小玩具

**Github源码**: [cartoonmad-go](https://github.com/Nzzz964/cartoonmad-go)

链接: [Colly 官网](http://go-colly.org/)

## 背景

初学**Golang**，为了熟悉语法与开发流程

## 使用

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

## Example

```bash
$ ./cartoonmad-amd64_linux -u https://www.cartoonmad.com/comic/1221.html -r 1-3 -t 16

[########                                          ] 17%        22/127
[##################################################]100%       127/127
```

> PS: 下载目录在当前工作目录 `downloads` 文件夹下  
