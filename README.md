# fduthesis-supplement

本仓库为[fduthesis]([https://zhuanlan.zhihu.com/p/654414894](https://github.com/stone-zeng/fduthesis))的补充，主体请先使用该仓库中的文件内容。

### 主要作用

在主体模板的基础上，提供复旦大学毕业论文盲审封面，并提供了修改版的页眉和页脚（此为可选项，可去除）。

### 使用方法-盲审封面

1. 参照[fduthesis]([https://zhuanlan.zhihu.com/p/654414894](https://github.com/stone-zeng/fduthesis))。
2. 将本仓库中的`fduthesis.cls`、`fduthesis.def`、`fduthesis-en.cls`、`main.tex`四个文件，移入你使用的LaTeX软件/网站的文件目录的根目录。
3. 如果不需要修改页眉和页脚，需要删除或注释掉`main.tex`中151-156行的源码。
```latex
\newpage
\thispagestyle{empty}  % 删除目录页的页眉
% \addtocontents{toc}{\protect\thispagestyle{empty}}
% 不插入页眉，插入页脚（罗马数字页码）
\pagestyle{plain}  % 仅显示页脚
\renewcommand{\thepage}{\roman{page}}  % 使用罗马数字页码
```

### 使用方法-页眉页脚修改

1. 完成前述的操作。
2. 在正文内容的若干个tex的第一个tex的开头，加入`example.tex`中的内容。
