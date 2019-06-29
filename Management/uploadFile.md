Web文件上传
===

[对象存储 OSS](https://help.aliyun.com/product/31815.html?spm=a2c4g.11186623.6.540.130f58a8aVIevh)  

[对象存储 OSS > 开发指南 > 使用前须知](https://help.aliyun.com/document_detail/31890.html?spm=a2c4g.11186623.3.2.4e9941f04ajg0d)  

[权限控制概述](https://help.aliyun.com/document_detail/31867.html?spm=a2c4g.11186623.3.3.f8ba41f0ZAgJl2)  

[STS临时授权访问OSS](https://help.aliyun.com/document_detail/100624.html?spm=a2c4g.11186623.2.10.4e9941f0nYVmqS)  



------------


[阿里云-对象存储 OSS > SDK 示例 > Node.js > 上传文件 > 上传本地文件](https://help.aliyun.com/document_detail/111265.html?spm=a2c4g.11186623.2.7.369a2778Bg9mOB#concept-uxl-2vb-dhb)  

[阿里云-对象存储 OSS > SDK 示例 > Node.js > 安装](https://help.aliyun.com/document_detail/32068.html?spm=a2c4g.11186623.2.7.1e6b77a3vmDt0E#concept-32068-zh)  
Github地址: https://github.com/ali-sdk/ali-oss?spm=a2c4g.11186623.2.12.73b2165asJOtlu

[OSS in Browser](https://github.com/ali-sdk/ali-oss/tree/master/example)  

[OSS Browser 提供类似windows资源管理器功能。用户可以很方便的浏览文件，上传下载文件，支持断点续传等](https://github.com/luozhang002/oss-browser)  

[Alibaba Cloud OSS SDK for Android](https://github.com/luozhang002/aliyun-oss-android-sdk)  

[Alibaba Cloud OSS SDK for iOS](https://github.com/luozhang002/aliyun-oss-ios-sdk)  

---------------

[阿里云视频文件的上传文件方法](https://help.aliyun.com/knowledge_detail/50618.html?spm=5176.2000002.0.0.6e653106qiibI2)  

[媒体处理 > SDK参考 > 上传SDK > 使用说明](https://help.aliyun.com/document_detail/48467.html?spm=a2c4g.11186623.2.19.3244501cXqwTpr)  

[媒体处理 > SDK参考 > 上传SDK > 使用说明-JavaScript版本](https://help.aliyun.com/document_detail/48471.html?spm=a2c4g.11186623.2.11.5fc64112ZeW4QR#concept-rk5-pv5-y2b)  

[媒体处理 > SDK参考 > 上传SDK > 上传SDK下载](https://help.aliyun.com/document_detail/48501.html?spm=a2c4g.11186623.2.11.1a785972y7vGjM#concept-k1z-vkv-y2b)  

[阿里云OSS文件上传（前端js文件直传方法）](https://blog.csdn.net/weixin_37626925/article/details/91360197)  
~~~
function upFile(el){
    // el为上传文件的元素
    // ----步骤1-------------------------------------------------
    var client = new OSS.Wrapper({
        region: "oss-cn-hangzhou", //阿里云获取
        accessKeyId: "yourAccessKeyId",
        accessKeySecret: "yourAccessKeySecret",
        bucket: "bucketName"  //要存储的目录名
    });
    // ----步骤2-------------------------------------------------
    var suffix = el.value.substr(el.value.indexOf(".")); // 获取文件后缀名
    var filename = new Date().getTime() + suffix; // 为文件命名
    client.multipartUpload("fileName/" + filename, el.files[0]).then(function (result){
        var url = result.res.requestUrls[0];
        var length = url.lastIndexOf('?');
        var imgUrl = length>0?url.substr(0,length):url; // 文件最终路径
        console.log(imgUrl);
    }).catch(function (err) {
        console.log(err);
    });
}
~~~

[阿里云oss js前端获取签名直传文件](https://blog.csdn.net/hch15112345824/article/details/78547190)  

[阿里云oss对象存储 js web直传中文件重命名和文件数量限制问题的解决](https://blog.csdn.net/qq_30377913/article/details/76571916)  

[阿里的oss文件上传前端代码,以及提交参数](https://blog.csdn.net/tomMMMMMMMMMMM/article/details/81001874)  

[JavaScript客户端直传OSS，服务端签名](https://blog.csdn.net/Vue2018/article/details/84322889)  

[JavaScript客户端签名直传](https://help.aliyun.com/document_detail/31925.html#concept-frd-4gy-5db)  

[JavaScript服务端签名后直传](https://help.aliyun.com/document_detail/31926.html)  

[服务端签名直传并设置上传回调](https://help.aliyun.com/document_detail/31927.html?spm=a2c4g.11186623.2.14.17f16e28EU8HNt#concept-qp2-g4y-5db)  

[oss 阿里云 javascript 上传图片](https://blog.csdn.net/shidewen1125/article/details/53442820)  

[js上传文件 -帮助文档- 阿里云](https://help.aliyun.com/wordpower/610868-1.html)  


-----------------

[h5上传视频文件](https://www.cnblogs.com/huiseshijie/p/8479536.html)  

[一般网站视频处理的方式 用户上传 各大主流视频站调用分享功能代码](https://blog.csdn.net/qq_27905477/article/details/80616416)  

[网站后台——用户上传图片剪切](https://blog.csdn.net/RZ_J9pp/article/details/89761873)  

[网站后台视频上传方式](https://jingyan.baidu.com/article/59703552d0a5918fc007409e.html)  

[网站后台添加视频](https://segmentfault.com/q/1010000010191583)  




[根本上解决npm install 报错“ajv-keywords@3.4.0 requires a peer of ajv@^6.9.1 but none is installed. You must install peer dependencies yourself.“](https://www.cnblogs.com/yalong/p/10406190.html)  
~~~
更新本机的npm到最新版本：npm install -g npm
~~~


[Browserify](https://www.jianshu.com/p/8d8b8752d8a0)  



