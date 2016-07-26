module-dev-example
---
该项目是一个模块开发的演示项目, 可以直接下载该项目作为开发模版, 修改对应的基础文件即可

快速开始
===
1.下载该项目到某个目录

2.修改文件
  - package.json(根目录下的, 修改描述和模块名)
  - README.md(写基础的模块信息, 例: 详细描述, 如何快速开始, 版本迭代)

3.进入`根`目录命令行输入 
  - `cnpm i`(安装服务器的基础包和模块开发的基础包)
  - `fis3 server start`(启动fis服务器)
  - `fis3 release -wclL` (编译项目, 并检查代码是否规范)
  - `npm test` or `karma start karma.config.js`(启动单元测试)  

4.大体目录结构
  - example(演示)
  - lib(模块文件放这里)
  - test(单元测试)
  - fis-conf.js(用于支持模块化开发, 搭建演示demo)
  - package.json(用于保存该模块所引用的其他模块)

test
===
如果你想查看单元测试结果, 那么你可以在根目录输入以下命令
测试脚本在test文件夹, 请根据自己的模块编写测试用例

参考 [jasmine](http://jasmine.github.io/2.4/introduction.html)

```

$ npm test

// or

$ karma start karma.config.js

```

ChangeLog
---
0.0.2
 - 去掉dev任务只留test任务
 - 服务器用fis3 server
 - 去掉gulpfile.js