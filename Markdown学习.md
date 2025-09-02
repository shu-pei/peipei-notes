#  Markdown笔记

使用typora学习markdown，md是一种轻量级标记语言，文档后缀是.md。

## 一、Markdown语法

#### 1.1 标题

使用#表示标题，一级标题对应一个#，至多6级标题，#之后要紧接一个空格表示标题；

也可以用快捷键 Ctrl + 0/1/2/3/4/5/6; 

#### 1.2 字体

+ 用一对星号\*扩住的文本表示斜体，如：*斜体*；

+ 也可以用一对\_扩住的文本表示斜体，如：_斜体_；

+ 也可以用快捷键Ctrl + l表示斜体；

+ 用一对\*\*扩住的文本表示粗体，如：**粗体**;

+ 也可以用一对\_\_扩住的文本表示粗体，如：__粗体__；

+ 也可以用快捷键Ctrl + B表示粗体；

+ 同理使用\*\*\*与\_\_\_表示粗斜体，如：***粗斜体***；

#### 1.3 线

+ 使用三个及以上的+号或*号或-表示一条分割线；

如：

---

+ 使用一对\~\~扩住的文本表示删除线，如：~~删除的文本~~；

+ 也可以使用Alt + Shift + 5添加删除线；

+ 使用HTML标签\<u\>和\</u\>表示下划线，如：<u>下划线</u>；

+ 也可以使用Ctrl + U表示下划线；

#### 1.4 列表

+ 使用*，+或-标记符号表示无序表项，标记符号后需紧接一个空格；

+ 使用数字加上\.再加上空格表示有序列表，并且数字并不重要；

+ 回车换行，会自动生成下一项，再回车退出当前列表，使用Tab将列表的第二项变成第一项的子列表；

#### 1.5 区块

+ 当引用他人内容时，可以使用区块，使用\>紧接空格表示区块，区块可以嵌套；

> 区块
>
> > 二级区块
> > 
>
> 

#### 1.6 代码

+ 如果是一行代码，可以使用段内代码块，用一对\`扩住代码，如： `printf("hello world")`
+ 如果是代码段，可以使用三个\`加enter/空格+编程语言表示，如：

``` C++
include<bits/stdc++.h>
using namespace std;    
```

#### 1.7 链接

+ 可以使用 \[链接名字\]\[参考链接\]\(链接地址 “可以选择的标题”\) 或者 单独显示链接 <链接地址>；
+ 锚点链接用于在同一文档内跳转，标题自动是锚点，锚点名称是空格替换为连字符，移除特殊字符；

#### 1.8 图片

+ 可以使用\!\[替代文字\]\(图片路径 “图片标题”\)，可以使用本地相对路径，确保图片的稳定；

图片尺寸控制：
```html
<img src="image.jpg" alt="描述文字" width="300" height="200">
<img src="image.jpg" alt="描述文字" width="50%">
<img src="image.jpg" alt="描述文字" style="width: 300px; height: auto;">
```

图片对齐：
```html
<!-- 居中对齐 -->
<div align="center">
  <img src="image.jpg" alt="居中图片" width="400">
</div>

<!-- 左对齐（默认） -->
<img src="image.jpg" alt="左对齐图片" style="float: left; margin-right: 20px;">

<!-- 右对齐 -->
<img src="image.jpg" alt="右对齐图片" style="float: right; margin-left: 20px;">
```

#### 1.9 表格

+ 可以使用\|来分割不同的单元格，使用\-来分隔表头和其他行；

语法格式如下：
\|表头\|表头\|
\|----\|----\|

typora自带对表格的控制，略；

## 二、数学公式

#### 2.1 LaTeX

在markdown中。数学通过LaTeX语法来表示；

基本语法：

+ 命令：以反斜杠\开头，如\alpha，\sum；

+ 参数：用花括号{}包围，如\frac{a}{b}；

+ 下标：使用_，如x_1;

+ 上标：使用^，如x^2;

#### 2.2 行内公式与块级公式

+ 行内公式使用单个美元符号$包围，公式嵌入到文本中；

+ 块级公式使用双美元符号$$包围，公司会独立成行并且居中；

+ 使用align环境创建多行对齐公式；

#### 2.3 常见LaTex表示方法

##### 基本运算符号

- 加减乘除：`+`, `-`, `\times`, `\div`
- 分数：`\frac{a}{b}` → $\frac{a}{b}$
- 根号：`\sqrt{x}`, `\sqrt[n]{x}` → $\sqrt{x}$, $\sqrt[n]{x}$
- 指数：`x^2`, `e^{i\pi}` → $x^2$, $e^{i\pi}$

##### 比较符号

- 等于：`=`, `\neq`, `\equiv` → $=$, $\neq$, $\equiv$
- 大小：`<`, `>`, `\leq`, `\geq` → $<$, $>$, $\leq$, $\geq$
- 约等于：`\approx`, `\sim` → $\approx$, $\sim$

##### 集合符号

- 属于：`\in`, `\notin` → $\in$, $\notin$
- 包含：`\subset`, `\supset` → $\subset$, $\supset$
- 交并：`\cap`, `\cup` → $\cap$, $\cup$
- 空集：`\emptyset` → $\emptyset$

##### 希腊字母

常用希腊字母及其 LaTeX 表示：

| 小写 | 大写 | LaTeX      | 小写 | 大写 | LaTeX    |
| :--- | :--- | :--------- | :--- | :--- | :------- |
| α    | Α    | `\alpha`   | ν    | Ν    | `\nu`    |
| β    | Β    | `\beta`    | ο    | Ο    | `o`      |
| γ    | Γ    | `\gamma`   | π    | Π    | `\pi`    |
| δ    | Δ    | `\delta`   | ρ    | Ρ    | `\rho`   |
| ε    | Ε    | `\epsilon` | σ    | Σ    | `\sigma` |
| θ    | Θ    | `\theta`   | τ    | Τ    | `\tau`   |
| λ    | Λ    | `\lambda`  | φ    | Φ    | `\phi`   |
| μ    | Μ    | `\mu`      | ω    | Ω    | `\omega` |

##### 特殊函数和符号

- 三角函数：`\sin`, `\cos`, `\tan`
- 对数：`\log`, `\ln`
- 极限：`\lim_{x \to 0}`
- 求和：`\sum_{i=1}^{n}`
- 积分：`\int_{a}^{b}`
- 无穷：`\infty`

##### 矩阵表示

使用 `matrix` 环境：
$$
\begin{pmatrix}
a & b \
c & d
\end{pmatrix}
$$

- `pmatrix`：圆括号 $\begin{pmatrix} a & b \ c & d \end{pmatrix}$
- `bmatrix`：方括号 $\begin{bmatrix} a & b \ c & d \end{bmatrix}$
- `vmatrix`：行列式 $\begin{vmatrix} a & b \ c & d \end{vmatrix}$

## 三、HTML





## 四、参考资料

[1] 菜鸟Markdown教程：[Markdown教程](https://www.runoob.com/markdown/md-tutorial.html)

