# TypeScript  

[TypeScript 教程 | 菜鸟教程](http://www.runoob.com/typescript/ts-tutorial.html)  

[TypeScript 中文手册](https://typescript.bootcss.com/)  

[深入理解 TypeScript](https://jkchao.github.io/typescript-book-chinese/)  

[TypeScript案例](https://www.tslang.cn/samples/index.html)  

[TypeScript-Node-Starter](https://github.com/Microsoft/TypeScript-Node-Starter#typescript-node-starter)

[Use TypeScript to Build a Node API with Express](https://developer.okta.com/blog/2018/11/15/node-express-typescript)  

[TypeScript教程](https://www.w3cschool.cn/typescript/typescript-tutorial.html)  

[TypeScript](https://www.tslang.cn/docs/handbook/typescript-in-5-minutes.html)   

[TypeScript](https://github.com/Microsoft/TypeScript/wiki)  
https://www.tslang.cn/  

[TypeScript 从入门到放弃](https://www.jianshu.com/p/c5005fad4274)  

[TypeScript中文网](https://www.tslang.cn/)  

[Typescript简介和安装](https://blog.csdn.net/xcg132566/article/details/76098753)   

安装简单总结：安装node-->npm安装typescript的compiler-->配置IDE-->编码运行   

[TypeScript 安装](https://blog.csdn.net/adelais__/article/details/79181474)  

[TypeScript官网](http://www.typescriptlang.org/index.html)  
~~~
安装Node.js，官网：https://nodejs.org/en/，LTS和Current都行，建议LTS；下载完成双击打开就可以，如下图  
~~~

下载node-v8.11.3-x64.msi  

添加到环境变量里面，C:\Program Files\nodejss 安装时已自动添加  
~~~
C:\Users\HP>node -v  
v8.11.3  
C:\Users\HP>npm -v  
5.6.0  
~~~

使用npm安装typescript，在命令提示符界面输入命令npm install -g typescript安装typescript和命令tsc -v查看其版本号  

C:\Users\HP>npm install -g typescript  
npm ERR! Unexpected end of JSON input while parsing near '...ake":"latest","merge2'  

npm ERR! A complete log of this run can be found in:  
npm ERR!     C:\Users\HP\AppData\Roaming\npm-cache\_logs\2018-08-11T15_37_19_183Z-debug.log  

C:\Users\HP>  

[Unexpected end of JSON input while parsing near错误解决办法](https://blog.csdn.net/m0_37836194/article/details/79107785)  
~~~
npm install出现”Unexpected end of JSON input while parsing near”的错误。

运行  npm cache clean --force。

C:\Users\HP>npm cache clean --force
npm WARN using --force I sure hope you know what you are doing.

C:\Users\HP>
~~~

C:\Users\HP>npm install -g typescript   
~~~
npm ERR! code EINTEGRITY
npm ERR! sha512-zQIMOmC+372pC/CCVLqnQ0zSBiY7HHodU7mpQdjiZddek4GMj31I3dUJ7gAs9o65X7mnRma6OokOkc6f9jjfBg== integrity checksum failed when using sha512: wanted sha512-zQIMOmC+372pC/CCVLqnQ0zSBiY7HHodU7mpQdjiZddek4GMj31I3dUJ7gAs9o65X7mnRma6OokOkc6f9jjfBg== but got sha512-grzsNRkoU3z1ZaH/3zfLBdzZERd/5+9eqHS6o8JyL5M9LqtuMnSrzprnYSn5JobtsPtIcpit5JSklgQ6qNWypg==. (7043689 bytes)

npm ERR! A complete log of this run can be found in:
npm ERR!     C:\Users\HP\AppData\Roaming\npm-cache\_logs\2018-08-11T15_55_19_863Z-debug.log

C:\Users\HP>

C:\Users\HP\AppData\Roaming\npm-cache\_logs\2018-08-11T15_55_19_863Z-debug.log
0 info it worked if it ends with ok
1 verbose cli [ 'C:\\Program Files\\nodejs\\node.exe',
1 verbose cli   'C:\\Program Files\\nodejs\\node_modules\\npm\\bin\\npm-cli.js',
1 verbose cli   'install',
1 verbose cli   '-g',
1 verbose cli   'typescript' ]
2 info using npm@5.6.0
3 info using node@v8.11.3

C:\Users\HP\AppData\Roaming\npm-cache\anonymous-cli-metrics.json
{"metricId":"c53eccb7-1a9b-4765-b26e-c10677ea0c52","metrics":{"from":"2018-08-11T15:37:19.175Z","to":"2018-08-11T15:55:19.853Z","successfulInstalls":0,"failedInstalls":2}}
~~~

[code EINTEGRITY，npm安装时候报错](https://www.cnblogs.com/zhaixr/p/7307718.html)  
~~~
解决方法：

1.如果有package-lock.json文件，就删掉

2.管理员权限进入cmd

3.执行npm cache clean --force

4.之后再npm install

有时候网不好也会出现问题，多试几次。
~~~

C:\Users\HP>npm install -g typescript  
[       ...........] - extract:typescript: verb lock using C:\Users\HP\AppData\Roaming\npm-cache\_locks\staging-44c5448c6858e3d9.lock for C:\Users\HP\AppDat   

npm install 提示 ERR! code EINTEGRITY
https://blog.csdn.net/Mr_rain/article/details/74551497

~~~
先运行 
npm i -g npm
再运行 
grep -ir “sha1-W/Rejkm6QYnhfUgnid/RW9FAt7Y= integrity chexxxxxxxxxxxxxxxxxxxxxxxxxxxxDUqxF47jfwOgvK2UM16SEXk=” ~/.npm

C:\Users\HP>npm i -g npm
C:\Users\HP\AppData\Roaming\npm\npx -> C:\Users\HP\AppData\Roaming\npm\node_modules\npm\bin\npx-cli.js
C:\Users\HP\AppData\Roaming\npm\npm -> C:\Users\HP\AppData\Roaming\npm\node_modules\npm\bin\npm-cli.js
+ npm@6.3.0
added 396 packages in 111.982s
~~~


C:\Users\HP>grep -ir "sha1-W/Rejkm6QYnhfUgnid/RW9FAt7Y= integrity chexxxxxxxxxxxxxxxxxxxxxxxxxxxxDUqxF47jfwOgvK2UM16SEXk=" ~/.npm
'grep' 不是内部或外部命令，也不是可运行的程序
或批处理文件。
~~~
C:\Users\HP>npm install -g typescript
C:\Users\HP\AppData\Roaming\npm\tsc -> C:\Users\HP\AppData\Roaming\npm\node_modules\typescript\bin\tsc
C:\Users\HP\AppData\Roaming\npm\tsserver -> C:\Users\HP\AppData\Roaming\npm\node_modules\typescript\bin\tsserver
+ typescript@3.0.1
added 1 package from 1 contributor in 377.309s

C:\Users\HP>tsc -v
Version 3.0.1

C:\Users\HP>
~~~

资料：https://github.com/npm/npm/issues/16861

[npm ERR! code EINTEGRITY问题解决方案](https://blog.csdn.net/u011218378/article/details/78250103)  

[搭建TypeScript开发环境](https://blog.csdn.net/diligentkong/article/details/74781539)  

~~~
F:\typesc\Hello.ts
export class Hello{

} 


C:\Users\HP>f:

F:\>cd typesc

F:\typesc>tsc Hello.ts

F:\typesc>

F:\typesc\Hello.js
"use strict";
exports.__esModule = true;
var Hello = /** @class */ (function () {
    function Hello() {
    }
    return Hello;
}());
exports.Hello = Hello;

然后在终端运行 alm 即可。

F:\typesc>node -v
v8.11.3

F:\typesc>npm -v
6.3.0

F:\typesc>tsc -v
Version 3.0.1

F:\typesc>
~~~


[TypeScript 入门指南](https://www.oschina.net/question/12_72250)  

[TypeScript 入门教程](http://www.runoob.com/w3cnote/getting-started-with-typescript.html)  

参考文档
TypeScript 中文手册:http://www.runoob.com/manual/gitbook/TypeScript/_book/  
http://code.tutsplus.com/tutorials/getting-started-with-typescript--net-28890    
https://zh.wikipedia.org/wiki/TypeScript  

----------------------
[在Angular 2/Typescript中声明全局变量的最佳方式是什么？](https://www.cnblogs.com/sybboy/p/8075146.html)  

[ts中如何声明window对象](https://www.jianshu.com/p/044791938881)  
~~~
在ts中，声明window.xx总是报错，把window写成（<any>window）就可以啦

<any>在这里的作用是强制类型转换

在window，变成全局变量了，不用require不用import
~~~

[TS引用JS模块的声明方法编写格式](https://www.jianshu.com/p/455d858b3d2a?utm_campaign)  

[笔记：Typescript 中引用全局变量](https://www.jianshu.com/p/de834f2fa309)  
var ins:any = (<any>window).ClassOutOfTS();

[typescript模块导入与全局变量踩坑日志](https://segmentfault.com/a/1190000016485619)  

[typescript之导入全局函数和类](https://blog.csdn.net/nk1212582/article/details/82193120)  
~~~
如果要导出多个对象，把它们放在顶层里导出
export class SomeType { /* ... */ }
export function someFunc() { /* ... */ }
导入时明确地列出导入的名字
import { SomeType, SomeFunc } from "./MyThings";
let x = new SomeType();
let y = someFunc();

~~~


