## 字体配置说明 (Font Setup)

由于 **Calibri** 和 **Cambria** 属于 Microsoft 商业版权字体，受许可证限制，本仓库**不包含**字体文件。

为了完美复刻 Word 原模板的排版，请您自行从操作系统中提取字体，并放入项目中。

### 获取步骤：
1. 从您的电脑系统中找到以下 8 个字体文件，并复制到此 `fonts` 文件夹中：

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

2. 确保您的 Overleaf 或本地编译器的 Compiler 已设置为 **XeLaTeX**。
3. 重新编译即可完美渲染。
