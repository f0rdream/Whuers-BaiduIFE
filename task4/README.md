# 说明
一定程度上考虑了自适应问题，同时运用了多种垂直居中和水平居中的方法
## 第一个div
灰色部分：
水平居中使用`text-align: center`
垂直居中使用`vertical-align: middle`
其中需要规定欲居中元素`display: inline-block`和`line-height: 600px`

黄色圆角部分：
外层div设置`position: relative`
内层圆角设置`position: absolute`
## 第二个div
灰色部分：
水平,垂直居中使用`position: absolute; top: 50%; left: 50%;`
然后规定负值的margin`margin: -100px 0 0 -200px`

黄色圆角部分：
原理同上，但是因为灰色div层已经规定`position: absolute`，所以用一个div包住圆角所在div
## 第三个div



说明正在施工中