# MPU FYP Final Report LaTeX template (COMP4299/CSAI4299)

本项目是澳门理工大学 (MPU) **COMP4299/CSAI4299 Final Year Project (2026/27 学年)** Progress Report 的 LaTeX 模板。本模板旨在复刻学校官方提供的 Word 模板格式，让习惯使用 LaTeX 的同学能够更高效地进行排版和写作。

> [!WARNING]
> **免责声明 (Disclaimer)**
> 使用本模板造成的一切后果需由使用者**自行负责**。包括但不限于：
> 1. 模板中可能存在的潜在排版错误或 Bug（尽管经过检查，仍不可避免的有出现错误的可能性）；
> 2. 导师或学校最终不认可此模板生成的 PDF 格式；
> 3. 因格式问题导致的任何学术或评分影响。
> 
> 在最终提交前，请务必仔细对照学校官方最新发布的 Word/PDF 格式要求进行人工核对！

## ✨ 关于本模板

- **适用范围**：专为 MPU `COMP4299/CSAI4299` 课程，基于 Progress Report 设计。其他课程或 Final Report 的具体格式要求可能有所不同，但本模板的代码结构清晰，可作为参考或在此基础上进行修改。
- **开发方式**：本模板的底层代码与格式解析由 **Qwen3.8-Max** 大模型辅助生成，随后经过了**人工审核、细节调整与排版优化**，以确保最终输出效果高度还原 Word 原貌。
- **持续维护**：后续如发现排版错误，作者会在此仓库持续更新代码。

---

## ⚠️ 字体配置说明 (Font Setup)

由于 **Calibri** 和 **Cambria** 属于 Microsoft 商业版权字体，受许可证限制，本仓库**不包含**字体文件。

为了完美复刻 Word 原模板的排版，请您自行从操作系统中提取字体，并放入项目中。

### 获取步骤：
1. 找到本项目根目录下名为 `fonts` 的文件夹。
2. 从您的电脑系统中找到以下 8 个字体文件，并复制到 `fonts` 文件夹中：

| 字体名称 | Windows 路径 (`C:\Windows\Fonts`) | Mac 路径 (`/Library/Fonts/Microsoft/`) | 需要的文件名 |
| :--- | :--- | :--- | :--- |
| **Cambria** | 找到 Cambria 常规 | 找到 Cambria | `cambria.ttc` |
| **Cambria Bold** | | | `cambriab.ttf` |
| **Cambria Italic** | | | `cambriai.ttf` |
| **Cambria Bold Italic**| | | `cambriaz.ttf` |
| **Calibri** | 找到 Calibri 常规 | 找到 Calibri | `calibri.ttf` |
| **Calibri Bold** | | | `calibrib.ttf` |
| **Calibri Italic** | | | `calibrii.ttf` |
| **Calibri Bold Italic**| | | `calibriz.ttf` |

3. 确保您的 Overleaf 或本地编译器的 Compiler 已设置为 **XeLaTeX**。
4. 重新编译即可完美渲染。

---

## 📖 使用指南
### 1. 自动更新目录
Table of Contents、Table of Figures 和 List of Tables 会自动更新，不需要人为进行设置。

### 2. 参考文献管理 (.bib)
本模板使用独立的 `references.bib` 文件来管理参考文献，大大减少了手动排版和管理交叉引用时的工作量。
- 在正文中需要引用的地方，使用 `~\cite{引用键名}` 即可插入引用（例如：`...as shown in previous studies~\cite{abelson1985structure}.`）。
- **注意**：前面的波浪号 `~` 是一个**不可断空格**，它能防止参考文献编号（如 `[1]`）被意外换行到下一行的行首，这是 LaTeX 排版的最佳实践。

### 3. 图表与章节的交叉引用
对于图、表、段落（章节）的交叉引用，请使用 `~\ref{标签名}` 命令。
- **图表**：在 `figure` 或 `table` 环境的 `\caption{}` 下方添加 `\label{fig:my_image}`，正文中写 `As shown in Figure~\ref{fig:my_image}`。
- **章节**：在 `\section{}` 或 `\subsection{}` 下方添加 `\label{sec:intro}`，正文中写 `In Chapter~\ref{sec:intro}`。
- 同样，记得使用 `~` 来防止 "Figure 1" 或 "Chapter 2" 被从中间截断换行。

### 4. Overleaf 限制
由于免费版 Overleaf 对编译时间的限制，后期编译时间受限时可使用本地编译，或可使用中国科技云的无限制 Overleaf 服务：https://www1.cstcloud.cn/resources/452 。
