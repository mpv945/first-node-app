# first-node-app
我的node项目

# node项目运行
  1. 参考hello_world_flutter 配置nodejs
  2. 新建firstNode.js ;点击debug生成launch.json。 运行就能输出测试的消息打印
  3. Express是一个非常流行的应用程序框架，用于构建和运行Node.js应用程序。npm install -g express-generator
  4. 在当前工作目录执行express first-node-app ；会覆盖git下载的first-node-app项目（这将创建一个myExpressApp使用应用程序内容调用的新文件夹。）
  5. 安装所有应用程序的依赖项（再次作为npm模块提供）cd first-node-app 然后 npm install；最后运行npm start（默认端口3000）
  6.如果需要debug的web项目Express，需要修改launch.json 修改成"program": "${workspaceFolder}\\bin\\www"
