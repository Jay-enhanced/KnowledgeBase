# Markdown 学习记录

> 参考：[Markdown官方教程](https://markdown.com.cn/ "Markdown 官方中文网站")

## 1 什么是Markdown？

Markdown是一种轻量级的标记语言，可用于在纯文本文档中添加格式化元素。

## 2 为什么要用Markdown？

Markdown在一些场景有自己独特的优势，是撰写笔记、技术总结以及案例等等的绝佳好帮手，本文就是用Markdown格式编写的。

Markdown有以下优点：

1. 专注于文字内容；
2. 语法简单，学习成本低；
3. 纯文本，易读写，版本控制系统能跟踪到修改点；
4. 渲染效果优雅，简约，强迫症的福音；
5. 跨平台。

## 3 Markdown工具

- VS Code，可以纯语法写，也可以装插件辅助；
- Typora，不想记语法，这个工具是我用过最棒的，可惜收费了。

## 4 基本语法

### 4.1 标题

格式：`n个# + space + 标题 `

| Markdown语法      | HTML语法 | 预览效果 |
| ----------------- | -------- | -------- |
| `# 一级标题`      | `<h1>一级标题</h1>` |<h1>一级标题</h1>          |
| `## 二级标题`     | `<h2>二级标题</h2>` | <h2>二级标题</h2> |
| `### 三级标题`    | `<h3>三级标题</h3>` | <h3>三级标题</h3> |
| `#### 四级标题`   | `<h4>四级标题</h4>` | <h4>四级标题</h4> |
| `##### 五级标题`  | `<h5>五级标题</h5>` | <h5>五级标题</h5> |
| `###### 六级标题` | `<h6>六级标题</h6>` | <h6>六级标题</h6> |

### 4.2 段落

行尾加上两个以上的空格表示换行。两段落之间留空一行隔开。

### 4.3 强调

粗体：文本两边添加两个`*`号，如`**粗体**`，效果：**粗体**。

斜体：文本两边添加一个`*`号，如`*斜体*`，*斜体*。

### 4.4 引用

格式：`> + space + 内容`

效果:

> 这是引用
>
> > 这是引用的引用，加一个`>`就可以了

### 4.5 列表

有序列表：`1. + space`

无序列表：`- + space`

使用`TAB`缩进可以嵌套列表。

1. 这是有序列表
   1. 这是有序的嵌套列表。

- 这是无序列表
  - 这是无序嵌套列表。

###  4.6 代码

单行代码：` `` `两个f反引号夹着的内容为单行代码；

多行代码：第一行的三个反引号后面表示语言的名字。

````markdown
```C
// this is C language
```
````

### 4.7 分割线

三个`---`。

下面是一个分割线。

---

### 4.8 链接

格式：`[名字](URL "title")`

如：[这是百度的链接](https://www.baidu.com "百度链接的title")

还可以使用尖括号`<>`将URL直接变成可以点击的地址。

如：<https://www.baidu.com>

### 4.9 图片

插入图片的格式：`![名字](路径) "title"`

如：下面是我的首页的logo。

![首页logo](../../logo.png "首页logo")

### 4.10 转义字符

有些字符会想要显示出来，需要使用转义字符，即前面加多一个反斜杠。

可做转义的字符：

| Character | Name                                                         |
| --------- | ------------------------------------------------------------ |
| \         | backslash                                                    |
| `         | backtick (see also [escaping backticks in code](https://markdown.com.cn/basic-syntax/escaping-characters.html#escaping-backticks)) |
| *         | asterisk                                                     |
| _         | underscore                                                   |
| { }       | curly braces                                                 |
| [ ]       | brackets                                                     |
| ( )       | parentheses                                                  |
| #         | pound sign                                                   |
| +         | plus sign                                                    |
| -         | minus sign (hyphen)                                          |
| .         | dot                                                          |
| !         | exclamation mark                                             |
| \|        | pipe (s                                                      |

### 4.11 内嵌HTML

Markdown可以很轻松地使用HTML标签来实现一下特定的效果。我个人一般不需要，因为这样子就失去了我对Markdown本身的理解，即学习成本低。

## 5 扩展语法

### 5.1 表格

格式如下，值得注意的是，第一行是表头，第二行是分割线，必须用三个以上的`-`来隔开。

```markdown
| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |
```

上面的代码效果如下：

| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |

如果需要对齐，用`:`放在左边或两边或右边即可。

```markdown
| Syntax      | Description |test|
| :----------- | :-----------: |--:|
| Header      | Title       |test|
| Paragraph   | Text        |test|
```

上面的代码效果如下：

| Syntax      | Description |test|
| :----------- | :-----------: |--:|
| Header      | Title       |test|
| Paragraph   | Text        |test|

### 5.2 脚注

格式：`[^1]: 这是一个脚注`

效果：

[^1]: 这是一个脚注

如果看不到，说明你的Markdown解释器不支持解析这个格式。

### 5.3 删除线

格式：`~~内容~~`

效果：~~内容~~

### 5.4 任务列表

格式：`- [x] 任务`，x表示被选中，不选中就不用x。

效果：

- [x] 被选中的任务
- [ ] 没被选中的任务

### 5.5 Emoji

格式：`:表情名字:`

如：哭:cry:

Emoji网站：[Emojipedia](https://emojipedia.org/)

