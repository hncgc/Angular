
# CSS

[CSS 教程](http://www.runoob.com/css/css-tutorial.html)  

[Less.js 中文文档](http://www.css88.com/doc/less/)  

[学习Less-看这篇就够了](https://segmentfault.com/a/1190000012360995)  

[Less 官网](https://less.bootcss.com/)  

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














