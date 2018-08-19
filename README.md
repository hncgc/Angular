# Angular
Angular

https://github.com/Mavlarn/Angular2-tutorial-Chinese


Angular2框架

Angular2教程
https://www.w3cschool.cn/angular2/

在手机上查看文档：https://m.w3cschool.cn/angular2/





TypeScript

https://github.com/Microsoft/TypeScript/wiki
https://www.tslang.cn/

TypeScript 从入门到放弃
https://www.jianshu.com/p/c5005fad4274


TypeScript中文网 
https://www.tslang.cn/

Typescript简介和安装
https://blog.csdn.net/xcg132566/article/details/76098753

安装简单总结：安装node-->npm安装typescript的compiler-->配置IDE-->编码运行

TypeScript 安装
https://blog.csdn.net/adelais__/article/details/79181474
TypeScript官网：http://www.typescriptlang.org/index.html
安装Node.js，官网：https://nodejs.org/en/，LTS和Current都行，建议LTS；下载完成双击打开就可以，如下图
下载node-v8.11.3-x64.msi

添加到环境变量里面，C:\Program Files\nodejss 安装时已自动添加

C:\Users\HP>node -v
v8.11.3
C:\Users\HP>npm -v
5.6.0

使用npm安装typescript，在命令提示符界面输入命令npm install -g typescript安装typescript和命令tsc -v查看其版本号

C:\Users\HP>npm install -g typescript
npm ERR! Unexpected end of JSON input while parsing near '...ake":"latest","merge2'

npm ERR! A complete log of this run can be found in:
npm ERR!     C:\Users\HP\AppData\Roaming\npm-cache\_logs\2018-08-11T15_37_19_183Z-debug.log

C:\Users\HP>

Unexpected end of JSON input while parsing near错误解决办法
https://blog.csdn.net/m0_37836194/article/details/79107785

npm install出现”Unexpected end of JSON input while parsing near”的错误。

运行  npm cache clean --force。

C:\Users\HP>npm cache clean --force
npm WARN using --force I sure hope you know what you are doing.

C:\Users\HP>

C:\Users\HP>npm install -g typescript
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



code EINTEGRITY，npm安装时候报错
https://www.cnblogs.com/zhaixr/p/7307718.html

解决方法：

1.如果有package-lock.json文件，就删掉

2.管理员权限进入cmd

3.执行npm cache clean --force

4.之后再npm install

有时候网不好也会出现问题，多试几次。

C:\Users\HP>npm install -g typescript
[       ...........] - extract:typescript: verb lock using C:\Users\HP\AppData\Roaming\npm-cache\_locks\staging-44c5448c6858e3d9.lock for C:\Users\HP\AppDat

npm install 提示 ERR! code EINTEGRITY
https://blog.csdn.net/Mr_rain/article/details/74551497

先运行 
npm i -g npm
再运行 
grep -ir “sha1-W/Rejkm6QYnhfUgnid/RW9FAt7Y= integrity chexxxxxxxxxxxxxxxxxxxxxxxxxxxxDUqxF47jfwOgvK2UM16SEXk=” ~/.npm

C:\Users\HP>npm i -g npm
C:\Users\HP\AppData\Roaming\npm\npx -> C:\Users\HP\AppData\Roaming\npm\node_modules\npm\bin\npx-cli.js
C:\Users\HP\AppData\Roaming\npm\npm -> C:\Users\HP\AppData\Roaming\npm\node_modules\npm\bin\npm-cli.js
+ npm@6.3.0
added 396 packages in 111.982s

C:\Users\HP>grep -ir "sha1-W/Rejkm6QYnhfUgnid/RW9FAt7Y= integrity chexxxxxxxxxxxxxxxxxxxxxxxxxxxxDUqxF47jfwOgvK2UM16SEXk=" ~/.npm
'grep' 不是内部或外部命令，也不是可运行的程序
或批处理文件。

C:\Users\HP>npm install -g typescript
C:\Users\HP\AppData\Roaming\npm\tsc -> C:\Users\HP\AppData\Roaming\npm\node_modules\typescript\bin\tsc
C:\Users\HP\AppData\Roaming\npm\tsserver -> C:\Users\HP\AppData\Roaming\npm\node_modules\typescript\bin\tsserver
+ typescript@3.0.1
added 1 package from 1 contributor in 377.309s

C:\Users\HP>tsc -v
Version 3.0.1

C:\Users\HP>

资料：https://github.com/npm/npm/issues/16861

npm ERR! code EINTEGRITY问题解决方案
https://blog.csdn.net/u011218378/article/details/78250103

搭建TypeScript开发环境
https://blog.csdn.net/diligentkong/article/details/74781539

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


webstorm
===

webstorm官网中文破解版
https://blog.csdn.net/vchen_hao/article/details/77248053

Webstorm 超实用教程
https://www.jianshu.com/p/4ce97b360c13
安装过程（包含输入注册码永久使用）
要填的内容：http://idea.imsxm.com/，复制进去即可。

使用WebStorm开发TypeScript的设置
https://blog.csdn.net/xiaozhi_2016/article/details/64922203

使用Visual Studio Code搭建TypeScript开发环境
https://www.cnblogs.com/sunjie9606/p/5945540.html
安装Visual Studio Code

ALM:TypeScript / JavaScript 的下一代 IDE
https://linux.cn/article-7406-1.html

ALM 安装很简单
npm install alm -g

F:\typesc>npm install alm -g
[ .................] \ fetchMetadata: sill resolveWithNewModule cookie-signature@1.0.6 checking installable status

F:\typesc>npm install alm -g
npm ERR! Unexpected end of JSON input while parsing near '...","version":"3.0.0","'

npm ERR! A complete log of this run can be found in:
npm ERR!     C:\Users\HP\AppData\Roaming\npm-cache\_logs\2018-08-12T03_50_50_985Z-debug.log

F:\typesc>


然后在终端运行 alm 即可。

F:\typesc>node -v
v8.11.3

F:\typesc>npm -v
6.3.0

F:\typesc>tsc -v
Version 3.0.1

F:\typesc>

Webstorm 超实用教程
https://www.jianshu.com/p/4ce97b360c13
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



F:\typesc>npm install less -g
C:\Users\HP\AppData\Roaming\npm\lessc -> C:\Users\HP\AppData\Roaming\npm\node_modules\less\bin\lessc
+ less@3.8.1
added 59 packages from 122 contributors in 25.969s

F:\typesc>


Less.js 中文文档
http://www.css88.com/doc/less/
学习Less-看这篇就够了
https://segmentfault.com/a/1190000012360995

TypeScript 入门指南
https://www.oschina.net/question/12_72250

使用WebStorm开发TypeScript的设置
https://blog.csdn.net/xiaozhi_2016/article/details/64922203
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

https://www.tslang.cn/docs/handbook/typescript-in-5-minutes.html



