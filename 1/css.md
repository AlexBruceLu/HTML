# css介绍
## css概述


    为了让网页元素的样式更加丰富，也为了让网页的内容和样式能拆分开，CSS由此思想而诞生，CSS是 Cascading 
    Style Sheets 的首字母缩写，意思是层叠样式表。有了CSS，html中大部分表现样式的标签就废弃不用了，html
    只负责文档的结构和内容，表现形式完全交给CSS，html文档变得更加简洁。

## css基本语法

**css的定义方法是：**

**选择器 { 属性：值； 属性：值； 属性：值；}**

    选择器是将样式和页面元素关联起来的名称，属性是希望设置的样式属性，每个属性有一个或多个值。属性和值
    之间用冒号，一个属性和值与下一个属性和值之间用分号，最后一个分号可以省略，代码示例：


```html
/* 样式中注释的写法，单行或者多行注释 */
div{
    width:100px;
    height:100px;
    background:gold;
}
```


## css引入方式

**css引入页面的方式有三种：**

### 1、内联式：通过标签的style属性，在标签上直接写样式。

```html
<div style="width:100px; height:100px; background:red ">......</div>
```

### 2、嵌入式：通过style标签，在网页上创建嵌入的样式表。

```html
<style type="text/css">
    div{ width:100px; height:100px; background:red }
    ......
</style>
```

### 3、外链式：通过link标签，链接外部样式文件到页面中。

```html
<link rel="stylesheet" type="text/css" href="css/main.css">
```

## css选择器

### 1、标签选择器


    标签选择器，此种选择器影响范围大，一般用来做一些通用设置，或用在层级选择器中。举例：


```html
div{color:red}
......
<div>这是第一个div</div>   <!-- 对应以上样式 -->
<div>这是第二个div</div>   <!-- 对应以上样式 -->
```


### 2、类选择器


    通过类名来选择元素，一个类可应用于多个元素，一个元素上也可以使用多个类，应用灵活，可复用，是css中应用最多的一种选择器。举例：


```html
.blue{color:blue}
.big{font-size:20px}
.box{width:100px;height:100px;background:gold}
......
<div class="blue">....</div>
<h3 class="blue big box">....</h3>
<p class="blue box">....</p>
```

### 3、层级选择器


    主要应用在标签嵌套的结构中，层级选择器，是结合上面的两种选择器来写的选择器,它可与标签选择器结合使用，减少命名，同时也可以通过层
    级，限制样式的作用范围。举例：


```html
.con{width:300px;height:80px;background:green}
.con span{color:red}
.con .pink{color:pink}
.con .gold{color:gold}
......
<div class="con">
    <span>....</span>
    <a href="#" class="pink">....</a>
    <a href="#" class="gold">...</a>
</div>
<span>....</span>
<a href="#" class="pink">....</a>
```


## CSS元素属性及盒子模型

    盒子模型
    元素在页面中显示成一个方块，类似一个盒子，CSS盒子模型就是使用现实中盒子来做比喻，帮助我们设置元素对应的样式。盒子模型示意图如下：


![image](https://raw.githubusercontent.com/wiki/AlexBruceLu/HTML/view01.jpg)


    把元素叫做盒子，设置对应的样式分别为：盒子的宽度(width)、盒子的高度(height)、盒子的边框(border)、盒子内的内容和边框之间的间
    距(padding)、盒子与盒子之间的间距(margin)。


    设置宽高


```html
width:200px;  /* 设置盒子的宽度，此宽度是指盒子内容的宽度，不是盒子整体宽度(难点) */
height:200px; /* 设置盒子的高度，此高度是指盒子内容的高度，不是盒子整体高度(难点) */
```


    设置边框,设置一边的边框，比如顶部边框，可以按如下设置：


```html
border-top:10px solid red;
其中10px表示线框的粗细；solid表示线性。
```


    设置其它三个边的方法和上面一样，把上面的'top'换成'left'就是设置左边，换成'right'就是设置右边，换成'bottom'就是设置底边。
    四个边如果设置一样，可以将四个边的设置合并成一句：


```html
border:10px solid red;
设置内间距padding
```


    设置盒子四边的内间距，可设置如下：


```html
padding-top：20px;     /* 设置顶部内间距20px */
padding-left:30px;     /* 设置左边内间距30px */
padding-right:40px;    /* 设置右边内间距40px */
padding-bottom:50px;   /* 设置底部内间距50px */
```


    上面的设置可以简写如下：


```html
padding：20px 40px 50px 30px; /* 四个值按照顺时针方向，分别设置的是 上 右 下 左四个方向的内边距值。 */
```


    padding后面还可以跟3个值，2个值和1个值，它们分别设置的项目如下：


```html
padding：20px 40px 50px; /* 设置顶部内边距为20px，左右内边距为40px，底部内边距为50px */
padding：20px 40px; /* 设置上下内边距为20px，左右内边距为40px*/
padding：20px; /* 设置四边内边距为20px */
```


    设置外间距margin
    外边距的设置方法和padding的设置方法相同，将上面设置项中的'padding'换成'margin'就是外边距设置方法。


    盒子的真实尺寸
    盒子的width和height值固定时，如果盒子增加border和padding，盒子整体的尺寸会变大，所以盒子的真实尺寸为：
    盒子宽度 = width + padding左右 + border左右
    盒子高度 = height + padding上下 + border上下

    
    块元素居中技巧
    块元素如果想设置相对页面水平居中，可以使用margin值中的auto关键字，“auto”只能用于左右的margin设置，不能用于上下的：


```html
.box{
      width:300px;
      height:300px;
      background:gold;
      margin-left:0px;
      margin-top:0px;
      margin-left:auto;
      margin-right:auto;
}
```


    简写如下：


```html
.box{
     width:300px;
     height:300px;
     background:gold;
     margin:0px auto;
 }
 ```


    设置元素浮动属性float
    浮动可以让块元素排列在一行，浮动分为左浮动：float:left; 右浮动：float:right;

    设置元素背景属性background
    设置元素背景色或者背景图片，如：background:gold; 设置元素背景色为金色



## css文本属性


    color 设置文字的颜色，如： color:red;

    font-size 设置文字的大小，如：font-size:12px;

    font-family 设置文字的字体，如：font-family:'微软雅黑';为了避免中文字不兼容，一般写成：font-family:'Microsoft Yahei';

    font-weight 设置文字是否加粗，如：font-weight:bold; 设置加粗 font-weight:normal 设置不加粗

    line-height 设置文字的行高，如：line-height:24px; 表示文字高度加上文字上下的间距是24px，也就是每一行占有的高度是24px

    text-decoration 设置文字的下划线，如：text-decoration:none; 将文字下划线去掉

    text-align 设置文字水平对齐方式，如text-align:center 设置文字水平居中

    text-indent 设置文字首行缩进，如：text-indent:24px; 设置文字首行缩进24px















