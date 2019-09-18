# H5程序设计基础

**qq : 1127570788**

**tel : 18633900994**

**name : 刘冠军**

- HTML（超文本标记语言）

- CSS

- JavaScript

- **HTML5**

- **CSS3**

  ## 文档基本结构

```html
<!DOCTYPE html>
<html>
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
    <div></div><!--块级元素-->
	<span></span><!--行内元素-->
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
        <select name="sel">
            <option value="beijing">北京</option>
        </select>
        <textarea></textarea>
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
- 群组选择器
- 属性选择器
- 相邻兄弟选择器
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

## 盒模型

- width
- height
- border : 1px solid red;
  - border-top
  - border-right
  - border-bottom
  - border-left
- margin(外边距：盒子之间的距离)
  - margin-top
  - margin-right
  - margin-bottom
  - margin-left
- padding(内边距：盒子边缘与内容之间的距离)
  - padding:10px；四个方向一样
  - padding:20px 10px；上下 /  左右
  - padding: 10px 20px 30px;上 / 左右 / 下
  - padding: 10px 20px 30px 40px;上右下左

## display:block/inline/inline-block/none;

- block : 将元素转换成块级元素
- inline : 将元素转换成行内元素
- inline-block : 将元素转换成行内块元素
- none : 元素不显示

## 浮动(float)

- 包裹性
- 向上性
- 不重叠

## 定位（position）

- position : fixed;(固定定位：相对于浏览器定位)
- position : relative;(相对定位：相对于该元素自身所在的位置定位)
- position : absolute;(绝对定位：相对于该元素有定位属性的父元素去定位，如果父元素都没定位属性，相对于body定位)
- position : static;(不定位)

## 层叠上下文

- z-index : 999;

## overflow(溢出处理)

- hidden（溢出隐藏）
- scroll（出现滚动条）
- auto（自动）



# JavaScript

## 简介

> 基于对象和事件驱动的脚本语言
>
> 特点：动态（声明时无需指定变量类型）、
>
> ​            弱类型（可以给变量赋值成任意类型）
>
> javascript包括：
>
> ​	ECMAscript(基本语法)
>
> ​	DOM（文档对象模型）
>
> ​	BOM（浏览器对象模型）

## 基础语法

```javascript
//声明变量
var num = 10;
//全局变量（声明在所有函数之外的变量）
//局部变量（函数内部，通过var声明的变量）
//在函数外部不能访问函数内的局部变量
//函数内可以访问全局变量
		var num = 199;
        function a(){
            num = num + 100;
            var sum = 100;
            console.log(sum);//100
        }
        a();
        console.log(num);//299
        console.log(sum);//报错
//基本数据类型
//Number、String、Boolean、Undefined、Null
var flag = true;
var str = 'abcd';
var num = 100;
console.log(typeof flag);//boolean
console.log(typeof str);//string
console.log(typeof num);//number
var u;
console.log(typeof u);//undefined
//运算符
+=   %=    ?:  && || !
//流程控制语句
//顺序结构   分支结构  循环结构
if(10>2){
   console.log(true);
}else{
    
}
switch(){
       case :
          break;
}
//循环结构
for(){
}
```

## 函数

```javascript
// 函数声明
        // 函数名以英文字母或$开头，不能是关键字
        // function fn(){
        //     console.log(100);
        // }
        // var f = function(){
        //     console.log('这是f函数');
        // }
// 函数的调用（函数+小括号调用）
        // fn();
// 函数的参数(函数声明时是形参，调用时是实参)
// 函数的返回值(返回一个值，或直接跳出整个函数)
        // 函数return后没有值，函数也有返回值，是undefined
        // 函数如果没有return语句，也有返回值，是undefined
        // function sum(a,b){
        //     return a+b;
        // }
        // console.log( sum(1,5) );
```

## 对象

```javascript

        // 对象的声明(一系列属性和方法的集合)
        // this是调用当前方法的对象
        var obj = {
            name:'潘',
            age:18,
            height:180,
            say:function(){
                console.log(this.name)
            }
        };
        // 对象的访问
        console.log(obj.name);
        console.log(obj['name']);
        obj.say();
        // 添加属性或方法
        obj.weight = 80;
        // 修改
        obj.name = '潘帅帅';
        console.log(obj);
        // 删除属性
        delete obj.name;
        // 遍历(for in 循环)
        for(var item in obj){
            if(typeof obj[item] !== "function"){
                document.write(obj[item]+'<br>');
            }
        }
```

## 数组和字符串

```javascript
// 数组的声明
        var arr = [1,2,3,4,5];
        // 数组的访问
        // console.log(arr[0]);
        // 数组的方法
        // push:在数组末尾添加元素，并返回数组的长度；
        // var newArr = arr.push(3,4,5);
        // console.log(newArr);
        // console.log(arr);
        // pop:删除数组末尾的元素，并返回删除的元素
        // var ele = arr.pop();
        // console.log(ele,arr);
        // arr.shift   arr.unshift
        // splice：从某一位开始删，删除几个，在该位添加
        // var ele = arr.splice(1,0,100,90);
        // console.log(arr,ele);
        // arr.indexOf()：返回该元素的下标索引，如果不存在返回-1。
        // 数组的去重
        // var arr = [1,2,3,2,4,3,3,2,5,6,2];
        // var newArr = [];
        // for(var i=0;i<arr.length;i++){
        //     if(newArr.indexOf(arr[i])==-1){
        //         newArr.push(arr[i]);
        //     }
        // }
        // console.log(newArr);

        // for(var i=0;i<arr.length-1;i++){
        //     for(var j=i+1;j<arr.length;j++){
        //         if(arr[i]===arr[j]){
        //             arr.splice(j,1);
        //             j--;
        //         }
        //     }
        // }
        // console.log(arr);
        // 数组的排序
        // 冒泡排序
        // console.time('a')
        // var arr = [1,2,3,2,9,4,6,3,90,67,5];
        // for(var i=0;i<arr.length-1;i++){
        //     for(var j=0;j<arr.length-i-1;j++){
        //         if(arr[j]>arr[j+1]){
        //             var temp = arr[j];
        //             arr[j] = arr[j+1];
        //             arr[j+1] = temp;
        //         }
        //     }
        // }
        // console.log(arr);
        // console.timeEnd('a');
        // 选择排序
        // var arr = [1,2,3,2,9,4,6,3,90,67,5];
        // for(var i=0;i<arr.length-1;i++){
        //     for(var j=i+1;j<arr.length;j++){
        //         if(arr[i]>arr[j]){
        //             var temp = arr[i];
        //             arr[i] = arr[j];
        //             arr[j] = temp;
        //         }
        //     }
        // }
        // console.log(arr);
```

## DOM（文档对象模型）

```javascript
// DOM(document object model：文档对象模型)
        // DOM 树
        // 节点类型：文本节点  元素节点  属性节点

        // 获取元素
        // document.getElementById();
        // document.getElementsByClassName();
        // document.getElementsByTagName();
        // var nav = document.getElementById('nav');
        // console.log(nav);
        // var lis = document.getElementsByTagName('li');
        // console.log(lis[0]);
        // 通过节点关系获取

        // console.log(nav.childNodes);
        // console.log(nav.children);
        // console.log(nav.parentNode);
        // 			  console.log(nav.firstElementChild.nextElementSibling);
// 事件类型：onclick  onmouseover onmouseout
        // onmousemove onmouseup onmousedown
        // 绑定事件
        // 三要素：绑定的元素、事件类型、事件处理函数

//节点的创建和删除
       // 1、先获取要操作的标签
        var inp = document.getElementById('msg');
        var list = document.getElementById('list');
        // 2、给input绑定键盘事件
        // 键盘事件：onkeydown   onkeyup
        inp.onkeydown = function(e){
            // 判断是否是回车键
            if(e.keyCode===13){
                // 创建一个li标签
                var li = document.createElement('li');
                // 给li里赋值成input框输入的内容
                li.innerHTML = inp.value;
                // 添加到指定的元素里
                list.appendChild(li);
                li.onclick = function(){
                    list.removeChild(this);
                }
                inp.value = '';
                // ul中添加一个li标签
                // list.innerHTML += '<li>'+inp.value+'</li>';
            }
        }
        // 先获取li
        var lis = list.children;
        // 给li绑定点击事件
        for(var i=0;i<lis.length;i++){
            lis[i].onclick = function(){
                list.removeChild(this);
            }
        }
//事件流：事件冒泡、事件捕获
//利用事件冒泡的特性，可以实现事件委托（即当需要给子元素绑定事件的时候，给父元素绑）
//阻止事件冒泡：e.stopPropagation();
```

## BOM(浏览器对象模型)

#### window对象下的方法

- alert()
- confirm()
- close()
- open()
- setInterval()
- setTimeout()
- clearInterval()
- clearTimeout()
- onload

#### window下的对象

- history
  - back()
  - forward()
  - go()
- location
  - hash
  - search
  - port
  - host
  - href
- screen
  - width
  - height
  - availHeight
  - availWidth
- navigator
  - userAgent
  - appVersion
- document



















