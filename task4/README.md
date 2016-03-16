# 说明
一定程度上考虑了自适应问题，同时运用了多种垂直居中和水平居中的方法

## 第一个div
### 灰色部分：
水平居中使用`text-align: center;`
垂直居中使用`vertical-align: middle;`
其中需要规定欲居中元素`display: inline-block;`和`line-height: 600px;`

### 黄色圆角部分：
外层div设置`position: relative;`
内层圆角设置`position: absolute;`

## 第二个div
### 灰色部分：
水平,垂直居中使用`position: absolute; top: 50%; left: 50%;`
然后规定负值的margin`margin: -100px 0 0 -200px;`

### 黄色圆角部分：
原理同上，但是因为灰色`div`层已经规定`position: absolute`，所以用一个`div`包住圆角所在`div`，实现相对于外层元素的绝对定位

## 第三个div
### 灰色部分： 
水平居中： `margin: 0 auto;`和`width: 400px;`
垂直居中： 构建了一个占位元素，使其高度为50%，同时设置负值的margin，使得需要的元素垂直居中

### 黄色圆角部分：
同第一个div

## 第四个div

### 灰色部分：
水平和垂直居中:通过设置外层`div`的`postion: relative;` 内层`div`的`postion: absolute;right: 0;left: 0;top: 0;bottom: 0;` `margin: auto;`

### 黄色部分
通过设置`float: right;`和`margin-top: 100px;`