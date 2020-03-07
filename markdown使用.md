# markdown使用

## markdown简介

![](https://www.runoob.com/wp-content/uploads/2019/03/iconfinder_markdown_298823.png)

* Markdown 是一种轻量级标记语言，它允许人们使用易读易写的纯文本格式编写文档。

* Markdown 语言在 2004 由约翰·格鲁伯（英语：John Gruber）创建。

* Markdown 编写的文档可以导出 HTML 、Word、图像、PDF、Epub 等多种格式的文档。

* Markdown 编写的文档后缀为 .md, .markdown。

### 编辑器

* Typeora支持导出HTML、PDF、Word、图片等多种类型文件。

* Typeota具有跨平台支持。

* Typeora官网：https://typora.io/

### 语言特点

+ "编程式"写文章，定位准确

+ 书写美观，方便使用

## Markdown标题

### 使用#表示

* 使用 # 号可表示 1-6 级标题，一级标题对应一个 # 号，二级标题对应两个 # 号，以此类推。

* 例：

  ```
  # 一级标题
  ## 二级标题
  ### 三级标题
  #### 四级标题
  ##### 五级标题
  ###### 六级标题
  ```

### 使用快捷键

* 可以使用ctrl+(1-6)表示1-6级标题

## Markdown段落格式

### 字体格式

* 例：

*斜体文本*
_斜体文本_
**粗体文本**
__粗体文本__
***粗斜体文本***
___粗斜体文本___

<u>下划线</u>

~~删除线~~

<!--注释-->

```
*斜体文本*
_斜体文本_
**粗体文本**
__粗体文本__
***粗斜体文本***
___粗斜体文本___
<u>下划线</u>
~~删除线~~
<!--注释-->
```

* 使用快捷键：

  *斜体文本*
  __粗体文本__

  <u>下划线</u>

  ~~删除线~~

  ````
  Ctrl+I
  Ctrl+B
  Ctrl+U
  Alt+Shift+5
  ````

### 段落格式

* 分隔线

  例：下面都可表示分隔线

  ````
  ***
  
  * * *
  
  *****
  
  - - -
  
  ----------
  ````

* 脚注

  例： 您好[^您好的解释]

  [^您好的解释]:您好是向您问好的意思

  ````
  [^要注明的文本]
  被标注的对象：  您好[^您好的解释]
  标注的内容：    [^您好的解释]:您好是向您问好的意思
  注意其中的标注的内容的引号为英文状态下的引号
  ````

## Markdown列表

* 两种列表类型：有序列表和无序列表。

### 无序列表

* 使用星号(*)、加号(+)或是减号(-)作为列表标记：

* 例：

  ```
  * 第一项
  * 第二项
  * 第三项
  
  + 第一项
  + 第二项
  + 第三项
  
  - 第一项
  - 第二项
  - 第三项
  ```

  ![](https://www.runoob.com/wp-content/uploads/2019/03/89446A8E-6D83-4666-AACC-980145D5F070.jpg)

### 有序列表

+ 有序列表使用数字并加上 . 号来表示

+ 例：

  ```
  1. 第一项
  2. 第二项
  3. 第三项
  ```

![](https://www.runoob.com/wp-content/uploads/2019/03/560384BB-2B00-41D5-ACF2-18972F7F2775.jpg)

### 列表嵌套

* 列表嵌套只需在子列表中的选项添加四个空格即可

* 例：

  ```
  1. 第一项：
      - 第一项嵌套的第一个元素
      - 第一项嵌套的第二个元素
  2. 第二项：
      - 第二项嵌套的第一个元素
      - 第二项嵌套的第二个元素
  ```

![](https://www.runoob.com/wp-content/uploads/2019/03/8ED795DA-F124-4E70-BA71-57CD9CF958A4.jpg)

## Markdown区块

* Markdown 区块引用是在段落开头使用 > 符号 ，然后后面紧跟一个**空格**符号

* 例：

  ```
  > 区块引用
  > 区块引用2
  > 区块引用3
  ```

> 区块引用
> 区块引用2
> 区块引用3

### 区块嵌套

* 另外区块是可以嵌套的，一个 > 符号是最外层，两个 > 符号是第一层嵌套，以此类推
* 例：

```
> 最外层
> > 第一层嵌套
> > > 第二层嵌套
```

![](https://www.runoob.com/wp-content/uploads/2019/03/AA0A4A6A-33A7-48C7-971F-73FFC8FE85B0.jpg)

### 区块中使用列表

* 区块可以与有序列表或者无序列表嵌套使用
* 例：

```
> 区块中使用列表
> 1. 第一项
> 2. 第二项
> + 第一项
> + 第二项
> + 第三项
```

> 区块中使用列表
> 1. 第一项
> 2. 第二项
> + 第一项
> + 第二项
> + 第三项

### 列表中使用区块

* 有序或者无序列表中可以嵌套区块使用
* 例：

```
* 第一项
    > 菜鸟教程
    > 学的不仅是技术更是梦想
* 第二项
```

* 第一项
    > 菜鸟教程
    > 学的不仅是技术更是梦想
    
* 第二项

## Markdown 代码

* 代码片段：如果是段落上的一个函数或片段的代码可以用反引号把它包起来（`）
* 例：

```
`printf()` 函数
```

`printf()` 函数

### 代码块

* 用\``` 包裹一段代码，并且可以指定语言(关键字会高亮显示)
* 例：

```
​```javascript
$(document).ready(function () {
    alert('RUNOOB');
});
​```
```

```javascript
$(document).ready(function () {
    alert('RUNOOB');
});
```

## Markdown链接

* 链接可以引用其他网址到文章
* 例：

```
[链接名称](链接地址)

或者

<链接地址>
```

[百度](https://www.baidu.com)           <https://www.baidu.com>

### 高级链接

* 链接可以用变量来代替，然后再在文末附带变量地址
* 例：

```
链接也可以用变量来代替，文档末尾附带变量地址：
这个链接用 1 作为网址变量 [Baidu][1]
然后在文档的结尾为变量赋值（网址,注意分号要用英文的状态）
  [1]:http://www.baidu.com/   
```

[Baidu][1]

[1]:http://www.baidu.com

## Markdown图片

* 插入图片

* 例：

  ```
  ![alt 属性文本](图片地址)
  ![alt 属性文本](图片地址 "可选标题")
  
   开头一个感叹号 !
   接着一个方括号，里面放上图片的替代文字
   接着一个普通括号，里面放上图片的网址，最后还可以用引号包住并加上选择性的 'title' 属性的文字。
   
   alt标签:用来描述图片关键词，可以不写。最初的本意是当图片因为某种原因不能被显示时而出现的替代文字，后来又被用于SEO，可以方便搜索引擎根据alt里面的关键字搜索到图片
   图片地址:可以是本地文件的链接，也可以是远端的图片地址，还可以是Base64编码后的文件，但是Base64编码的图片本身最好比较小最好。
  
  ```

![百度图标](https://dss0.bdstatic.com/5aV1bjqh_Q23odCf/static/superman/img/logo_top-e3b63a0b1b.png)

![百度图标](https://dss0.bdstatic.com/5aV1bjqh_Q23odCf/static/superman/img/logo_top-e3b63a0b1b.png"百度图标")

![](data:image/jpg;base64,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)

#### Base64转换图片(python)

![](https://bbs-img.huaweicloud.com/blogs/img/1524448316938093.png)

![](https://bbs-img.huaweicloud.com/blogs/img/1524448354913927.png)

### 高级图片插入

* 类似插入高级链接一样
* 例：

```
这个链接用 1 作为网址变量 [baidu][1].
然后在文档的结尾为变量赋值（网址）

[1]: https://dss0.bdstatic.com/5aV1bjqh_Q23odCf/static/superman/img/logo_top-e3b63a0b1b.png
```

[baidu][1]

[1]: https://dss0.bdstatic.com/5aV1bjqh_Q23odCf/static/superman/img/logo_top-e3b63a0b1b.png

## Markdown表格

* Markdown 制作表格使用 `|` 来分隔不同的单元格，使用 `-` 来分隔表头和其他行

* 例：

  ```
  |  表头   | 表头  |
  |  ----  | ----  |
  | 单元格  | 单元格 |
  | 单元格  | 单元格 |
  ```

| 表头   | 表头   |
| ------ | ------ |
| 单元格 | 单元格 |
| 单元格 | 单元格 |

### 对其方式

- -: 设置内容和标题栏居右对齐。
- :- 设置内容和标题栏居左对齐。
- :-: 设置内容和标题栏居中对齐。
- 例：

```
| 左对齐 | 右对齐 | 居中对齐 |
| :-----| ----: | :----: |
| 单元格 | 单元格 | 单元格 |
| 单元格 | 单元格 | 单元格 |
```

| 左对齐 | 右对齐 | 居中对齐 |
| :----- | -----: | :------: |
| 单元格 | 单元格 |  单元格  |
| 单元格 | 单元格 |  单元格  |

## 其他技巧

### 支持的 HTML 元素

* 不在 Markdown 涵盖范围之内的标签，都可以直接在文档里面用 HTML 撰写。

  目前支持的 HTML 元素有：`<kbd> <b> <i> <em> <sup> <sub> <br>`等 

* 例：

  ````
  使用 <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> 重启电脑
  ````

  使用 <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> 重启电脑

### 转义

* Markdown 使用了很多特殊符号来表示特定的意义，如果需要显示特定的符号则需要使用转义字符，Markdown 使用反斜杠转义特殊字符
* 例：

```
**文本加粗** 
\*\* 正常显示星号 \*\*
```

### **文本加粗** 

\*\* 正常显示星号 \*\*

* Markdown 支持以下这些符号前面加上反斜杠来帮助插入普通的符号：

```
\   反斜线
`   反引号
*   星号
_   下划线
{}  花括号
[]  方括号
()  小括号
#   井字号
+   加号
-   减号
.   英文句点
!   感叹号
```

### 公式

* 当你需要在编辑器中插入数学公式时，可以使用两个美元符 $$ 包裹 TeX 或 LaTeX 格式的数学公式来实现。提交后，问答和文章页会根据需要加载 Mathjax 对数学公式进行渲染。
* 例：

```
$$
\mathbf{V}_1 \times \mathbf{V}_2 =  \begin{vmatrix} 
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
\frac{\partial X}{\partial u} &  \frac{\partial Y}{\partial u} & 0 \\
\frac{\partial X}{\partial v} &  \frac{\partial Y}{\partial v} & 0 \\
\end{vmatrix}
${$tep1}{\style{visibility:hidden}{(x+1)(x+1)}}
$$
```


$$
\mathbf{V}_1 \times \mathbf{V}_2 =  \begin{vmatrix} 
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
\frac{\partial X}{\partial u} &  \frac{\partial Y}{\partial u} & 0 \\
\frac{\partial X}{\partial v} &  \frac{\partial Y}{\partial v} & 0 \\
\end{vmatrix}
${$tep1}{\style{visibility:hidden}{(x+1)(x+1)}}
$$

### typora 画流程图、时序图(顺序图)、甘特图



```mermaid
%% 语法示例
        gantt
        dateFormat  YYYY-MM-DD
        title 软件开发甘特图
        section 设计
        需求                      :done,    des1, 2014-01-06,2014-01-08
        原型                      :active,  des2, 2014-01-09, 3d
        UI设计                     :         des3, after des2, 5d
    未来任务                     :         des4, after des3, 5d
        section 开发
        学习准备理解需求                      :crit, done, 2014-01-06,24h
        设计框架                             :crit, done, after des2, 2d
        开发                                 :crit, active, 3d
        未来任务                              :crit, 5d
        耍                                   :2d
        section 测试
        功能测试                              :active, a1, after des3, 3d
        压力测试                               :after a1  , 20h
        测试报告                               : 48h
```