# Markdown!

## 1 基础

### 1.1 段落，空格，分行

#### 1.1.1 段落

段落用一个空行来分隔，例如：

```plain
ab

c1

23
```

表示为：

ab

c1

23

#### 1.1.2 空格

单独的一个分行不能分段，也不能在显示效果中分行，例如：

```plain
ab
c1
23
```

表示为：

ab
c1
23

#### 1.1.3 分行

要在显示效果中分行，可以在1.1.2的每行末加入两个空格，例如：

```plain
ab
c1
23
```

显示为：

ab  
c1  
23

### 1.2 标题

标题的语法是连续1~6个\#后面一个空格，然后加上文字。\#的数量越少，标题字号越大，$n$ 个\#就被称为 $n$ 级标题。例如，上一行的“标题”是这样写的：

```plain
### 1.2 标题
```

它是一个三级标题。

而第一行的源码是这样：

```plain
# Markdown!
```

它是一个一级标题。

这是最小的标题：

```plain
###### :\-: 表格居中标识
```

它是一个六级标题。

## 2.常用语法

### 2.1 粗体，斜体，删除线

#### 2.1.1 粗体

粗体的语法是把一段文字用左右各两个\*或\_包围起来，例如：

```plain
**这是粗体** 这不是粗体 __这也是粗体__
```

显示为：

**这是粗体** 这不是粗体 __这也是粗体__

#### 2.1.2 斜体

斜体的语法是把一段文字用左右各**一**个\*或\_包围起来，例如：

```plain
*这是斜体* 这不是斜体 _这也是斜体_
```

显示为：

*这是斜体* 这不是斜体 _这也是斜体_

另外，如果左右各三个\*或\_，就是粗偏斜体，例如：

```plain
*这是斜体* **这是粗体** ***这是粗偏斜体***
```

显示为：

*这是斜体* **这是粗体** ***这是粗偏斜体***

\*与文字之间可以不空格，而\_与文字之间必须空格。

#### 2.1.3 删除线

删除线的语法是把一段文字用左右各两个\*或\_包围起来，例如：

```plain
~~这是普通删除线~~|~~*这是删除线加斜体*~~|~~**这是删除线加粗体**~~|~~***这是删除线加粗偏斜体***~~
```

显示为：

~~这是普通删除线~~|~~*这是删除线加斜体*~~|~~**这是删除线加粗体**~~|~~***这是删除线加粗偏斜体***~~

而

```plain
~~这是普通删除线~~|*~~这是删除线加斜体~~*|**~~这是删除线加粗体~~**|***~~这是删除线加粗偏斜体~~***
```

显示效果相同。

甚至 ~~***这是删除线加粗偏斜体***~~ 还可以这样写：

```plain
*~~**这是删除线加粗偏斜体**~~*
```

或者：

```plain
**~~*这是删除线加粗偏斜体*~~**
```

但是绝对不能这样写：

```plain
*~~**这是删除线加粗偏斜体*~~**
```

效果如下：

*~~**这是删除线加粗偏斜体*~~**

还有这样：

```plain
**~~*这是删除线加粗偏斜体**~~*
```

效果如下：

**~~*这是删除线加粗偏斜体**~~*

~~呼。删除线一下子写了50行……~~

P.S. 删除线会与“一”重合，还会把“二”转换成“~~二~~”。

### 2.2 代码块

#### 2.2.1 小段代码

可以用左右各一个\`包围文字来把它放在框里，例如：

```plain
`以前显示Markdown源码都是用上下各三个 这个字符 包围的，一个的话，可用来粘贴一行代码，如 const int S[5]={0,2,4,1,3};`
```

显示为：

`以前显示Markdown源码都是用上下各三个 这个字符 包围的，一个的话，可用来粘贴一行代码，如 const int S[5]={0,2,4,1,3};`

#### 2.2.2 大段代码

代码的上一行和下一行需要各三个\`，上一行的\`右边要写上语言，如cpp，c，java，pascal等。

特别的，plain专用于粘贴非代码的文字。

例如：

```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
	int n;
	cin>>n;
	cout<<2*n;
	return 0;
}
```

### 2.3 列表

#### 2.3.1 无序列表

在每段文字前加上\*，\+，或\-，再加上一个空格，例如：

```plain
* Markdown!
* 基础
* 段落，空格，换行
- 常用语法
- 代码块
- 列表
+ 有序列表
+ 无序列表
```

显示为：

* Markdown!
* 基础
* 段落，空格，换行
- 常用语法
- 代码块
- 列表
+ 有序列表
+ 无序列表

#### 2.3.2 有序列表

在每段文字前加上数字，再加英文句点`.`和一个空格，例如：

```plain
1. a
2. b
3. c
4. d
3. e
1. f
3. g

|

3. h
3. i
```

显示为：

1. a
2. b
3. c
4. d
3. e
1. f
3. g

|

3. h
3. i

### 2.4 链接

#### 2.4.1 一种格式

格式如下：

1. `[`
2. 链接显示的一段文字
3. `](`
4. 链接地址
5. `)`

例如：

```plain
[CSDN](https://csacademy.com/app/graph_editor/)
```

显示为：

[CSDN](https://csacademy.com/app/graph_editor/)

#### 2.4.2 另一种格式

1. `<`
2. 链接地址
3. `>`

例如：

```plain
<https://floor.io/>

<https://florr.io/>
```

显示为：

<https://floor.io/>

<https://florr.io/>

P.S. 你会发现第一个网站无法打开，因为没有这个网站名。

### 2.5 分割线

一行中，当**只**有 $\ge 3$ 个\*或\-或\_时，它就会被自动识别为分割线，例如：

```plain
***
* * *
*****
***what***
---
***what***

---
-- - --
_____
***_-
***
--
___
---
*-_
***
***************************
```

显示为：

***
* * *
*****
***what***
---
***what***

---
-- - --
_____
***_-
***
--
___
---
*-_
***
***************************

### 2.6 转义字符

\\能使一些字符从特殊含义（如 _斜体_）转变成原来的字符，例如：

```plain
\\
\`
\*
\_
\{
\}
\[
\]
\(
\)
\#
\+
\-
\.
\!
```

显示为：

\\
\`
\*
\_
\{
\}
\[
\]
\(
\)
\#
\+
\-
\.
\!
