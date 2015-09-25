### fixednav 问题记录 ###
###滚动页面时，选中导航中对应项目###

* **问题描述** ：domready在图片未加载完成时已经执行，如果导航对应锚点项目中，有图片width:100%，高度不确定时，由于图片未加载完成，初始化时获取到的导航锚点项 ''<nowiki>item.offset().top</nowiki>'' 有可能是错误的，所以在滚动页面时，会出现提前选中某项目（此时还未看到该项目的内容）。
* **解决方法** ：给未确定高度的图片占位，即css中设置img的父级div的padding-top:图片高宽比，并且设置img的position为absolute。

* **代码示例** ：
<code css>
/*padding-top为高宽比=图片高度/图片宽度*100 ex:203(imgh)/640(imgw)*100% = 32%*/
.item-pic{padding-top: 32%; display: block; position: relative; z-index: 2;} 
.item-pic img{width: 100%; position: absolute; left: 0; top: 0; z-index: 0;}
</code>