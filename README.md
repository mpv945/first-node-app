# first-node-app
我的node项目

# node项目运行
  1. 参考hello_world_flutter 配置nodejs
  2. 新建firstNode.js ;点击debug生成launch.json。 运行就能输出测试的消息打印
  3. Express是一个非常流行的应用程序框架，用于构建和运行Node.js应用程序。npm install -g express-generator
  4. 在当前工作目录执行express first-node-app ；会覆盖git下载的first-node-app项目（这将创建一个myExpressApp使用应用程序内容调用的新文件夹。）
  5. 安装所有应用程序的依赖项（再次作为npm模块提供）cd first-node-app 然后 npm install；最后运行npm start（默认端口3000）
  6.如果需要debug的web项目Express，需要修改launch.json 修改成"program": "${workspaceFolder}\\bin\\www"

# 本地安装
  ## 1. 将安装包放在 ./node_modules 下（运行 npm 命令时所在的目录），如果没有 node_modules 目录，会在当前执行 npm 命令的目录下生成 node_modules 目录。 2. 可以通过 require() 来引入本地安装的包。
# 全局安装
  ## 1. 将安装包放在 /usr/local 下或者你 node 的安装目录。2. 可以直接在命令行里使用。
  注意：如果你希望具备两者功能，则需要在两个地方安装它或使用 npm link。
# node基本知识学习（api说明：http://nodejs.cn/api/assert.html和http://www.runoob.com/nodejs/nodejs-tutorial.html）；其他；例如Webpack:https://www.jianshu.com/p/42e11515c10f;使用技巧：http://blog.fens.me/series-nodejs/
## 项目目录下的package.json包含项目基本信息和依赖信息，类似java的pom文件
1. node --version 查看node版本；npm -v 查看npm 版本,检查npm 是否正确安装。
2. npm init 初始化项目，其实就是创建一个package.json文件。需要根据你自己的情况输入。在最后输入 "yes" 后会生成 package.json 文件
3. npm adduser （在 npm 资源库中注册用户）输入提示的信息。登陆npm；接下来我们就用以下命令来发布模块：npm publish https://blog.csdn.net/qq_24956515/article/details/80514262
4. npm install cnpm -g --registry=https://registry.npm.taobao.org 安装cnpm (国内淘宝镜像源)；这样就可以使用 5. cnpm 命令来安装模块了cnpm install [name]
6. npm install 模块名 安装模块；npm install -g express 全局安装express模块
7. npm list 列出已安装模块，可以指定模块，查看模块的版本信息，加-g查看全局的 ；npm show express 显示express模块详情
8. npm update 升级当前目录下的项目的所有模块,可以指定模块进行更新；npm update -g express 升级全局安装的express模块
  注意：update时，最好在某个模块内运行，以免更新到其他不想更新的模块。
9. npm uninstall express 删除指定的模块；var http = require("http")  node引入模块使用require
10. npm rm|r|uninstall |un <name>：删除模块，但是不会删除package.json文件dependencies选项中对应的依赖配置
   xxx 卸载xxx。多个依赖可用空格分割。xxx -D 卸载xxx，并将依赖信息从package.json中的devDependencies中清除。
11. npm search jquery （npm search 搜索（快捷方式：find, s）
12. npm root 查看依赖安装路径（也就是node_modules的路径）-g 查看全局安装路径。
13. npm view 查看模块的注册信息。列出jquery的所有版本， 如：npm view jquery versions；列出gulp的所有依赖， 如：npm view gulp dependencies
14. npm <script>：有npm start [<name>]，npm stop [<name>]，npm test [<name>] 等，该些脚本定义在package.json文件scripts中。
15. Package.json 属性说明：http://www.runoob.com/nodejs/nodejs-npm.html
