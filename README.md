# Angular

Angular

https://github.com/Mavlarn/Angular2-tutorial-Chinese

Angular2框架

[Angular2教程](https://www.w3cschool.cn/angular2/)  

[在手机上查看文档](https://m.w3cschool.cn/angular2/)  

[Webstorm](https://github.com/hncgc/Angular/tree/master/IDE)  

[Node.js](https://github.com/hncgc/Angular/tree/master/Node)  

[TypeScript](https://github.com/hncgc/Angular/tree/master/TypeScript)  

[WebSocket](https://github.com/hncgc/Angular/tree/master/WebSocket)  
 

[NPM 使用介绍](http://www.runoob.com/nodejs/nodejs-npm.html)  

使用淘宝 NPM 镜像
~~~
大家都知道国内直接使用 npm 的官方镜像是非常慢的，这里推荐使用淘宝 NPM 镜像。

淘宝 NPM 镜像是一个完整 npmjs.org 镜像，你可以用此代替官方版本(只读)，同步频率目前为 10分钟 一次以保证尽量与官方服务同步。

你可以使用淘宝定制的 cnpm (gzip 压缩支持) 命令行工具代替默认的 npm:

$ npm install -g cnpm --registry=https://registry.npm.taobao.org
这样就可以使用 cnpm 命令来安装模块了：

$ cnpm install [name]
更多信息可以查阅：http://npm.taobao.org/。
~~~

[npm太慢， 淘宝npm镜像使用方法](https://blog.csdn.net/quuqu/article/details/64121812)  
~~~
淘宝 npm 地址： http://npm.taobao.org/
1.临时使用
npm --registry https://registry.npm.taobao.org install express
1
2.持久使用
npm config set registry https://registry.npm.taobao.org
1
配置后可通过下面方式来验证是否成功 
npm config get registry
或 
npm info express

3.通过cnpm使用
npm install -g cnpm --registry=https://registry.npm.taobao.org
1
使用 
cnpm install express
~~~

[淘宝 NPM 镜像](http://npm.taobao.org/)  

~~~
C:\Users\HP>npm install -g cnpm --registry=https://registry.npm.taobao.org
npm WARN deprecated socks@1.1.10: If using 2.x branch, please upgrade to at least 2.1.6 to avoid a serious bug with socket data flow and an import issue introduced in 2.1.0
C:\Users\HP\AppData\Roaming\npm\cnpm -> C:\Users\HP\AppData\Roaming\npm\node_modules\cnpm\bin\cnpm
+ cnpm@6.0.0
added 629 packages from 837 contributors in 49.465s

C:\Users\HP>cnpm -v
cnpm@6.0.0 (C:\Users\HP\AppData\Roaming\npm\node_modules\cnpm\lib\parse_argv.js)
npm@6.4.0 (C:\Users\HP\AppData\Roaming\npm\node_modules\cnpm\node_modules\npm\lib\npm.js)
node@8.11.3 (C:\Program Files\nodejs\node.exe)
npminstall@3.11.0 (C:\Users\HP\AppData\Roaming\npm\node_modules\cnpm\node_modules\npminstall\lib\index.js)
prefix=C:\Users\HP\AppData\Roaming\npm
win32 x64 10.0.17134
registry=https://registry.npm.taobao.org

C:\Users\HP>

~~~

[npm 切换淘宝镜像几种方式](https://blog.csdn.net/yuanyuanispeak/article/details/79480904)  

~~~
C:\Users\HP>npm config get registry
https://registry.npmjs.org/

C:\Users\HP>npm info express

express@4.16.3 | MIT | deps: 30 | versions: 259
Fast, unopinionated, minimalist web framework
http://expressjs.com/

keywords: express, framework, sinatra, web, rest, restful, router, app, api

dist
.tarball: https://registry.npmjs.org/express/-/express-4.16.3.tgz
.shasum: 6af8a502350db3246ecc4becf6b5a34d22f7ed53
.unpackedSize: 205.6 kB

dependencies:
accepts: ~1.3.5            cookie: 0.3.1              finalhandler: 1.1.1        path-to-regexp: 0.1.7
array-flatten: 1.1.1       debug: 2.6.9               fresh: 0.5.2               proxy-addr: ~2.0.3
body-parser: 1.18.2        depd: ~1.1.2               merge-descriptors: 1.0.1   qs: 6.5.1
content-disposition: 0.5.2 encodeurl: ~1.0.2          methods: ~1.1.2            range-parser: ~1.2.0
content-type: ~1.0.4       escape-html: ~1.0.3        on-finished: ~2.3.0        safe-buffer: 5.1.1
cookie-signature: 1.0.6    etag: ~1.8.1               parseurl: ~1.3.2           send: 0.16.2
(...and 6 more.)

maintainers:
- dougwilson <doug@somethingdoug.com>
- hacksparrow <captain@hacksparrow.com>
- jasnell <jasnell@gmail.com>
- mikeal <mikeal.rogers@gmail.com>

dist-tags:
latest: 4.16.3

published 5 months ago by dougwilson <doug@somethingdoug.com>

C:\Users\HP>

~~~

[后台管理](https://github.com/hncgc/Angular/tree/master/Management)  

[在线测试](http://coolaf.com/)  

[Editor](https://github.com/hncgc/Angular/tree/master/Editor)  




