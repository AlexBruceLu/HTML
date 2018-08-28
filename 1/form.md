## html表单


    表单用于搜集不同类型的用户输入，表单由不同类型的标签组成，相关标签及属性用法如下：


### 1、<form>标签定义整体的表单区域


    action属性 定义表单数据提交地址
    method属性 定义表单提交的方式，一般有“get”方式和“post”方式

    
### 2、<label>标签为表单元素定义文字标注

### 3、<input>标签定义通用的表单元素


    type属性
    type="text" 定义单行文本输入框
    type="password" 定义密码输入框
    type="radio" 定义单选框
    type="checkbox" 定义复选框
    type="file" 定义上传文件
    type="submit" 定义提交按钮
    type="reset" 定义重置按钮
    type="button" 定义一个普通按钮
    value属性 定义表单元素的值
    name属性 定义表单元素的名称，此名称是提交数据时的键名


### 4、<textarea>标签定义多行文本输入框

### 5、<select>标签定义下拉表单元素

### 6、<option>标签与<select>标签配合，定义下拉表单元素中的选项


**最终实现结果如下：**


![image](https://raw.githubusercontent.com/wiki/AlexBruceLu/HTML/biao.png)


```html
<!DOCTYPE html>
<html lang="zh-CN">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>去年买的表</title>
    <link rel="Shortcut Icon" href="https://raw.githubusercontent.com/wiki/AlexBruceLu/HTML/favicon.ico">
    <style>
        .box {
            width: 458px;
            height: 344px;
            background-image: url(https://raw.githubusercontent.com/wiki/AlexBruceLu/HTML/1f.jpg);
            border: 1px solid rgb(255, 255, 255);
            margin: 40px auto;
            border-collapse:collapse;
        }

        .box th {
            border: 1px solid aliceblue;
            text-align: center;
        }

        .box td {
            border: 1px solid aliceblue;
            text-align: center;
            font-family: "	Microsoft YaHei"
        }
        .color1{
            color: #f8f8f0;
        }
        .color2{
            color: #a6e22e;
        }
        .color3{
            color: #f72671;
        }
        .color4{
            color: #65d7ed;
        }
        .color5{
            color: #ffe792;
        }
    </style>
</head>

<body>
    <table class="box">
        <tr>
            <th class="color2">编号</th>
            <th class="color4">姓名</th>
            <th class="color1">性别</th>
            <th class="color3">爱好</th>
            <th class="color5">住址</th>
        </tr>
        <tr class="color2">
            <td>1</td>
            <td>德玛</td>
            <td>男</td>
            <td>抽烟</td>
            <td>德玛西亚</td>
        </tr>
        <tr class="color1">
            <td>2</td>
            <td>寒冰</td>
            <td>女</td>
            <td>足疗</td>
            <td>艾欧尼亚</td>
        </tr>
        <tr class="color3">
            <td>3</td>
            <td>日女</td>
            <td>女</td>
            <td>SPA</td>
            <td>钢铁烈阳</td>
        </tr>
        <tr class="color4">
            <td>4</td>
            <td>二珂</td>
            <td>女</td>
            <td>SPA</td>
            <td>钢铁烈阳</td>
        </tr>
        <tr class="color5">
            <td>5</td>
            <td>陈粒</td>
            <td>女</td>
            <td>SPA</td>
            <td>钢铁烈阳</td>
        </tr>
    </table>
</body>

</html>
```
