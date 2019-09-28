# markdown的基本语法测试
介绍markdown的基本语法。
如果使用Pycharm编辑器可以在 File->Settting->Plugins中搜索MarkDown support安装。
>详情见[markdown guide](https://www.markdownguide.org/basic-syntax/)

## 标题
一级标题，使用一个#，两级标题使用##，三级标题使用###，以此类推

## 段落
需要一个空白行分割前面的内容，不需要新的段落不需要增加使用空格或Tab键进行缩进

## 换行
换行是在每行后输入两个或多个空格，建议pycharm直接使用Tab键，在回车    
已经换行了。

## 标记重点
### 加粗
使用四个星号将内容加粗的内容括起来。

输入：
```
**Good**
```
输出：
> **Good**


### 斜体字
使用两个星号将需要进行斜体的内容括起来。
输入：
```
*Good*
```  
输出:     
> *Good*


### 加粗并倾斜
使用6个星号将需要加粗和倾斜的内容括起来。
输入：
```
***Good***
```
输出：
> ***Good***


## 块级引用
使用'>'进行块引用。     
输入：
```
> sdfsadlsdfasdfsafasadfasdfasdfssdfasfasdfasdfasdfasd
> 
> asdfasdfasdf asdfasdfasdfasdf
``` 
输出：     
>> sdfsadlsdfasdfsafasadfasdfasdfssdfasfasdfasdfasdfasd
>> 
>> asdfasdfasdf asdfasdfasdfasdf


### 镶嵌的块引用
块引用可以包含其他块引用。   
输入：
```
> sdfasdfasldfasls
>
>> asfasdfasdfasdsdflsdfsf
```
输出：
>> sdfasdfasldfasls
>>
>>> asfasdfasdfasdsdflsdfsf


### 块应用可以包含其他的元素
输入：
```
> #### 标题-块引用
>
> - 项目1
> - 项目2
>
> *项目总结*

```
输出：
> #### 标题-块引用
>
> - 项目1
> - 项目2
>
> *项目总结*


## 代码
使用``插入代码。
输入：
```
`name = 1`
```
输出：
> `name = 1`


### 代码块
每行使用至少4个空格缩进或者一个Tab键缩进。
输入：
```

    a = 1
    b = 2
    c = 2
    for i in range(2):
        print(i)
```
输出：

>     a = 1
>     b = 2
>     c = 2
>     for i in range(2):
>         print(i)

另类写法，采用``` ```的形式。    
输入：     
\`\`\`  
a = 1   
\`\`\`      

输出：
```
a = 1
```

## 水平线规则
使用三个或三个以上的星号或下划线。
输入：  
```
***
```   

输出：
***

或者输入：     
```
___
```

输出
___


## 添加链接
如给“百度”这两个字添加链接。
输入：     
```
网址链接：[百度](https://www.baidu.com)
```

输出：     
> 网址链接：[百度](https://www.baidu.com)

### 给链接添加标题
```
网址链接是：[百度](https://www.baidu.com "太菜")
```

> 网址链接是：[百度](https://www.baidu.com "太菜")

### URL和电子邮件地址
使用<>将URL或者电子邮件包括起来
输入：
```
<http://www.baidu.com>     
<fake@example.com>
```

输出： 
> <http://www.baidu.com>     
> <fake@example.com>

### 格式化链接
可以使用标记重点的方式格式化链接。
输入：
```
This is the **[Markdown Guide](https://www.markdownguide.org)**.    
This is the *[Markdown Guide](https://www.markdownguide.org)*.  
This is the ***[Markdown Guide](https://www.markdownguide.org)***.
```   

输入：     
> This is the **[Markdown Guide](https://www.markdownguide.org)**.    
> This is the *[Markdown Guide](https://www.markdownguide.org)*.  
> This is the ***[Markdown Guide](https://www.markdownguide.org)***.


### 参考风格的链接
这种类型的链接包含两个部分，一个是文本，一个是存放的位置。
输入：
```
In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends
of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to
eat: it was a [hobbit-hole][1], and that means comfort.

[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"
```

输出：     
> In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole,
> filled with the ends of worms and an oozy smell, nor yet a dry, bare, 
> sandy hole with nothing in it to sit down on or to eat: it was a 
> [hobbit-hole][1], and that means comfort.

[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"

使用带标题的链接同样可以实现以上效果。
输入：  
 ```
In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends
of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to
eat: it was a [hobbit-hole](https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"), 
and that means comfort.
 ```
 
 输出：    
> In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole,
> filled with the ends of worms and an oozy smell, nor yet a dry, bare, 
> sandy hole with nothing in it to sit down on or to eat: it was a 
> [hobbit-hole](https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"), 
> and that means comfort.

## 图片
使用![]来引用图片。     
输入：
```
![This place was so cool!](test.bmp "Cool")
``` 

输出：
> ![This place was so cool!](test.bmp "Cool")

### 为图片添加链接
在图片的引用放入链接的[]中即可，
输入：
```
[![An old rock in the desert](test.bmp "百度图片")](https://www.baidu.com)
```

输出：
> [![An old rock in the desert](test.bmp "百度图片")](https://www.baidu.com)


##转义符号“\”
输入：    
```
* abc

\* abc
```
输出： 
> * abc

> \* abc


## 列表
###有序列表
有序列表指带有数字需要的列,列的第一行必须为1，后面的数字不固定
```
1. 条目1
1. 条目2
1. 条目3
    1. 二级条目1
    2. 二级条目2
1. 条目4
5. 条目5
7. 条目6
```

输出：
> 1. 条目1
> 1. 条目2
> 1. 条目3
>     1. 二级条目1
>     2. 二级条目2
> 1. 条目4
> 5. 条目5
> 7. 条目6


### 无序列表
无需列表使用-、+或*

输入:
```
- 条目1
- 条目2
    - 条目
    - 条目
+ 条目3
+ 条目4
    + 条目
    + 条目
    
* 条目5
* 条目6
    * 条目5
    * 条目6
```

输出：
> - 条目1
> - 条目2
>     - 条目
>     - 条目
> + 条目3
> + 条目4
>     + 条目
>     + 条目
>    
> * 条目5
> * 条目6
>    * 条目5
>    * 条目6


### 添加其他元素进入列表
#### 段落进入列表
 在一个条目后回车空白行后增加4个空格或者一个Tab键回车后输入段落内容
输入：
```
- 条目1
- 条目2

    段落手动阀手动阀
    
- 条目3
```
输出：
> - 条目1
> - 条目2
>
>    段落手动阀手动阀
>    
>- 条目3


#### 块引用进入条目列表
```
- 条目1
- 条目2
> 段落手动阀手动阀   
- 条目3
```

输出：
> - 条目1
> - 条目2
> > 段落手动阀手动阀   
> - 条目3

#### 代码块放入列中
使用8个空格
输入：
```
- 条款1
- 条款2

        for i in range(10):
            print(i)
- 条款3
```

输出：
> - 条款1
> - 条款2
>
>        for i in range(10):
>           print(i)
> - 条款3
#### 图片进入列表

```
使用8个空格
- 条款1
- 条款2

![图片](test.bmp)
- 条款3

```

输出：
> 使用8个空格
> - 条款1
> - 条款2
>
> ![图片](test.bmp)
> - 条款3


# markdown扩展语法测试
## 表格
使用-和|的组合创建表格, 如下：
输入：
```
| 测试 | 内容 |
| --------- | -------- |
| a         | b |
```   

输出：
> | 测试 | 内容 |
> | --------- | -------- |
> | a         | b |

### 对齐
输入：
```
| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: |
| Header      | Title       | Here's this   |
| Paragraph   | Text        | And more      |
```

输出：
> | Syntax      | Description | Test Text     |
> | :---        |    :----:   |          ---: |
> | Header      | Title       | Here's this   |
> | Paragraph   | Text        | And more      |


### 表格内容格式化
对表格内容可以使用增加链接、代码和标记重点等语法，但是不能使用列表、标题、引用快
图片等语法

 
## 代码块
使用\~\~\~或者\`\`\`    
输入：     
\`\`\`

a= 1

\`\`\`

输入：
> ```
> 
> a = 1
>
> ```

### 语法高亮,
在\`后面添加指定的语言。  
输入：     
\`\`\`python    
a = 1  
\`\`\`

输出：
> ```python
> a = 1
> ```


## 附注(Footnotes)

输入：
```
Here's a simple footnote,[^1] and here's a longer one.[^bignote]

[^1]: This is the first footnote.

[^bignote]: Here's one with multiple paragraphs and code.

    Indent paragraphs to include them in the footnote.

    `{ my code }`

    Add as many paragraphs as you like.
```

> Here's a simple footnote,[^1] and here's a longer one.[^bignote]
>
> [^1]: This is the first footnote.
>
> [^bignote]: Here's one with multiple paragraphs and code.
>
>     Indent paragraphs to include them in the footnote.
> 
>     `{ my code }`
>
>     Add as many paragraphs as you like.

  
## 删除线
使用四个`符号包围的内容会增加删除线。     
输入：
```
~~Good~~ 
```  
输出:
> ~~Good~~
 
 
## 任务列表-复选框
使用-和[ ]的组合。
输入：
```
- [x] Contra
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media
```
输出：
> - [x] Contra
> - [x] Write the press release
> - [ ] Update the website
> - [ ] Contact the media
 

## 自动URL链接
一般编辑器开启自动url，例如输入http://192.168.0.1/

### 关闭自动url
一般编辑器开启自动url，例如输入`http://www.example.com`


## 锚点
待补充

## Definition Lists
待补充


