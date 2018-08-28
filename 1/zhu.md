### 实现如下结果


![image](https://raw.githubusercontent.com/wiki/AlexBruceLu/HTML/zhu.png)



***代码实现如下***


```html
<!DOCTYPE html>
<html lang="zh-CN">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>注册表</title>
    <link rel="Shortcut Icon" href="https://raw.githubusercontent.com/wiki/AlexBruceLu/HTML/favicon.ico">
    <style>
        .total {
            width: 1920px;
            height: 1080px;
            background-image: url(https://raw.githubusercontent.com/wiki/AlexBruceLu/HTML/7.jpg);
            background-repeat: no-repeat;
            margin: 0px;
            /* background-attachment:fixed; */
        }

        .total form {
            width: 400px;
            height: 450px;
            border: 3px solid rgb(143, 136, 136);
            margin: 200px 200px;
            padding: 0px 20px;
        }

        .total h3 {
            width: 400px;
            height: 40px;
            margin: 0px auto;
            text-align: center;
            border-bottom: 1px solid rgb(143, 136, 136);
            line-height: 40px;
        }
        .total .r{
            margin-left: 100px;

        }
    </style>
</head>

<body class="total">
    <form>
        <h3>
            用户注册表
        </h3>
        <p>
            <label>用户名：</label>
            <input type="text" />
        </p>
        <p>
            <label>密&nbsp;&nbsp;&nbsp;码：</label>
            <input type="password">
        </p>
        <p>
            <label>性&nbsp;&nbsp;&nbsp;别：</label>
            <input type="radio" name="gender" /> male
            <input type="radio" name="gender" /> female
            <input type="radio" name="gender" /> others
        </p>
        <p>
            <label>爱&nbsp;&nbsp;&nbsp;好：</label>
            <input type="checkbox" /> 抽烟
            <input type="checkbox" /> 喝酒
            <input type="checkbox" /> 烫头
            <input type="checkbox" /> 足疗
        </p>
        <p>
            <label>籍&nbsp;&nbsp;&nbsp;贯：</label>
            <select name="site">
                <option value="0">北京</option>
                <option value="1">上海</option>
                <option value="2">广州</option>
                <option value="3">深圳</option>
            </select>
        </p>
        <p>
            <label>照&nbsp;&nbsp;&nbsp;片：</label>
            <input type="file" name="照片" />
        </p>
        <p>
            <label>简&nbsp;&nbsp;&nbsp;介：</label>
            <textarea name="about"></textarea>
        </p>
        <p>
            <input class="r" type="submit" name="确定" value="提交" />
            <input class="r" type="reset" name="取消" value="取消" />
        </p>
    </form>
</body>

</html>
```
