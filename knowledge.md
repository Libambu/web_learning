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

## 字体属性

**color**

```html
div{color : red;}
div{color:#ff0000}
div{color:rgb(255,0,0)}
div{color:rgba(255,0,0,1)}
```

rgba最后一个 参数是透明度 范围0~1

**font-size**

浏览器最低支持的字体大小是12px

**font-weight**

| 值      | 描述               |
| ------- | ------------------ |
| bold    | 定义粗体字符       |
| bolder  | 定义更粗字体       |
| lighter | 定义更细字体       |
| 100~900 | 400默认值，700bold |

**font-style字体样式**

| 值     | 描述   |
| ------ | ------ |
| normal | 默认值 |
| italic | 斜体字 |

**font-famliy**

P{

​	font-family:"Simsun";宋体

}

## 背景属性

| 属性                | 描述                 |
| ------------------- | -------------------- |
| background-color    | 设置背景颜色         |
| background-image    | 设置背景图片         |
| background-position | 设置背景图片显示位置 |
| background-repeat   | 设置背景图片如何填充 |
| background-size     | 设置背景图片大小属性 |

**backage-image属性**

图片默认放在左上角，图片不够大时会平铺图形

**backage-repeat**

| repeat    | 默认值           |
| --------- | ---------------- |
| repeat-x  | 只在水平方向平铺 |
| repeat-y  | 只在垂直方向平铺 |
| no-repeat | 不平铺           |

**backage-size**

长度，百分比

cover 保持纵横比覆盖背景

contain 保持纵横比，放在合适背景的最大大小

**backage-position属性**

x% y%

第一个值为水平位置，第二个值为垂直位置，左上角是00 右下角是100 100，默认为00

如果之指定了一个值，另外一个值是50

## 文本属性

**text-align**

指定元素文本的水平对齐方式

| 值     | 描述                 |
| ------ | -------------------- |
| left   | 文本居左排列，默认值 |
| right  | 文本排列到右边       |
| center | 把文本排列到中间     |

```
h1{text-align:center}
```

**text-decoration**

规定添加到文本的修饰，下划线，上划线，删除线

| 值           | 描述       |
| ------------ | ---------- |
| underline    | 定义下划线 |
| overline     | 定义上划线 |
| line-through | 定义删除线 |

**text-transform**

控制文本的大小写

| 值         | 描述                 |
| ---------- | -------------------- |
| captialize | 定义每个单词开头大写 |
| uppercase  | 定义全部大写         |
| lowercase  | 定义全部小写         |

**text-indent**

规定文本块中文本的缩进

```html
p{
	text-indent:50px;
}
```

负数值是允许的，如果值为负数，将第一行左缩进

## 表格属性

使用css可以使HTML更加美观

**表格边框**

```css
table,td{
	border:1px solid black
}
```

1px边框的大小

solid边框的属性，实线

black 无需多言

**只写table只是外边框有线了，加上td就有内边框了**

**折叠边框**

border-collapse属性设置表格的边框是否被折叠成一个单一的边框或者展开

```HTML
table{border-collapse:collapse}
table,td{border-collapse:collapse}
```

**表格宽度和高度**

width和height属性定义表格的宽度和高度

```css
table{width:100px;}
td{height:50px;}
```

**表格文字对齐**

表格中文本的水平和垂直对齐

水平对齐

```css
td {
	text-align:right;
}
```

垂直对齐

```css
td{
    height:50px;
    vertical-align:top/center/bottom;
}
```

**表格填充**

在表的内容中控制空格之间的边框，使用td和th

```css
 td
{
    padding:10px;
}
```

  **表格颜色**

```css
table,td,th{
	border:1px solid green;
}
td
{
	backage-color:green;背景颜色
    color:white;字体颜色
}
```

## 关系选择器

1. **后代选择器**
2. **子代选择器**
3. **相邻兄弟选择器**
4. **通用兄弟选择器**

**后代选择器**

​	定义：选择所有被E元素包含的F元素，中间用空格隔开

```css
E F{
	
}
```

**子代选择器**

​	定义：选择所有作为E元素的直接字元素F，对更深一层的元素不起作用，用>表示

```
E>F{

}
```

**相邻兄弟选择器**

​	定义：选择紧跟E元素后的F元素，选择相邻的对一个兄弟元素，只能向下选择

```css
E+F{
    
}
```

**通用兄弟选择器**

​	定义：选择E元素之后的所有兄弟元素F，用~隔开，只能向下选择

```css
E~F{
    
}
```

## box model

所有的HTML元素都可以看做盒子，在CSS中，boxmodel这一术语是用来设计和布局时使用

它包括外边框(margin)，边框(border)，内边距(padding)，实际内容(content)

```html
<body>
    <div>
    	我是内容
    </div>
</body>
```

```css
<style>
div{
    width:100px;
    height:100px;
    backage-color:green;
    padding(内边距):50px(上下大小)10px;(左右大小)和内容的颜色一致
    border(边框):5px solid blue;
    Margin(外边距):50px;完全透明的，把周围的撑开
}
</style>
```

padding和margin也可以分四个方向来写，便于精细控制

```css
<style>
	div{
		padding-left:50px;
        padding-right:50px;
        padding-top:50px;
        padding-bottom:20px;
}
</style>
```

## 弹性盒子模型

弹性盒是一种当页面需要适应不同的屏幕大小以及设备类型时确保元素具有恰当的行为的布局方式

**css3弹性盒子内容**

弹性盒子由弹性容器(Flex container)和弹性子元素(Flex item)组成

弹性容器通过设置display属性的值为flex将其定义为弹性容器

弹性容器内包含了一个或多个弹性子元素

**弹性容器外以及谈弹性元素内是正常渲染的。弹性盒子只是定义了弹性字元素如何在弹性容器内布局**

**默认弹性盒子是横向摆放的**

**flex-direction属性，指定弹性元素在父容器中的位置**

```css
flex-dirction:row|row-reverse|column|column-reverse
```

```css
.flex-container{
    display:flex;
    flex-direction:colum;
    width:400px;
    height:250px;
    backage-color:lightgrey
}
```

**justify-content属性，规定垂直方向的对齐**

```css
justify-content:flex-start|flex-end|center
```

 **align-items属性，水平方向的对齐方式**

```css
align-items:flex-start|flex-end|center
```

**子元素上的属性：flex-grow**

根据弹性盒子所设置的扩展因子作为比率来分配空间

默认值为0，即如果存在剩余空间，也不放大

如果只有一个子元素设置，那么按照扩展因子转化的百分比对其分配剩余空间。超出按100%

```html
.flex-container{
	display:flex;
	
}
.flex-item1{
	flex:1;
}
.flex-item2{
	flex:1;
}
.flex-item3{
	flex:2;
}
```

三个item分配比例：1:1:2

## 浮动

增加一个浮层来放置内容

float属性定义元素在哪个方向浮动，任何元素都可以浮动

| 值    | 描述         |
| ----- | ------------ |
| left  | 元素向左浮动 |
| right | 元素向右浮动 |

**浮动的原理**

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        div{
            width: 2500px;
            background-color: bisque;
        }
        img{
            width: 300px;
            height: auto;
            border: 1px solid #ccc;
        }
        .fix{
            float: left;
        }
        ul li{
            float: left;
            border: 100px solid white;
            font-size: 20px;
        }
    </style>
</head>
<body>
    <div>
        <img src="./111.jpg" alt="111">
        <img src="./111.jpg" alt="111">
    </div>
    <p>这样写两个图片会有间隙，可以用float:left;来解决</p>
    <div >
        <img class="fix" src="./111.jpg" alt="111">
        <img class="fix" src="./111.jpg" alt="111">       
    </div>
    <div>
        <p style="clear: both;">脱离文档流实现水平摆放</p>
    </div>
    <div>
        <ul>
            <li>
                <a href="#">导航一</a>
            </li>
            <li>导航二</li>
            <li>导航三</li>
            <li>导航四</li>
        </ul>
    </div>
    <div>
        当空间不足时元素会选择横向摆放
    </div>
</body>
</html>

## 清除浮动

副作用：

1、浮动元素会造成父元素高度塌陷

2、后续元素会受到影响

**清除浮动方法**

1、父元素设置高度

2、受影响的元素增加clear属性

3、overflow清除浮动

4、伪对象方法

## 定位

| 值       | 描述     |
| -------- | -------- |
| relative | 相对定位 |
| absolute | 绝对定位 |
| fixed    | 固定定位 |

其中，绝对定位和固定定位会脱离文档流

设置定位后，可以使用四个方向进行调整：left top right bottom

**相对定位**

```html
<div class="box"></div>
```

```css
.box{
    width:200px;
    height:200px;
    background-color:red;
    position:relative;
    left:100px
}
```

相对定位不脱离文档流

**绝对定位**

```html
<div class="box1"></div>
<div class="box2"></div>
```

```css
.box1{
    width:200px;
    height:200px;
    background-color:red;
    position:absolute;
    left:50px;
}
.box2{
    width:300px;
    height:200px;
    backage-color:green;
}
```

**box1会脱离文档流，覆盖在box2的上方**

**固定定位**

```html
<div class="box1"></div>
```

```css
.box1{
    width:200px;
    height:200px;
    background-color:red;
    position:fixed;
    left:50px;
}
```

**固定定位也会脱离标准流，而且不会随页面滑动杆**

 **设置定位之后，相对定位和绝对定位他是相对具有定位的父级元素进行位置调整，如果父级元素不存在定位，则继续向上逐级寻找，直到顶层文档**

**Z-index**

**Z-index**用于设置元素的堆叠顺序，拥有更高堆叠顺序的元素总是处在堆叠状态较低的元素前面

```css
.box1{
    postion:absolute;
    z-index:1;
}
.box2{
    postion:absolute;
    z-index:2;
}
```

## css3新特性

**圆角**

boeder-radius属性

四个值：左上，右上，右下，左下

两个值：左上右下，右上左下

一个值：四个圆角都相同

```css
.box1{
   boeder-radius:10px 20px 10px 10px;
    boeder-radius:100%;
    完全就是一个圆
}
```

**阴影**

box-shadow 向框添加一个或多个阴影

```css
box-shadow:h-shadow v-shadow blur color
```

| 值       | 描述                 |
| -------- | -------------------- |
| h-shadow | 必选，水平阴影的位置 |
| v-shadow | 必选，垂直阴影的位置 |
| blur     | 可选，迷糊距离       |
| color    | 可选，阴影的颜色     |

## 动画

动画是使元素从一种样式逐渐变为另一种样式的效果

可以改变任意多的样式，任意多的次数

用百分比来规定变化发生的时间，或者用关键词from和to，等同于0%和100%

**@keyframes创建动画**

```css
{
    <style>
		@keyframs name{
    		from|0%{
        		css样式
    		}
    		percent{
        		css样式
    		}
    		to|100%{
				css样式
    		}
		}
    	<div>
    		width:100px;
    		height:100px;
    		animation:name 3s liner 0 infinite normal
    	</div>
    </ style>
}
```

percent是百分比

animation执行动画

```css
animation:name duration timing delay iteration-count direction
```

| 值                   | 描述                                              |
| -------------------- | ------------------------------------------------- |
| name                 | 设置动画名称                                      |
| duration             | 设置动画持续时间                                  |
| timing-function      | 设置动画的速率                                    |
| delay                | 设置动画开始的时间                                |
| iteration-count      | 设置循环次数，infinite为无限循环                  |
| direction            | 设置动画播放的方向                                |
| animation-play-state | 控制动画播放的状态，running为播放，paused代表暂停 |

| timing-function | 描述             |
| --------------- | ---------------- |
| ease            | 逐渐变慢（默认） |
| linear          | 匀速             |
| ease-in         | 加速             |
| ease-out        | 减速             |
| ease-in-out     | 先加速再减速     |

| direction值 | 描述                         |
| ----------- | ---------------------------- |
| normal      | 默认值为向前播放             |
| alternate   | 第偶次向前播放，奇次反向播放 |

## 精灵图

一种前端页面图片应用处理方式。它允许你将一个页面涉及到的所有零星图片都包含在一张大图中

原理：

1、通过backage-image引入背景图片

2、通过background-position把背景图片移动到自己需要的位置

```html
<i class="icon1"></i>
<i class="icon2"></i>
```

```css
.icon1{
    display:black;
    background-image:url(1.png);
    background-position:-20px 0;
    width 45px;
    height 70px;
}
.icon2{
    display:black;
    background-image:url(1.png);
    background-position:-93px -84px;
    width 45px;
    height 70px;
}
```































 

































































































































































