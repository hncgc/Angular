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


------------------

[JS - 简单的下载图片至本地](https://www.cnblogs.com/jzsz/p/8029536.html)  
~~~
<iframe id="saveImg" src="图片路径" style="display:none;"></iframe>
<a href="#" onclick="saveImg.document.execCommand('saveAs');">下载</a>
~~~

[使用JavaScript将图片保存至本地](https://www.cnblogs.com/zhangkaiqiang/p/8183926.html)  

[原生js 保存图片到本地](https://www.cnblogs.com/web-fusheng/p/8608430.html)  

[H5 -- （功能）基于html2canvas实现长按网页保存为图片到本地](https://blog.csdn.net/weixin_41076513/article/details/80896399)  

[HTML+JS下载图片到本地](https://blog.csdn.net/wuye_lh/article/details/80050393)  

[js下载图片(不让浏览器打开)](https://blog.csdn.net/liiil/article/details/80887155)  


-----------------------------

[js中怎么截取文件后缀名](https://zhidao.baidu.com/question/304974772611548764.html)  
~~~
var fileExtension = fileName.substring(fileName.lastIndexOf('.') + 1);

function getFileName(o){//通过第一种方式获取文件名
    var pos=o.lastIndexOf("\\");//查找最后一个\的位置
    return o.substring(pos+1); //截取最后一个\位置到字符长度，也就是截取文件名 
}
 
function getFileName2(o){//通过第二种方式获取文件名
    var arr = o.split('\\');//通过\分隔字符串，成字符串数组
    return arr[arr.length-1];//取最后一个，就是文件名
}
~~~

[js中截取文件的后缀名方法](https://blog.csdn.net/qq_34409900/article/details/80408235)  

[JS中如何删除某个指定字符(前)后的字符串](https://zhidao.baidu.com/question/292699810.html)  
~~~
var str;
var ipos;
str="123456789+abc";
ipos = str.indexOf("+");
str1=str.substring(0,ipos); //取前部分
str2=str.substring(ipos,str.length);//取后部分
~~~

[JS数组、字符串常用方法](https://www.cnblogs.com/songzk/p/6081883.html)  



------------------
[js中string转int把String类型转化成int类型](https://www.jb51.net/article/53680.htm)  
~~~
var j = parseInt("11");
~~~

---------------------

[JS设置 按钮为可用和不可用两种状态](https://blog.csdn.net/mengke1124/article/details/46532457)  
~~~
<input type="button" value="确定"  id="stamp" onclick="stampBill()">
<script>
//取stamp，
var stamp = document.getElementById("stamp");//设置盖章按钮为不可用
 
stamp.disabled=true;
//按钮变为不可点击
//按钮变为可以点击
//stamp.disabled=false;
</script>
~~~

[JS获取上一访问页面URL地址document.referrer实践](https://blog.csdn.net/Duan_Super/article/details/79987008)  

[js判断访客来源网址和关键字](https://www.cnblogs.com/zgzy/p/4341663.html)  

[js 判断字符串中是否包含某个字符串](https://www.cnblogs.com/xiaoshen666/p/10823381.html)  







