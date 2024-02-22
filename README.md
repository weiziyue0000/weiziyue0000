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
