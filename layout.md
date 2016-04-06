# NOTE1
###慕课笔记
####关于布局：

布局运用的三个方法：盒模型，浮动，绝对定位。

盒模型：从上到下顺序是border，content+padding,background-image,background-color,margin.

浮动：

- 浮动元素脱离标准文档流，向左/右移动，直到碰到包含框或者浮动框。
- 当元素设置了float属性不为none ，而且元素未设置高宽，那么它的高宽是随内容变化而变化的
- 浮动元素会对紧跟其后的元素和他的父元素造成影响
- 对紧跟其后的元素，消除影响用clear:both;对父元素使用overflow:hidden,width:100%.

绝对定位：

- abosolute和fixed是绝对定位；relative是相对定位
- 未设置偏移量时，绝对定位元素脱离了文档流，（z-index高于下面元素，它之后的元素会当他不存在而替代他的位置）但在原先初始的位置。
- 未设置高宽，高宽随内容变化；
- 设置了偏移量以后，值为absolute的元素以position不是static的最近父元素为参照，不然以<html>为参照。而fixed以可视窗口为参照。

Tips:

- 一般不设置高，而是让高随内容撑开。
- 如果是浮动元素或者是position:absolute,无法用margin:0 auto 居中。
- 横向两列布局，且一个为固定宽度而另一个为自适应时，自适应的用绝对定位，并且固定宽度的块一定要高于自适应的块高。
- fixed定位时注意margin重合的问题。
