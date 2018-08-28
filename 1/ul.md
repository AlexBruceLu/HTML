# 标签列表

列表一般应用在布局中的新闻标题列表和文章标题列表以及菜单，它是含有语义的，标签结构如下：


```html
<ul>
    <li>列表标题一</li>
    <li>列表标题二</li>
    <li>列表标题三</li>
</ul>
```


列表的内容一般是可以链接的，点击链接到新闻或者文章的具体内容，所以具体结构一般是这样的：


```html
<ul>
    <li><a href="#">列表标题一</a></li>
    <li><a href="#">列表标题二</a></li>
    <li><a href="#">列表标题三</a></li>
</ul>
```


**附：**

    
    list-style 去掉列表项的小圆点，比如：list-style:none
    body标签本来默认margin是8px；设置body的margin为0px，可以内容置顶不留空隙。
    多级标且重复出现可简写，如下：


```html
<ul>
    <li><a href="#">列表文字</a></li>
    <li><a href="#">列表文字</a></li>
    <li><a href="#">列表文字</a></li>
    <li><a href="#">列表文字</a></li>
    <li><a href="#">列表文字</a></li>
    <li><a href="#">列表文字</a></li>
</ul>
/* 简写为：ul>(li>a{列表文字})*6*/
```


```html
/*清除掉列表标签的默认样式*/
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Link</title>
    <style>
    .link{
        /* 去掉小圆点 */
        list-style: none;
        /* 清除外边距 */
        margin: 0px;
        /* 清除内边距 */
        padding: 0px;
    }
    .link a{
        /* 去掉下划线 */
        text-decoration: none;
    }
    </style>
</head>
<body>
    <ul class="link">
        <li><a href="#">列表更改后文字</a></li>
        <li><a href="#">列表更改后文字</a></li>
        <li><a href="#">列表更改后文字</a></li>
        <li><a href="#">列表更改后文字</a></li>
        <li><a href="#">列表更改后文字</a></li>
        <li><a href="#">列表更改后文字</a></li>
    </ul>
</body>
</html>
```

**对比效果图**

![image](https://raw.githubusercontent.com/wiki/AlexBruceLu/HTML/link.png)


