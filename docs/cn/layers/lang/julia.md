---
title: "SpaceVim lang#julia 模块"
description: "这一模块为 julia 开发提供支持，包括代码补全、语法检查、代码格式化等特性。"
lang: cn
---

# [可用模块](../../) >> lang#julia

<!-- vim-markdown-toc GFM -->

- [模块简介](#模块简介)
- [功能特性](#功能特性)
- [启用模块](#启用模块)
- [快捷键](#快捷键)
  - [交互式编程](#交互式编程)
  - [运行当前脚本](#运行当前脚本)

<!-- vim-markdown-toc -->

## 模块简介

这一模块为 SpaceVim 提供了 julia 开发支持，包括代码补全、语法检查、以及代码格式化等特性。

## 功能特性

该模块主要包括插件 [julia-vim](https://github.com/JuliaEditorSupport/julia-vim)， 该插件提供：

- 语法高亮


同时，该模块还为 julia 开发提供了交互式编程和调试等功能。

## 启用模块

可通过在配置文件内加入如下配置来启用该模块：

```toml
[[layers]]
  name = "lang#julia"
```


## 快捷键

### 交互式编程

启动 `julia` 交互进程，快捷键为： `SPC l s i`。

将代码传输给 REPL 进程执行：

| 快捷键      | 描述                        |
| ----------- | --------------------------- |
| `SPC l s b` | 发送整个文件内容至 REPL |
| `SPC l s l` | 发送当前行内容至 REPL       |
| `SPC l s s` | 发送已选中的内容至 REPL     |

### 运行当前脚本

在编辑 julia 文件时，可通过快捷键 `SPC l r` 快速异步运行当前文件，运行结果会展示在一个独立的执行窗口内。
