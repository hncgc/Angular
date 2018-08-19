# Angular
Angular

https://github.com/Mavlarn/Angular2-tutorial-Chinese


Angular2框架

[Angular2教程](https://www.w3cschool.cn/angular2/)  

[在手机上查看文档](https://m.w3cschool.cn/angular2/)  


webstorm
===

[webstorm官网中文破解版](https://blog.csdn.net/vchen_hao/article/details/77248053)  

[Webstorm 超实用教程](https://www.jianshu.com/p/4ce97b360c13)  
~~~
安装过程（包含输入注册码永久使用）
要填的内容：http://idea.imsxm.com/，复制进去即可。
~~~

[使用WebStorm开发TypeScript的设置](https://blog.csdn.net/xiaozhi_2016/article/details/64922203)  

[使用Visual Studio Code搭建TypeScript开发环境](https://www.cnblogs.com/sunjie9606/p/5945540.html)  
安装Visual Studio Code

[ALM:TypeScript / JavaScript 的下一代 IDE](https://linux.cn/article-7406-1.html)  
~~~
ALM 安装很简单
npm install alm -g

F:\typesc>npm install alm -g
[ .................] \ fetchMetadata: sill resolveWithNewModule cookie-signature@1.0.6 checking installable status

F:\typesc>npm install alm -g
npm ERR! Unexpected end of JSON input while parsing near '...","version":"3.0.0","'

npm ERR! A complete log of this run can be found in:
npm ERR!     C:\Users\HP\AppData\Roaming\npm-cache\_logs\2018-08-12T03_50_50_985Z-debug.log

F:\typesc>
~~~

[Webstorm 超实用教程](https://www.jianshu.com/p/4ce97b360c13)  
~~~
一、下载安装包  
二、安装过程（包含输入注册码永久使用）  
1. 配置 Webstorm 安装项  
选择 64 位，防止桌面 Webstorm 快捷方式打不开  
2. 是否导入 Webstorm 配置信息  
3. 激活 Webstorm  
要填的内容：http://idea.imsxm.com/，复制进去即可  
4. 设置 Webstorm 工具的主题和风格  
三、使用心得  
File -> settings -> Editor -> colors&fonts -> scheme name.  
觉得 Default Darcula 这两款主题还可以  
2. 换成自己熟悉编辑器的快键键：如 Eclipse 的快捷键 + 自定义快捷键组合  
3. 取消勾选安全保存时间  
4. 集成 Eslint  
集成 Eslint 的前提是你的项目里使用了 Eslint  
5. 集成 Git  
6. 常用开发工具窗口  
7. 配置 Less 自动转译 CSS  
8. Webstorm 安装 Editorconfig 插件  
9. 文件类型设置 —— File Types  
使用微信开发工具开发小程序  
使用 File Types 可以将 .wxml 和 .wxss 文件类型添加到 Webstorm 中。  
在 Cascading Style Sheet 下添加 *.wxss 类型，使用 css 语法高亮；  
在 HTML 下添加 *.wxml 类型，使用 html 语法高亮。  
注意：前面的 * 号不能忘记  
10. Webstorm 2017.2 版本使用搜狗输入法卡顿问题  
11. Webstorm 弹出 Npm 对话框  
12. 快捷键 —— 最常用的快捷键最佳应在 10 个以内  
四、优化 Webstorm  
1. 调整 webstorm 内存  
webstorm 安装目录 > bin > WebStorm.exe.vmoptions。文本编辑器打开，修改第二行和第三行内容。  

第二行：-Xms526m  

第三行：-Xmx1024m  
2. 把不必要索引的文件进行排除  
选择项目 > 右键 > Mark Directory As > Excluded。操作完成后会发现项目“消失了”。  
3. 关闭 node_modules 校验  
4. 取消勾选不常用的插件  
webstorm 中可以集成很多插件，这些插件也会影响运行速度，有的插件你可能压根都没听过，更不会使用，可以取消勾选。  
~~~

F:\typesc>npm install less -g  
C:\Users\HP\AppData\Roaming\npm\lessc -> C:\Users\HP\AppData\Roaming\npm\node_modules\less\bin\lessc  
+ less@3.8.1  
added 59 packages from 122 contributors in 25.969s  

F:\typesc>  


[Less.js 中文文档](http://www.css88.com/doc/less/)  
[学习Less-看这篇就够了](https://segmentfault.com/a/1190000012360995)  

[使用WebStorm开发TypeScript的设置](https://blog.csdn.net/xiaozhi_2016/article/details/64922203)  
~~~
1. 打开Webstorm，新建一个空白项目，命名为TypeScriptProgram
2.在Webstorm中右击项目名，选择new->tsconfig.json File，创建tsconfig.json文件
3.打开Webstorm,为TypeScript文件更改编译设置，File->Settings->File Watchers->TypeScript，这里我们需要选择TypeScript，但是

File Watchers下默认是不存在的。需要点击右侧“+”号，选择<custom>,弹出 New Watcher，设置好圈红线的部分，点击ok。勾
TypeScript
选“TypeScript”，点击ok。

Name: TypeScript
File type: TypeScript
Program:    C:\Users\HP\AppData\Roaming\npm\tsc.cmd
Arguments:   --sourcemap --target "ES5"

Working directory:  $FileDir$

7.设置typescript自动编译，勾选下图圈红线的位置

F:\typesc\test\test.ts

/**
 * Created by Cheng GongChun on 2018-8-12
 */
interface Person {
    firstName: string
    lastName: string
}

class User {
    fullName : string
    constructor(firstName: string, lastName:string) {
        this.fullName = firstName + " " + lastName
    }
}

function welcome(person : Person) {
    return person.firstName + " " + person.lastName
}

let user =  { firstName : "Cheng", lastName : "Gongchun"}
console.log(welcome(user))

F:\typesc\test\test.js

var User = (function () {
    function User(firstName, lastName) {
        this.fullName = firstName + " " + lastName;
    }
    return User;
}());
function welcome(person) {
    return person.firstName + " " + person.lastName;
}
var user = { firstName: "Cheng", lastName: "Gongchun" };
console.log(welcome(user));
//# sourceMappingURL=test.js.map

~~~

https://www.tslang.cn/docs/handbook/typescript-in-5-minutes.html   

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

