[适用软件MarkdownPad](http://markdownpad.com/ "http://markdownpad.com/")

[md官网语法速查](https://markdown.com.cn/cheat-sheet.html#%E6%80%BB%E8%A7%88 "语法总览")

## markdown标题语法

	要创建标题，请在单词或短语前面添加井号 (#) 。
	"# "的数量代表了标题的级别。并且为了兼
	容考虑，请用一个空格在 # 和标题之间
	进行分隔。

## md段落语法
我喜欢你，你喜欢我吗？
我喜欢你，你喜欢我吗？
	
	注意：不要用空格（spaces）或制表符（ tabs）缩进段落。

## md换行语法
我喜欢你，你喜欢我吗？  
我喜欢你，你喜欢我吗？

	在一行的末尾添加两个或多个空格，
	然后按回车键,即可创建一个换行(<br>)。


我喜欢你，你喜欢我吗？<br>
我喜欢你，你喜欢我吗？
	
	也可以在末尾添加html的<br>来换行
## md强调语法
### 粗体（Bold）
今天**天气**很好！

	要加粗文本，请在单词或短语
	的前后各添加两个星号。（最好
	不使用下划线形式）
### 斜体(Italic)
今天*天气*很好！

	要用斜体显示文本，请在
	单词或短语前后添加一个
	星号（最好不使用下划线
	形式）
###同时使用粗体跟斜体
今天***天气***很好！

	要同时用粗体和斜体突出显示文
	本，请在单词或短语的前后各添
	加三个星号
	
## md引用语法
	
	要创建块引用，请在段落前添
	加一个 > 符号。
>今天天气很好！  
>你好呀！  
>气压  
>温度<br>
>123

	写完一行直接回车，会在
	下一行自动创建 > 符号。
	创建新的一行可以在这一
	行的结束添加两个空格或
	者<br>
>今天天气很好！  
>你好呀！  
>>气压  
>温度<br>
>123

	嵌套块引用 >>

## md列表语法
### 有序列表
	要创建有序列表，请在每个列表
	项前添加数字并紧跟一个英文句
	点。数字不必按数学顺序排列，
	但是列表应当以数字 1 起始。

1. 123
2. 12312  
	1. 333
	2. 231
3. 12312
4. 412123

<br>

	数字英文句点之后必须接一个空格
	，才能是有序列表。第一个1.成功
	后回车会继续自动创建2. 。
	有序列表写完后需要隔一行再添加
	一个<br>空行符，否则之后会出问
	题。（有序列表未结束）

### 无序列表
	要创建无序列表，请在每个列表项前
	面添加破折号 (-)。缩进一个或多个
	列表项可创建嵌套列表。
- 123
- 321
- 333
- 222

<br>
	
	“-” 后同样需要有空格。有序列表写
	完后需要隔一行再添加一个<br>空行
	符，还需要再隔一个空行,否则之后会
	出问题。（无序列表未结束）
### 列表中嵌套其他元素
	要在保留列表连续性的同时在列表中
	添加另一种元素，请将该元素缩进四
	个空格或一个制表符。
实例：  

-   This is the first list item.
-   Here's the second list item.

    I need to add another paragraph below the second list item.

-   And here's the third list item.
-   Here's the second list item.

    > A blockquote would look great below the second list item.

-   And here's the third list item.

<br>


1.  Open the file.
2.  Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>

3.  Update the title to match the name of your website.

<br>

1. First item
2. Second item
3. Third item
    - Indented item
    - Indented item
4. Fourth item


## md代码语法
### 反引号表示代码
	要将单词或短语表示为代码，请
	将其包裹在反引号 (`) 中。(是
	esc下面的按键，与 ~ 使用一个
	按键)
At the command prompt, type `nano`.  
``Use `code` in your Markdown file.``
### 代码块
	要创建代码块，请将代码块的每一行缩
	进至少四个空格或一个制表符。（这就
	是一个代码块）
## md分割线
	要创建分隔线，请在单独一行上使用
	三个或多个星号 (***)、破折号 
	(---) 或下划线 (___) ，并且不能
	包含其他内容。

为了兼容性，请在分隔线的前后均添加空白行。

***

---

___

## md链接语法
链接文本放在中括号内，链接地址放在后面的括号中，链接title可选。

超链接Markdown语法代码：[超链接显示名](超链接地址 "超链接title")

这是一个链接 [Markdown语法](https://markdown.com.cn)。

### 给链接增加title
这是一个链接 [Markdown语法](https://markdown.com.cn "最好的markdown教程")。

### 网址和Email地址
使用尖括号可以很方便地把URL或者email地址变成可点击的链接。

<https://markdown.com.cn>  
<fake@example.com>

### 带格式化的链接
强调 链接, 在链接语法前后增加星号。 要将链接表示为代码，请在方括号中添加反引号。

I love supporting the **[EFF](https://eff.org)**.  
This is the *[Markdown Guide](https://www.markdownguide.org)*.  
See the section on [`code`](#code).  

### 引用类型链接
引用样式链接是一种特殊的链接，它使URL在Markdown中更易于显示和阅读。参考样式链接分为两部分：与文本保持内联的部分以及存储在文件中其他位置的部分，以使文本易于阅读。

#### 链接的第一部分格式
引用类型的链接的第一部分使用两组括号进行格式设置。第一组方括号包围应显示为链接的文本。第二组括号显示了一个标签，该标签用于指向您存储在文档其他位置的链接。

尽管不是必需的，可以在第一组和第二组括号之间包含一个空格。第二组括号中的标签不区分大小写，可以包含字母，数字，空格或标点符号。

以下示例格式对于链接的第一部分效果相同：

[hobbit-hole][1]  
[hobbit-hole] [1]

#### 链接的第二部分格式
引用类型链接的第二部分使用以下属性设置格式：

放在括号中的标签，其后紧跟一个冒号和至少一个空格（例如[label]:）。
链接的URL，可以选择将其括在尖括号中。
链接的可选标题，可以将其括在双引号，单引号或括号中。
以下示例格式对于链接的第二部分效果相同：

	[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle
	[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"
	[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle 'Hobbit lifestyles'
	[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle (Hobbit lifestyles)
	[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"
	[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> 'Hobbit lifestyles'
	[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> (Hobbit lifestyles)


可以将链接的第二部分放在Markdown文档中的任何位置。有些人将它们放在出现的段落之后，有些人则将它们放在文档的末尾（例如尾注或脚注）。
[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> 'Hobbit lifestyles'
#### 链接最佳实践
不同的 Markdown 应用程序处理URL中间的空格方式不一样。为了兼容性，请尽量使用%20代替空格。此软件会直接替换空格，直接复制url链接即可。

[link](https://www.example.com/my%20great%20page)

## md图片语法
要添加图像，请使用感叹号 (!), 然后在方括号增加替代文本，图片链接放在圆括号里，括号里的链接后可以增加一个可选的图片标题文本。

插入图片Markdown语法代码：![图片alt](图片链接 "图片title")。

![图片](https://markdown.com.cn/assets/img/philly-magic-garden.9c0b4415.jpg "md官网图")

### 给图片增加链接
给图片增加链接，请将图像的Markdown 括在方括号中，然后将链接添加在圆括号中。

[![沙漠中的岩石图片](https://markdown.com.cn/assets/img/philly-magic-garden.9c0b4415.jpg "Shiprock")](https://markdown.com.cn)

## md转义字符语法
[md转义字符语法][2]

[2]: https://markdown.com.cn/basic-syntax/escaping-characters.html

#扩展语法

## md表格（不支持）
[md表格](https://markdown.com.cn/extended-syntax/tables.html)

## md删除线（不支持）
[md删除线](https://markdown.com.cn/extended-syntax/strikethrough.html)

