## html概述

### 1. html概述及html文档基本结构

#### 1.1 html概述

    HTML是 HyperText Mark-up Language 的首字母简写，意思是超文本标记语言，超文本指的是超链接，
    标记指的是标签，是一种用来制作网页的语言，这种语言由一个个的标签组成，用这种语言制作的文件
    保存的是一个文本文件，文件的扩展名为html或者htm。


#### 1.2 html文档基本结构

***一个html的基本结构如下：***

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8">
        <title>网页标题</title>
    </head>
    <body>
          网页显示内容
    </body>
</html>
```


    第一行是文档声明，第二行“<html>”标签和最后一行“</html>”定义html文档的整体，“<head>”标签
    和“<body>”标签是它的第一层子元素，“<head>”标签里面负责对网页进行一些设置以及定义标题，
    设置包括定义网页的编码格式，外链css样式文件和javascript文件等，设置的内容不会显示在网页
    上，标题的内容会显示在标题栏，“<body>”内编写网页上显示的内容。
    一个html文件就是一个网页，html文件用编辑器打开显示的是文本，可以用文本的方式编辑它，如
    果用浏览1器打开，浏览器会按照标签描述内容将文件渲染成网页。


#### 1.3 html文档快速创建

    
    新建一个html文档后，可以用快捷键的方式快速创建html文档。快捷键：!+tab键，或者 html:5+tab键。


### 2. html标签入门


    标签语法：学习html语言就是学习标签的用法，html常用的标签有20多个，学会这些标签的使用，就基
    本上学会了HTML的使用。


```html
<!-- 1、成对出现的标签：-->

<h1>h1标题</h1>
<div>这是一个div标签</div>
<p>这个一个段落标签</p>


<!-- 2、单个出现的标签： -->
<br>
<img src="images/pic.jpg" alt="图片">

<!-- 3、带属性的标签，如src、alt 和 href等都是属性 -->
<img src="images/pic.jpg" alt="图片">
<a href="http://www.baidu.com">百度网</a>

<!-- 4、标签的嵌套 -->
<div>
    <img src="images/pic.jpg" alt="图片">
    <a href="http://www.baidu.com">百度网</a>
</div>
```




