javascript
===


[JavaScript 教程](http://www.w3school.com.cn/js/)  

[JavaScript教程](https://www.liaoxuefeng.com/wiki/001434446689867b27157e896e74d51a89c25cc8b43bdb3000)  

---------------

[js中var、let、const区别](https://www.cnblogs.com/songyifan427/p/9957752.html)  

[JS中let和var的区别](https://www.cnblogs.com/asand/p/7205632.html)  

---------------

延迟
---

[js中的延迟执行和定时执行](http://www.jq22.com/webqd164)  

[js页面长时间无操作执行](http://www.jq22.com/webqd2456)  


-------------

[js关闭当前页面(窗口)的几种方式总结](https://www.cnblogs.com/chuhj/p/7131759.html)  
~~~
<a href="javascript:window.opener=null;window.open('','_self');window.close();"><img src="images/ic_action_cancel_black.png"/></a>
~~~

[js ---任何浏览器关闭当前网页的代码](https://www.cnblogs.com/Nico-luo/p/8029772.html)  

[js中关闭当前页面并刷新父页面](https://blog.csdn.net/qq_34275268/article/details/81161826)  
~~~
window.parent.opener.location.reload();
window.close(); 
~~~



[关于js返回上一页的实现方法](https://www.cnblogs.com/wlqh/p/5948879.html)  
~~~
下面是常用代码：

<a href="<a href="javascript :history.back(-1)">返回上一页</a>
或
<a href="javascript :;" onClick="javascript :history.back(-1);">返回上一页</a>

如果是用按钮做的话就是：
<input type="button" name="Submit" onclick="javascript:history.back(-1);" value="返回上一页">

用图片做的话就是：
<a href="javascript :;" onClick="javascript :history.back(-1);"><img src="图片路径" border="0" title="返回上一页"></a>


[color=#FF0000]几秒钟后[/color]自动返回上一页代码:（加入两个head间，3000表示3秒）
<SCRIPT language=javascript>
function go()
{
window.history.go(-1);
}
setTimeout("go()",3000);
</SCRIPT>
~~~

[js中实现页面跳转（返回前一页、后一页）](https://www.cnblogs.com/amingxiansen/p/9074596.html)  
~~~
<a href="javascript:history.go(-1)">返回上一页</a> 
<a href="javascript:location.reload()">重载页面，本地刷新</a> 
<a href="javascript:history.go(-1);location.reload()">返回上一页重载页面，本地刷新</a> 

<a href="#" onclick="self.location=document.referrer;">返回</a> 

自动刷新页面的方法:
1.页面自动刷新：把如下代码加入<head>区域中
<meta http-equiv="refresh" content="20">  
2.页面自动跳转：把如下代码加入<head>区域中
<meta http-equiv="refresh" content="20;url=http://www.javaeye.com">  
其中20指隔20秒后跳转到http://www.javaeye.com页面
3.页面自动刷新js版

<script language="JavaScript">
function myrefresh()
{
       window.location.reload();
}
setTimeout('myrefresh()',1000); //指定1秒刷新一次
</script>
~~~

[js跳转页面与打开新窗口的方法](https://www.cnblogs.com/lijshui/p/7451360.html)  



