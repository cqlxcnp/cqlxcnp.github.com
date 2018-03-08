---
layout: post
title: jekyll本地编译错误：invalid byte sequence in GBK
key: 20180308
tags: jekyll  invalid-byte-sequence-in-GBK
---
## 错误详情
执行```bundle exec jekyll serve```时，提示：   
```shell
Liquid Exception: invalid byte sequence in GBK in _layouts/redirect.html
jekyll 3.3.1 | Error:  invalid byte sequence in GBK
```
## 解决方案
### Command Line Prompt(命令行）
执行一遍```chcp 65001```,再执行```bundle exec jekyll serve```   
### Bash Shell
```shell
export LC_ALL=en_US.UTF-8
export LANG=en_US.UTF-8
jekyll --server --auto
bundle exec jekyll serve
```