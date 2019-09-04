# H5程序设计基础

- HTML（超文本标记语言）

- CSS

- JavaScript

- **HTML5**

- **CSS3**

  ## 文档基本结构

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```

## 常用标签

```html
根据效果或者功能，选择合适的标签
<!-- 标题 -->
    <h1></h1>
    <!-- 段落 -->
    <p></p>
    <!-- 图片 -->
    <img src="imgs/news.jpg"/>
    <!-- 超链接 anchor-->
    <a target="_blank" href="http://www.baidu.com">百度一下，你就知道</a>
    <!-- 列表 -->
    <!-- unordered list -->
    <ul>
        <!-- list item -->
        <li></li>
    </ul>
    <!-- ordered list-->
    <ol>
        <li></li>
    </ol>
    <!-- 布局 division-->
    <div></div>
    <!-- 表单 -->
    <form action="" method="get">
        <!-- 表单元素 -->
        <p>
            用户名：<input type="text">
        </p>
        <p>
            <input type="text" name="user" placeholder="用户名">
        </p>
        <input type="password" name="pwd">
        <input type="radio" name="sex" value="man">男
        <input type="radio" name="sex" value="women">女
        <input type="checkbox" name="course" value="">  
        <input type="checkbox" name="course" value="">
        <input type="checkbox" name="course" value="">
        <input type="checkbox" name="course" value="">
        <input type="submit" value="登录">
        <input type="button" value="按钮">
    </form>
```



```html
表格
<!-- border:设置表格的边框 -->
    <!-- bordercolor:设置表格边框颜色 -->
    <!-- cellspacing:设置单元格和单元格之间的距离 -->
    <!-- cellpadding:设置单元格和内容之间的距离 -->
    <!-- width/height:设置表格的宽度/高度 -->
    <!-- align:设置表格对齐方式 -->
    <!-- bgcolor:设置表格背景色 -->
    <table bgcolor="" align="center" bordercolor="red" width="800" border="5" cellspacing="0" cellpadding="10">
        <!-- align：写在tr或td上是设置文字对齐方式 -->
        
        <!-- 列合并（写在td或th上）：colspan -->
        <!-- 行合并（写在td或th上）：rowspan -->
        <tr>
            <th colspan="4">商品类目</th>
        </tr>
        <tr align="center">
            <td rowspan="3">移动</td>
            <td>移动</td>
            <td>移动</td>
            <td>移动</td>
        </tr>
        <tr>
            <td>移动</td>
            <td>移动</td>
            <td>移动</td>
        </tr>
        <tr>
            <td>移动</td>
            <td>移动</td>
            <td>移动</td>
        </tr>
        <tr>
            <td rowspan="3">移动</td>
            <td>移动</td>
            <td>移动</td>
            <td>移动</td>
        </tr>
        <tr>
            <td>移动</td>
            <td>移动</td>
            <td>移动</td>
        </tr>
        <tr>
            <td>移动</td>
            <td>移动</td>
            <td>移动</td>
        </tr>
    </table>
```



## CSS(层叠样式表)

### 使用方法

- 行内样式（1000）
- 外联样式
- 内部样式

### 基本选择器

- 标签选择器（1）
- 类选择器（class）（10）
- id选择器（100）

## 选择器优先级

> id > 类选择器 > 标签选择器

## 派生选择器

- 包含选择器（后代选择器）
- 子选择器
- 通配符选择器

## 字体样式

- font-size
- font-style : italic/oblique;
- font-weight : bold/bolder;
- font-family : "宋体"

## 文本样式

- （水平对齐方式）text-align : center / left / right;
- （设置字体颜色）color : red;
- （设置首行缩进）text-indent : 2em;
- （行高/设置文字垂直对齐方式）line-height : 30px;
- （文本修饰）text-decoration : none/underline/overline/line-through;

## 背景样式

- background-color : #ccc;
- background-image : url( );
- background-repeat : no-repeat;
- background-position : 
- background : red url() no-repeat 100px center;

## 列表样式

- list-style : none;

## 超链接样式（伪类选择器）

- :link 只有超链接可以用（未被访问之前）
- :visited 只有超链接可以用（访问过后）
- :hover 可用于任意标签（鼠标经过时）
- :active（鼠标点击时）



















