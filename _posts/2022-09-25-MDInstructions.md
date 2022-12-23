---
layout:     post
title:      Markdown 基本语法
subtitle:   MarkDown使用指北（1）
date:       2022-09-25
author:     Tresol
header-img: "img/img7.jpg"
catalog: true
tags:
    - 笔记
    - 计算机语言
    - Markdown
---

# 前言

作为Markdown小白，本篇文章改编自据说是[Markdown官方网站](http://markdown.com.cn)的《基本语法》，补充、删除了一部分内容。

`注意`：本文仅介绍Markdown语言，不涉及其他轻量级标记语言，请注意。

# Markdown 基本语法

Markdown是一种轻量级标记语言，排版语法简洁，让人们更多地关注内容本身而非排版。它使用易读易写的纯文本格式编写文档，可与HTML混编，可导出 HTML、PDF 以及本身的 .md 格式的文件。因简洁、高效、易读、易写，Markdown被大量使用，如[Github](http://github.com/)、[Wikipedia](https://www.wikipedia.ch/)、[简书](https://www.jianshu.com)等。

### Markdown 标题语法

要创建标题，请在单词或短语前面添加井号 (`#`) 。`#` 的数量代表了标题的级别。例如，添加三个 `#` 表示创建一个三级标题 (等同于HTML中的`<h3>`) (例如：`### My Header`)。
    
还可以在文本下方添加任意数量的 `==` 号来标识一级标题，或者 `--` 号来标识二级标题。

### Markdown 段落

要创建段落，请使用空白行将一行或多行文本进行分隔。不要用空格（Space）或制表符（Tabs）缩进段落。

### Markdown 换行语法

在一行的末尾添加两个或多个空格，然后按回车键，即可创建一个换行(`<br>`)。这种换行方式被称为**结尾空格**。为了兼容性，请在行尾添加“结尾空格”或 HTML 的 `<br>` 标签来实现换行。

### Markdown 强调语法

#### 粗体

要加粗文本，请在单词或短语的前后各添加两个`*`或下划线`_`。为了兼容性，如需加粗一个单词或短语的中间部分用以表示强调的话，请在要加粗部分的两侧各添加两个`*`，而不可以使用`_`。

```
**Tresol**
__Tresol__
我的**博客**。
```

效果：

**Tresol**

我的**博客**。

#### 斜体

要用斜体显示文本，请在单词或短语前后添加一个星号`*`或`_`。要斜体突出单词的中间部分，请在字母前后各添加一个`*`，中间不要带空格。

```
本代码为 *斜体* 示范。
本代码为 _斜体_ 示范。
本代码为*斜体*示范。
```

效果：

本代码为 *斜体* 示范。

本代码为*斜体*示范。

#### 粗体和斜体

要同时用粗体和斜体突出显示文本，请在单词或短语的前后各添加三个`*`或`_`。为了兼容性，要加粗并用斜体显示单词或短语的中间部分，请在要突出显示的部分前后各添加三个`*`，中间不要带空格。

```
***Tresol***
___Tresol___
我的***博客***。
```

***Tresol***

我的***博客***。

### Markdown 引用语法

要创建块引用，请在段落前添加一个 `>` 符号。

```
> Tresol Blog，我的博客。
```

渲染效果如下所示：

> Tresol Blog，我的博客。

#### 多个段落的块引用

块引用可以包含多个段落。为段落之间的空白行添加一个 `>` 符号。

```
> Tresol Blog，我的博客。
>
> 欢迎来到Tresol Blog。
```

渲染效果如下：

> Tresol Blog，我的博客。
>
> 欢迎来到Tresol Blog。

#### 嵌套块引用

块引用可以嵌套。在要嵌套的段落前添加一个 `>>` 符号。

```
> Tresol Blog，我的博客。
>
>> 欢迎来到Tresol Blog。
```

渲染效果如下：

> Tresol Blog，我的博客。
>
>> 欢迎来到Tresol Blog。

#### 带有其它元素的块引用

块引用可以包含其他 Markdown 格式的元素。并非所有元素都可以使用，你需要进行实验以查看哪些元素有效。

```
> - C++是一门严谨的计算机语言。
> - Python具有通俗、易于使用的特点。
>
>  你可以在[GitHub](http://github.com)上找到*很多*的**C++**代码。
```
渲染效果如下：

> - C++是一门严谨的计算机语言。
> - Python具有通俗、易于使用的特点。
>
>  你可以在[GitHub](http://github.com)上找到*很多*的**C++**代码。

在块引中可以包含“标题”元素。

### Markdown 列表语法

可以将多个条目组织成有序或无序列表。

#### 有序列表

要创建有序列表，请在每个列表项前添加数字并紧跟一个英文句点。数字不必按数学顺序排列，但是列表应当以数字 1 起始。

```
1. 这是一个列表（第一项）。
2. 这是一个列表（第二项）。
3. 这是一个列表（第三项）。
4. 这是一个列表（第四项）。

1. 这是一个列表（第一项）。
1. 这是一个列表（第二项）。
1. 这是一个列表（第三项）。
1. 这是一个列表（第四项）。

1. 这是一个列表（第一项）。
8. 这是一个列表（第二项）。
3. 这是一个列表（第三项）。
5. 这是一个列表（第四项）。
```

渲染效果：

1. 这是一个列表（第一项）。
8. 这是一个列表（第二项）。
3. 这是一个列表（第三项）。
5. 这是一个列表（第四项）。

```
1. 这是一个列表（第一项）。
2. 这是一个列表（第二项）。
3. 这是一个列表（第三项）。
    1. 这是一个列表（第3.1项）。
    2. 这是一个列表（第3.2项）。
4. 这是一个列表（第四项）。
```

渲染效果：

1. 这是一个列表（第一项）。
2. 这是一个列表（第二项）。
3. 这是一个列表（第三项）。
    1. 这是一个列表（第3.1项）。
    2. 这是一个列表（第3.2项）。
4. 这是一个列表（第四项）。

为了确保兼容性，请不要使用 `()`。

#### 无序列表

要创建无序列表，请在每个列表项前面添加破折号 (`-`)、星号 (`*`) 或加号 (`+`) 等标记符。缩进一个或多个列表项可创建嵌套列表。

为了确保兼容性，请在每一列表中使用同一个标记符。

```
- 这是一个列表（第一项）。
- 这是一个列表（第二项）。
- 这是一个列表（第三项）。
- 这是一个列表（第四项）。

* 这是一个列表（第一项）。
* 这是一个列表（第二项）。
* 这是一个列表（第三项）。
* 这是一个列表（第四项）。

+ 这是一个列表（第一项）。
+ 这是一个列表（第二项）。
+ 这是一个列表（第三项）。
+ 这是一个列表（第四项）。
```

渲染效果：

+ 这是一个列表（第一项）。
+ 这是一个列表（第二项）。
+ 这是一个列表（第三项）。
+ 这是一个列表（第四项）。

```
- 这是一个列表（第一项）。
- 这是一个列表（第二项）。
- 这是一个列表（第三项）。
    - 缩进项1
    - 缩进项2
- 这是一个列表（第四项）。
```

渲染效果：

- 这是一个列表（第一项）。
- 这是一个列表（第二项）。
- 这是一个列表（第三项）。
    - 缩进项1
    - 缩进项2
- 这是一个列表（第四项）。

要在保留列表连续性的同时在列表中添加另一种元素，请将该元素缩进四个空格或一个制表符，如下例所示：

```
- 这是一个列表（第一项）。
- 这是一个列表（第二项）。

    我想在这里插入一个段落。
    
    > 我想在这里插入一个引用。

- 这是一个列表（第三项）。
```

渲染效果：

- 这是一个列表（第一项）。
- 这是一个列表（第二项）。

    我想在这里插入一个段落。
    
    > 我想在这里插入一个引用。

- 这是一个列表（第三项）。

#### 代码块

代码块通常采用四个空格或一个制表符缩进。当它们被放在列表中时，请将它们缩进八个空格或两个制表符。

```
1. 欢迎来到Tresol的博客。
2. 插入代码：

        include<bits/stdc++.h>
        using namwspace std;
        int main(){
            cout<<"Welcome to Tresol Blog!";
            return 0;
        }

3. 结束！
```

渲染效果：

1. 欢迎来到Tresol的博客。
2. 插入代码：

        include<bits/stdc++.h>
        using namwspace std;
        int main(){
            cout<<"Welcome to Tresol Blog!";
            return 0;
        }

3. 结束！

无序列表和有序列表可以混用。

### Markdown 代码语法

要将单词或短语表示为代码，请将其包裹在反引号`` ` ``中。

```
在C++中，一个重要的代码便是` Using namespace std `。
```

渲染效果：

在C++中，一个重要的代码便是` Using namespace std `。

#### 转义反引号

如果你要表示为代码的单词或短语中包含一个或多个反引号，则可以通过将单词或短语包裹在双反引号` `` `中。

```
`` Tresol `Blog` ``
```

渲染效果：

`` Tresol `Blog` ``

#### 代码块

要创建代码块，请将代码块的每一行缩进至少四个空格或一个制表符。

```
    <html>
      <head>
      </head>
    </html>
```

渲染效果如下：

    <html>
      <head>
      </head>
    </html>

### Markdown 分隔线语法

要创建分隔线，请在单独一行上使用三个或多个星号 (`***`)、破折号 (`---`) 或下划线 (`___`) ，并且不能包含其他内容。为了兼容性，请在分隔线的前后均添加空白行。

```
****************
________________
----------------
```

渲染效果：

****************

### Markdown 链接语法

链接文本放在中括号内，链接地址放在后面的括号中，链接标题可选。

超链接Markdown语法代码：`[超链接显示名](超链接地址 "超链接标题")`

对应的HTML代码：`<a href="超链接地址" title="超链接title">超链接显示名</a>`

```
这是一个链接 [Tresol Blog](https://tresol.github.io)。
```
渲染效果如下：

这是一个链接 [Tresol Blog](https://tresol.github.io)。

#### 给链接增加标题

链接标题是当鼠标悬停在链接上时会出现的文字，这个标题是可选的，它放在圆括号中链接地址后面，跟链接地址之间以空格分隔。

```
这是一个链接 [Tresol Blog](https://tresol.github.io "Tresol的博客")。
```

渲染效果如下：

这是一个链接 [Tresol Blog](https://tresol.github.io "Tresol的博客")

#### 网址和Email地址

使用尖括号可以很方便地把URL或者email地址变成可点击的链接。

```
<https://tresol.github.io>
<tresol@163.com>
```

渲染效果如下：

<https://tresol.github.io>

<tresol@163.com>

#### 带格式化的链接

强调链接, 在链接语法前后增加星号。要将链接表示为代码，请在方括号中添加反引号。

```
我热衷于支持 **[EFF](https://eff.org)**。

这是*[Tresol Blog](https://tresol.github.io)*。
```
渲染效果如下：

我热衷于支持 **[EFF](https://eff.org)**。

这是 *[Tresol Blog](https://tresol.github.io)* 。

#### 引用类型链接

引用样式链接是一种特殊的链接，它使URL在Markdown中更易于显示和阅读。参考样式链接分为两部分：与文本保持内联的部分以及存储在文件中其他位置的部分，以使文本易于阅读。

##### 链接的第一部分格式

引用类型的链接的第一部分使用两组括号进行格式设置。第一组方括号包围应显示为链接的文本。第二组括号显示了一个标签，该标签用于指向您存储在文档其他位置的链接。尽管不是必需的，可以在第一组和第二组括号之间包含一个空格。第二组括号中的标签不区分大小写，可以包含字母，数字，空格或标点符号。以下示例格式对于链接的第一部分效果相同：

```
[hobbit-hole][1]
[hobbit-hole] [1]
```

##### 链接的第二部分格式

引用类型链接的第二部分使用以下属性设置格式：

放在括号中的标签，其后紧跟一个冒号和至少一个空格（例如`[label]:`）。链接的URL，可以选择将其括在尖括号中。链接的可选标题，可以将其括在双引号，单引号或括号中。以下示例格式对于链接的第二部分效果相同：

```
[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle
[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"
[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle 'Hobbit lifestyles'
[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle (Hobbit lifestyles)
[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"
[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> 'Hobbit lifestyles'
[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> (Hobbit lifestyles)
```

可以将链接的第二部分放在Markdown文档中的任何位置。有些人将它们放在出现的段落之后，有些人则将它们放在文档的末尾（例如尾注或脚注）。

为了兼容性，请尽量使用`%20`代替空格。

### Markdown 图片语法

要添加图像，请使用感叹号 (`!`), 然后在方括号增加替代文本，图片链接放在圆括号里，括号里的链接后可以增加一个可选的图片标题文本。

插入图片Markdown语法代码：`![图片提示词](图片链接 "图片标题")`。

对应的HTML代码：`<img src="图片链接" alt="图片提示词" title="图片标题">`

```
![这是图片](/assets/img/philly-magic-garden.jpg "Magic Gardens")
```

#### 链接图片

给图片增加链接，请将图像的Markdown 括在方括号中，然后将链接添加在圆括号中。

```
[![图片](/assets/img/shiprock.jpg "Shiprock")](https://tresol.github.io)
```

### Markdown 转义字符语法

要显示原本用于格式化 Markdown 文档的字符，请在字符前面添加反斜杠字符 `\` 。

```
\* 给图片增加链接，请将图像的Markdown 括在方括号中，然后将链接添加在圆括号中。
```

渲染效果如下：

\* 给图片增加链接，请将图像的Markdown 括在方括号中，然后将链接添加在圆括号中。

#### 可做转义的字符

以下列出的字符都可以通过使用反斜杠字符从而达到转义目的。

```
\	`	*	_	{ }	[ ]	( )	#	+	-	.	!	|	
```
### 特殊字符自动转义
在 HTML 文件中，有两个字符需要特殊处理： `<` 和 `&` 。 `<` 符号用于起始标签，`&` 符号则用于标记 HTML 实体，如果你只是想要使用这些符号，你必须要使用实体的形式，像是 `&lt`; 和 `&amp`;。

在HTML中，`&`必须写成`&amp`。但是，Markdown 允许你直接使用这些符号。如果你使用 `&` 符号的作为 HTML 实体的一部分，那么它不会被转换，而在其它情况下，它则会被转换成 `&amp;`。所以你如果要在文件中插入一个著作权的符号，你可以写`&copy;`，Markdown 将不会对这段文字做修改，但是如果你写`AT&T`，Markdown 就会将它转为`AT&amp;T`。类似的状况也会发生在 `<` 符号上，因为 Markdown 支持行内 HTML ，如果你使用 `<` 符号作为 HTML 标签的分隔符，那 Markdown 也不会对它做任何转换，但是如果你写`4 < 5`，Markdown 将会把它转换为`4 &lt; 5`

需要特别注意的是，在 Markdown 的块级元素和内联元素中， `<` 和 `&` 两个符号都会被自动转换成 HTML 实体，这项特性让你可以很容易地用 Markdown 写 HTML。

### Markdown 内嵌 HTML 标签

对于 Markdown 涵盖范围之外的标签，都可以直接在文件里面用 HTML 本身。如需使用 HTML，不需要额外标注这是 HTML 或是 Markdown，只需 HTML 标签添加到 Markdown 文本中即可。

#### 行级內联标签

HTML 的行级內联标签如 `<span>`、`<cite>`、`<del>` 不受限制，可以在 Markdown 的段落、列表或是标题里任意使用。依照个人习惯，甚至可以不用 Markdown 格式，而采用 HTML 标签来格式化。例如：如果比较喜欢 HTML 的` <a>` 或` <img> `标签，可以直接使用这些标签，而不用 Markdown 提供的链接或是图片语法。当你需要更改元素的属性时（例如为文本指定颜色或更改图像的宽度），使用 HTML 标签更方便些。

HTML 行级內联标签和区块标签不同，在內联标签的范围内， Markdown 的语法是可以解析的。

```
<em>欢迎来到</em> **Tresol Blog**。
```

渲染效果如下:

<em>欢迎来到</em> **Tresol Blog**。

#### 区块标签

区块元素，比如 `<div>`、`<table>`、`<pre>`、`<p>`等标签，必须在前后加上空行，以便于内容区分。而且这些元素的开始与结尾标签，不可以用 tab 或是空白来缩进。Markdown 会自动识别这区块元素，避免在区块标签前后加上没有必要的` <p> `标签。

例如，在 Markdown 文件里加上一段 HTML 表格：

```
这是正常的段落。

<table>
    <tr>
        <td>Tresol</td>
    </tr>
</table>

这是正常的段落。
```

请注意，Markdown 语法在 HTML 区块标签中将不会被进行处理。例如，你无法在 HTML 区块内使用 Markdown 形式的**强调**。

出于安全原因，并非所有 Markdown 应用程序都支持在 Markdown 文档中添加 HTML。如有疑问，请查看相应 Markdown 应用程序的手册。某些应用程序只支持 HTML 标签的子集。

对于 HTML 的块级元素 `<div>`、`<table>`、`<pre>`、`<p>`，请在其前后使用空行与其它内容进行分隔。尽量不要使用制表符或空格对 HTML 标签做缩进，否则将影响格式。

在 HTML 块级标签内不能使用 Markdown 语法。例如 `<p>**Tresol**</p>` 将不起作用。