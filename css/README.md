
# CSS

[CSS 教程](http://www.runoob.com/css/css-tutorial.html)  

CSS
---

[六种实现元素水平居中](https://www.w3cplus.com/css/elements-horizontally-center-with-css.html)  

[纯CSS实现垂直居中的几种方法](https://www.cnblogs.com/hutuzhu/p/4450850.html)  

[用CSS/CSS3 实现 水平居中和垂直居中的完整攻略](https://blog.csdn.net/summer_lover_/article/details/66479576)  

[css text-decoration下划线 删除线 上划线属性样式](http://www.divcss5.com/rumen/r129.shtml)  

[DIV CSS如何给文字字体添加下划线？](http://www.divcss5.com/wenji/w586.shtml)  

[CSS巧妙实现分隔线的几种方法](https://blog.csdn.net/jian_xi/article/details/72572393)  

[里面的div怎么撑开外面的div让高度自适应](https://www.cnblogs.com/xiaoxiao2014/p/5474620.html]

Less
---

[Less.js 中文文档](http://www.css88.com/doc/less/)  

[学习Less-看这篇就够了](https://segmentfault.com/a/1190000012360995)  

[Less 官网](https://less.bootcss.com/)  

Less安装
---

~~~
C:\Users\Chun>npm install -g less
C:\Users\Chun\AppData\Roaming\npm\lessc -> C:\Users\Chun\AppData\Roaming\npm\nod
e_modules\less\bin\lessc
+ less@3.8.1
added 59 packages in 11.809s

C:\Users\Chun>

D:\www\css>lessc -v
lessc 3.8.1 (Less Compiler) [JavaScript]

D:\www\css>lessc global.less > global.css

D:\www\css>lessc index.less >index.css

~~~

[CSS3 @media 查询](http://www.runoob.com/cssref/css3-pr-mediaquery.html)  
https://c.runoob.com/codedemo/5371

[Css3中的媒体查询@media](https://www.cnblogs.com/clean/p/7595776.html)  
~~~
<link rel+"stylesheet" media="screen and (orientation: portrait)" href="portrait-screen.css"/>
//设置了媒体类型和媒体特性（显示屏， 纵向放置）


<link rel="stylesheet" media="not screen and (orientation: portrait)" href="portrait-
screen.css" />
//非纵向放置的显示屏

<link rel="stylesheet" media="screen and (orientation: portrait) and (min-width:800px)" href="800wide-portrait-screen.css" />
//限制只有视口宽度大于800px像素的显示屏设备才能加载此文件
~~~

媒体查询列表（需要用逗号隔开）：  
~~~
<link rel="stylesheet" media="screen and (orientation: portrait) and (min-width:800px), projection" href="800wide-portrait-screen.css" />
~~~

除了以上方法还可以使用CSS中的@import指令在当前样式表中按条件引入其他样式表。（使用@import方法会增加HTTP请求影响加载速度）  
~~~
@import url("phone.css") screen and (max-width:360px);
~~~

Foundation
---

[Foundation中文网](http://foundation.org.cn/)  

[Foundation5 教程](http://www.runoob.com/foundation/foundation-tutorial.html)  


[HTML中的 UL 标签中li横向排列](https://blog.csdn.net/leewokan/article/details/6626774)   
  
[HTML_水平线详解](https://blog.csdn.net/admin_maxin/article/details/54572740)  


js
---

[最简单的jQuery轮播图](http://www.jq22.com/webqd656)  

[带按钮控制轮播焦点图代码](http://www.jsdaima.com/js/189.html)  

[jquery.flexslider.js带左右箭头且带按钮可滚动的图片插件](https://www.cnblogs.com/linjiaxin/p/5960998.html)  











