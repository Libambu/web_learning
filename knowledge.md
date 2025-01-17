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

 

























