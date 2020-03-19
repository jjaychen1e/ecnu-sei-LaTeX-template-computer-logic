# ecnu-sei-LaTeX-template-computer-logic
 华东师范大学软件工程学院计算机逻辑基础课程的 LaTeX 模版

## 这是什么？

因为《计算机逻辑基础》课程中需要用到许多 `Proof Box`，但是简单的 LaTeX 是无法满足我们的需求的。教材的 `Acknowledge` 部分指出：

> We acknowledge **[Paul Taylor’s LaTeX package](https://www.paultaylor.eu/proofs/)** for proof boxes.

在其个人网站中我们可以找到作者所指的宏包，大体满足我们课程作业的需求。在此基础上进行修改，以更好更方便地帮助我们完成作业。

另外，这个包和 `ctex` 有冲突，会导致排版错乱，如果你有任何解决方案，欢迎提出 `PR`.

具体的例子参考 `example.tex` ，以及对应的 `example.pdf` 。更多细节请参考 `Paul Taylor’s LaTeX package/boxuser.pdf` 及其源码。**注意**，`example-1` 和 `example-2` 中没有使用它提供的根据标签自动生成行号的功能，因为我觉得对于作业程度的排版来说，不如直接写来得快。

## 修改日志

1. 注释缺少的宏包引用 `\usepackage{daymonthyear}`
2. 去掉其提供的 `\intro` 和 `\elim`，修改为自己的样式
3. 添加一些快捷的命令，具体如下

```latex
\def\premise{\mathrm{premise}}
\def\assumption{\mathrm{assumption}}
\def\MT{\mathrm{MT\ }}
\def\LEM{\mathrm{LEM}}
\def\intro{\mathrm{i\ }}
\def\elim{\mathrm{e\ }}
\def\introa{\mathrm{i_1\ }}
\def\elima{\mathrm{e_1\ }}
\def\introb{\mathrm{i_2\ }}
\def\elimb{\mathrm{e_2\ }}
```

