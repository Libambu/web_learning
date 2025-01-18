# HTML 学习

## 标题

```html
<h1>一级标题</h1>
<h2>二级标题</h2>
<h3>三级标题</h3>
<h4>四级标题</h4>
<h5>五级标题</h5>
<h6>六级标题</h6>
```

在标签中添加属性，可设置位置

```html
align="left|center|right"
```

## 段落，换行，水平线

```html
<p>段落<br>换行</p>
水平线
<hr color=""width="px" size="px" align="center">
```

## 图片

```html
<img src="" alt="" title="" width="" height="">
src 图片的路径或名字
alt 规定图片的代替文本
width 规定图片的宽度
height 规定图片的高度
title 图片提示
```

## 超文本链接

```html
<a href="我的链接">
	<img src="">
</a>
```

一个未访问过的链接会显示为蓝色字体并附带下划线

访问过的链接会变成紫色

点击连接时，链接会显示为红色并带有下划线

## 文本标签

常见的文本标签

```html
<em></em>   定义着重文字
<b></b>	   定义粗体文字	
<i></i>	   定义斜体文字
<strong></strong>定义加重语气
<del></del>  定义删除字
<span></span> 元素没有特定含义   
可以嵌套在p标签中 <p>段落<em>嵌套文本</em>段落</p>
```

## 列表标签之有序列表

有序列表是一列项目，列表项目使用数字进行标记

```html
<ol>
    <li>第一项</li>
    <li>第二项</li>
</ol>
```

ol有type属性,嵌套

```html
1 数字
a 小写字母
A 大写字母
i 小写罗马字母
I 大写罗马字母
<ol type="1">
    <li>
    	水果
        <ol>
        	apple
            banana
        </ol>
    </li>
</ol>
```

## 列表标签之无序列表

项目列表，圆圈标记

```html
<ul>
    <li>
    	蔬菜
        <ul>
        	cai1
            cai2
        </ul>
    </li>
</ul>
```

type

- disc 默认实心圆
- circle空心圆
- square 小方块
- none 不显示

**有序列表和无序列表可以互相嵌套**

##  表格

单元格：同行等高，同列等宽

表格 table

行 tr

列 td

```html
<table>
    <tr>
        <td>apple</td>
        <td>banana</td>
    </tr>
    <tr>
        <td>banana</td>
        <td>apple</td>
    </tr>
</table>

快捷键
table>tr*3>td*3
```

表格属性

border=“1” 设置边框

width 宽度属性

height 高度属性

## 表格单元格合并

水平合并 colspan

垂直合并 rowspan

```html
<table>
    <tr>
        <td>单元格1</td>
        <td>单元格2</td>
        <td>单元格3</td>
        <td>单元格4</td>
        <td>单元格5</td>
    </tr>
    <tr>
        <td>单元格6</td>
        <td>单元格7</td>
        <td>单元格8</td>
        <td>单元格9</td>
        <td>单元格10</td>
    </tr>
    <tr>
        <td>单元格11</td>
        <td>单元格12</td>
        <td>单元格13</td>
        <td>单元格14</td>
        <td>单元格15</td>
    </tr>
    <tr>
        <td>单元格16</td>
        <td>单元格17</td>
        <td>单元格18</td>
        <td>单元格19</td>
        <td>单元格20</td>
    </tr>
    <tr>
        <td>单元格21</td>
        <td>单元格22</td>
        <td>单元格23</td>
        <td>单元格24</td>
        <td>单元格25</td>
    </tr>
</table>
```

## Form表单

所有用户输入的地方都用表单来填写，如登录注册搜索框

```html
<form action="url" method="get|post" name="myform">
```

**属性说明**

action 服务器地址

name 表单名称

**method中post和get的区别**

- 数据提交方式，get把提交的数据url可以看到，post看不到
- get一般用于提交少量数据，post用来提交大量数据

**表单元素**

一个完整的表单包含三个元素：表单标签，表单域(输入框)，表单按钮（提交）

```html
<form>
	<input type="text">
    <input type="submit">
</form>
```

## 表单元素

文本框

```html
<form>
	账号：<input type="text">
    密码：<input typr="text">
</form>
```

密码框

```html
<form>
        账号：<input type="text" ><br>
        密码：<input type="password"><br>
        <input type="submit" value="登录">
</form>

```

更改value “登录提交等等”

## 块元素和行内元素（内联元素）

**常见的块级元素,可以自动换行，可以调整大小**

```html
div form h1~h6 hr p table ul
```

**常见的内联元素，不可自动换行，不可调节大小**

```
a b em span i strong
```

**行内块级元素，不可自动换行，可以调节大小**

```
button img input
```

## H5新增语义化标签

```html
<div></div>
```

容器标签，把一个内容模块放在一个容器中，用于区分

```html
<header></header> 头部
<nav></nav>导航
<section></section>定义文档中的节，比如章节，页眉，页脚
<aside></aside>侧边栏
<footer></footer>脚部
<article></article>代表一个独立完整的相关内容块，比如一篇完整的论坛帖子，一篇博客文章，一个用户评论等等
```

# CSS 学习

**css的目的就是让网页具有美观一致的页面**

 选择器通常是需要改变样式的HTML元素

每条声明由一个属性和一个值组成

```css
写在<head></head>块中
<style>
h1{
    color : blue;
    font-size: 12px;
}
p{
    
}
</style>
```

## css的引用方式

**内联样式（行内样式）**

缺乏整体性和规划性，不利于维护，维护成本高

```html
<p style="background:orange;font-size:24px">CSS</p>
```

**内部样式**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        h1{
            color: blue;
        }
        p{
            color:blueviolet
        }
    </style>
</head>
<body>  
    <h1>This is a heading</h1>
    <hr>
    <p>
        首页跳转 链接如下
        <br>
        <a href="./test02.html">
            跳转到test02.html
        </a>
    </p>
</body>
</html>
```

**外部标签**

```html
<link rel="stylesheet" type="text/css" href="xx.css">
```

需要单独创建一个css文件

```css
p{
    color : red;
    font-size : 100px;
}
```

## 选择器一

**全局选择器**

可以与任何元素匹配，优先级最低，一般做样式初始化

```css
*{
	margin:0;
    padding:0;
}
```

**元素选择器**

学前端后学java标红java

```html
<p>学前端后学<span>java</span></p>
```

```css
span{
	color : red;
}
```

类选择器

```html
<a href="./link.html" class="content size">This is a link.</a>
```

class一个类可以放很多属性

```html
.content{

}
.size{

}
```

## 选择器二

**id选择器**

```css
#mytext{
	color ： "red"；
}
```

```html
<p id = "mytext"></p>
```

id和一个标签是一一对应的

**合并选择器**

```html
p,h3
{
	color ： "red";
}
<p></p>
<h3></h3>
类和标签都可以，中间逗号隔开就行
```

**优先级排行**

  行内样式>ID选择器＞类选择器＞元素选择器









































