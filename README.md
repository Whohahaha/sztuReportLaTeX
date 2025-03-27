# labreport 宏包

`labreport.sty` 是一个专为撰写中文实验报告设计的 LaTeX 宏包，集成了中文排版、美观边框、标题样式、页眉页脚、自定义字体等功能，适用于工科、医学、计算机等专业的实验报告格式统一化。

> 当前版本：v1.7  
> 最近更新：2025-03-16  
> ⚠️ 当前版本仅支持 macOS 系统，尚未适配 Windows 下的字体环境

---

## 🎯 功能亮点

- A4 页面 + 自定义边距 + 页边框（0.5 磅）
- 支持中文宋体、黑体，避免斜体错误调用
- 一级标题使用中文编号（如：一、二、三、）
- 页脚页码自动设置（默认从第 2 页开始）
- 支持代码高亮（基于 `minted` + Pygments）
- 内置常用宏包：图表、表格、美化、数学、浮动体等

---

## 📦 安装方式

### 1. 下载宏包

你可以克隆或下载此仓库：

```bash
git clone https://github.com/your-username/labreport.git

将 labreport.sty 文件复制到你的 LaTeX 项目根目录中，或安装到本地 texmf 路径中。

2. LaTeX 环境要求
	•	TeX 发行版：建议使用 MacTeX（macOS 用户）
	•	编译方式：使用 XeLaTeX（支持中文字体）
	•	代码高亮依赖：
	•	安装 minted 宏包（MacTeX 通常已内置）
	•	安装 Python 工具 Pygments：

pip install Pygments



⸻

🔧 依赖宏包列表（自动加载）

下列宏包大部分由 TeX Live / MacTeX 默认提供：

宏包名称	用途说明
geometry	页面尺寸和边距控制
xeCJK	中文字体支持（需 XeLaTeX）
titlesec	自定义标题格式
zhnumber	中文数字编号（章节编号）
fancyhdr	页眉页脚样式控制
tikz + eso-pic	添加页边框
graphicx	插图支持
subcaption	子图排版
booktabs	表格美化
array	表格扩展
caption	自定义图表标题
amsmath	数学公式
fix-cm	字体大小微调
float	控制浮动体
minted	代码高亮（需 Python 和 Pygments）



⸻

🚫 系统兼容性

本宏包当前仅在 macOS 下开发测试，默认使用系统字体：
	•	宋体：Songti SC
	•	黑体：PingFang SC

⚠️ 在 Windows 或 Linux 下，默认字体可能不存在，需手动修改 \setCJKmainfont 和 \setCJKfamilyfont 行。

⸻

✍️ 使用示例

\documentclass{article}
\usepackage{labreport}

\begin{document}

\section{实验目的}
掌握数字电路设计流程，理解时序逻辑基本原理。

\subsection{实验内容}
使用 Verilog HDL 编写计数器模块，并在 FPGA 板上验证功能。

\end{document}



⸻

📄 许可证（License）

本项目基于 MIT License 开源：

Copyright (c) 2025 徐颢然

Permission is hereby granted, free of charge, to any person obtaining a copy...
[以下略，请参见 LICENSE 文件完整内容]



⸻

📬 联系方式

作者：徐文宇（Nathan）
邮箱：whohahaha@outlook.com

欢迎提出建议与改进意见，欢迎 Star 🌟 或 Fork 本项目！
