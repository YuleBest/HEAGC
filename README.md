# 16进制编码+压缩加密脚本工具

## 简介

这是一个用于对Bash脚本进行16进制编码和压缩加密的工具。通过该工具，你可以将原始脚本文件转换为一个加密后的新脚本文件，该文件在执行时会自动解码并执行原始脚本内容。这种加密方式可以增加脚本的复杂度，防止未经授权的查看和执行。

## 功能特点

- **16进制编码**：将脚本内容转换为16进制格式，增加可读性难度。
- **压缩加密**：对脚本内容进行gzip压缩，进一步减小体积并增加解密难度。
- **多层数编码**：用户可以自定义编码层数，多层编码增加了脚本的加密强度。
- **进度条显示**：在处理过程中，会有彩色进度条显示当前处理进度。
- **脚本大小预估**：在编码前，工具会预估编码后脚本的大小，帮助用户决定编码层数。
- **执行权限保留**：加密后的脚本仍然保持可执行权限。

## 使用方法

1. 将此脚本保存到与需要加密的脚本同一目录下。
2. 运行此脚本，根据提示选择需要加密的脚本文件。
3. 输入新脚本保存的文件名。
4. 按照提示输入希望的编码层数。
5. 等待处理完成，最终生成加密后的脚本。

## 注意事项

- **兼容性**：加密后的脚本需要在支持`gzip`和`xxd`命令的环境中运行。
- **安全性**：虽然此工具增加了脚本的复杂度，但不应视为绝对安全，对于敏感数据请使用专业的加密工具。
- **大小限制**：过多的编码层数可能会导致脚本体积显著增加，请根据预估结果合理选择层数。

## 作者

由酷安用户 [@于乐Yule](http://www.coolapk.com/u/18214705) 和 [@王哪摸](http://www.coolapk.com/u/552579) 共同开发。

## 更新日志（详见 [Releases](https://github.com/YuleBest/HEAGC/Releases)）

- 初始版本：提供基本的16进制编码和压缩加密功能。
- v1.9~v2.0：
  1. 加入了gzip 压缩
  2. 优化交互逻辑、显示美观度
  3. 检测与脚本同目录下的脚本文件
  4. 对解码部分进行了混淆
  5. 文件的大小测试环节使用了计算方法得出
  6. 加入了进度条动画
  7. 代码方面，不再对代码进行加密
  8. 代码方面，更改大部分变量名，对大部分代码进行了注释，使代码更容易阅读
  9. 详见 [Release](https://github.com/YuleBest/HEAGC/Releases)

## 联系方式

如有任何问题或建议，请通过酷安私信联系 [@于乐Yule](http://www.coolapk.com/u/18214705) 或 [@王哪摸](http://www.coolapk.com/u/552579)。
