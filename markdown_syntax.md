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
~~~
**Good**
~~~
输出：
> **Good**


### 斜体字
使用两个星号将需要进行斜体的内容括起来。
输入：
~~~
*Good*
~~~  
输出:     

*Good*


### 加粗并倾斜
使用6个星号将需要加粗和倾斜的内容括起来。
输入：
~~~
***Good***
~~~
输出：     
***Good***



## 块级引用
使用'>'进行块引用。     
输入：
~~~
> sdfsadlsdfasdfsafasadfasdfasdfssdfasfasdfasdfasdfasd
> 
> asdfasdfasdf asdfasdfasdfasdf
~~~ 
输出：     
> sdfsadlsdfasdfsafasadfasdfasdfssdfasfasdfasdfasdfasd
> 
> asdfasdfasdf asdfasdfasdfasdf


### 镶嵌的块引用
块引用可以包含其他块引用，例如：
>sdfasdfasldfasls
>
>>asfasdfasdfasdsdflsdfsf
### 块应用可以包含其他的元素
> #### 标题-块引用
>
> - 项目1
> - 项目2
>
> *项目总结*


## 代码
使用``插入代码，例如：
`name = 1`
### 转义
主要用于代码中显示\`符号，例如：

``Use \`code\` in your Markdown file.``

### 代码块
每行使用至少4个空格缩进或者一个Tab键缩进：
 
    a = 1
    b = 2
    c = 2
    for i in range(2):
        print(i)

扩展语法，例如：

```
a = 1
b = 2
c = 2
for i in range(2):
    print(i)

```

## 水平线规则
使用三个或三个以上的星号或下划线，例如：

***

___

## 添加链接
如给“百度”这两个字添加链接，例如：  
网址链接：[百度](https://www.baidu.com)

### 给链接添加标题
网址链接是：[百度](https://www.baidu.com "太菜")

### URL和电子邮件地址
使用<>，例如：    
<http://www.baidu.com>  
<fake@example.com>

### 格式化链接
可以使用标记重点的方式格式化链接.例如：    
This is the **[Markdown Guide](https://www.markdownguide.org)**.    
This is the *[Markdown Guide](https://www.markdownguide.org)*.  
This is the ***[Markdown Guide](https://www.markdownguide.org)***.

### 参考风格的链接
这种类型的链接包含两个部分，一个是文本，一个是存放的位置
#### 格式化第一个部分-文本内容
In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends
of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to
eat: it was a [hobbit-hole][1], and that means comfort.

[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"

使用带标题的链接同样可以实现以上效果：     
In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends
of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to
eat: it was a [hobbit-hole](https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"), and that means comfort.

## 图片
使用![]来引用图片, 例如:     
![This place was so cool!](test.bmp "Cool")

### 为图片添加链接
在图片的引用放入链接的[]中即可，例如:    
[![An old rock in the desert](test.bmp "百度图片")](https://www.baidu.com)
### 


##转义符号“\”
用来标记，例如：    
* sfasd  

\* sfasd  


## 列表
###有序列表
1. 条目1
1. 条目2
1. 条目3
    1. 二级条目1
    2. 二级条目2
1. 条目4
5. 条目5
7. 条目6

### 无序列表
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
  
### 添加其他元素进入列表
#### 段落进入列表
 在一个条目后回车空白行后增加4个空格或者一个Tab键回车后输入段落内容
- 条目1
- 条目2

    段落手动阀手动阀
    
- 条目3

#### 块引用进入条目列表
- 条目1
- 条目2
>段落手动阀手动阀   
- 条目3

#### 代码块列表
使用8个空格
- 条款1
- 条款2

        for i in range(10):
            print(i)
- 条款3
#### 图片进入列表
使用8个空格
- 条款1
- 条款2

![图片](test.bmp)
- 条款3


# markdown扩展语法测试
## 表格
使用-和|的组合创建表格, 如下：   

| 测试 | 内容 |
| --------- | -------- |
| a         | b |

### 对齐
| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: |
| Header      | Title       | Here's this   |
| Paragraph   | Text        | And more      |

### 表格内容格式化
| Syntax      | Description | Test Text     |
| :--       |    :----:   |          ---: |
| Header      | Title       | Here's this   |
| Paragraph   | Text        | And more      |

 
##代码块
~~~
for i in range(1):
    print(i)
~~~
### 语法高亮
在```后面添加指定的语言，例如：   
~~~json
{
  "a": 1,
  "b": 2
}
~~~

在如python:   
~~~python
for i in range(10):
    print(i)
~~~

## 附注(Footnotes)
Here's a simple footnote,[^1] and here's a longer one.[^bignote]

[^1]: This is the first footnote.

[^bignote]: Here's one with multiple paragraphs and code.

    Indent paragraphs to include them in the footnote.

    `{ my code }`

    Add as many paragraphs as you like.
  
  
## 删除线
使用四个~符号包围的内容会增加删除线，例如：     
~~Good~~ 
 
 
## 任务列表-复选框
使用-和[ ]的组合，例如：  

- [x] Contra
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media
 

## 自动URL链接
一般编辑器开启自动url，例如输入http://192.168.0.1/

### 关闭自动url
一般编辑器开启自动url，例如输入`http://www.example.com`


## 锚点
待补充

## Definition Lists
待补充


