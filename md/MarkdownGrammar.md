---
aliases: MARKDOWN 语法
---

```dialogue
left:黑曜石
< 欢迎回到Obsidian, 今天又是有意义的一天。
right:Obsidian
> Welcome back to Obsidian! 
> What another meaningful day today!


````

## 标题语法
共六级
># 语法
>## 语法
>### 语法

## 段落语法
要创建段落，请使用空白行将一行或多行文本进行分隔。

## 换行语法
在一行的末尾添加两个或多个空格，然后按回车键,即可创建一个换行(`<br>`)。

## 强调语法
##### bold
>**important**
>important
##### italic
>*important*
##### bold&italic
>***important***
##### highlight
>==important==

## 引用语法
##### 段落引用
>sdfsd的发射点犯得上犯得上犯得上犯得上发射点
>sdfsd啊发发但是安德森发大水范德萨范德萨
>大师傅似的啊范德萨发达
##### 嵌套块引用
>important
>>important
>>>important
##### 带有其他元素的块引用
块引用可以包含其他 Markdown 格式的元素。并非所有元素都可以使用，你需要进行实验以查看哪些元素有效。
>Important
>`important`
>- important
>- important
>==important==

## 列表语法
##### 有序列表
要创建有序列表，请在每个列表项前添加数字并紧跟一个英文句点。数字不必按数学顺序排列，但是列表应当以数字 1 起始。
1. one
    - one(-之前缩进四个空格)
    - two
2. two
3. three
##### 无序列表
- one
- two
- three
##### 列表中嵌套其他元素
要在保留列表连续性的同时在列表中添加另一种元素，请将该元素缩进四个空格或一个制表符，如下例所示：
- one
    one
	three
- two
    ==two==
    >one

## 代码语法
`yes`
``yes`no`yes``

## 分割线语法
--- 
>---之后留有一个空格

## 链接语法
链接文本放在中括号内，链接地址放在后面的括号中，链接title可选。
超链接Markdown语法代码：`[超链接显示名](超链接地址 "超链接title")`
>[必应搜索](https://cn.bing.com "最好的搜索引擎")
后面的"..."内容是当鼠标悬停在链接上时的显示内容

><https://cn.bing.com>
如此也可表达链接

##### 带格式化的链接
强调链接, 在链接语法前后增加星号。 要将链接表示为代码，请在方括号中添加反引号。
><**https://cn.bing.com**>
><*https://cn.bing.com*>
>I don't like the **[Bing](http://cn.bing.com)**.
>I don't like the [`Bing`](#https://cn.bing.com).

## 图片语法
插入图片Markdown语法代码：`![图片alt](图片链接 "图片title")`。
>![picture](C:\Users\Administrator\Desktop\2050700.jpg "beauty")

## 表格语法
要添加表，请使用三个或多个连字符（`---`）创建每列的标题，并使用管道（`|`）分隔每列。您可以选择在表的任一端添加管道。
>| fruits     | animals|
>|---------|--------|
>| apple    | pig        |
>| banana | monkey|

也可以使用[Markdown Tables Generator](https://www.tablesgenerator.com/markdown_tables)快速生成表格形成markdown格式的文件嵌入obsidian中

##### 对齐方法
通过在标题行中的连字符的左侧，右侧或两侧添加冒号（`:`），将列中的文本对齐到左侧，右侧或中心。
>| fruits| animals|
>| :---| :---|
>|apple|pig|
>|banana|monkey|

##### 格式化
表格中设置文本格式。例如，可以添加链接，代码（仅反引号（`` ` ``）中的单词或短语，而不是代码块）和强调。

不能添加标题，块引用，列表，水平规则，图像或HTML标签。

## 脚注语法
 Here is a very simple footnote[^1], and here's only one simple sentence[^2]
 
 [^1]: It is vey easy. 
 [^2]: Don't you feel well

 ## 删除线语法
 ~~yes~~
 ~~       ~~
 
 ## 任务列表语法
 - [x] one
 - [ ] two
 - [ ] three

## 标签语法
#士大夫

## 块链接语法
##### 标题引用
>引用标题演示:[[Practise|TRY]]
这也是内部链接打开方法 [[3.对齐]]

##### 具体标题引用
[[]]里面用上下键浮动到某个标题上然后再按#可以链接到具体标题
在预览模式下，内部链接可以显示为其他文字。要实现这点，只需通过 `|` 来修饰内部链接。
>[[另一篇笔记名称|预览模式下显示的自定义字段]]。这可以与链接标题语法一起使用，比如[[折叠#举个例子|举个折叠的例子]]。

##### 块链接
>[[3.对齐#^0065fa]]
具体为[[xxx^xxx]]

##### 块引用
>![[3.对齐#^0065fa]]
在块链接之前加上!
下面我空一行然后用^创建一个块id方便直接引用

^6666666

![[#^6666666]]
