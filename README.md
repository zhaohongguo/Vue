# Vue 总结
	vue ..
vue-cli的安装<br/>
		cnpm install --global vue-cli<br/>
		vue <br/>
		$ vue list<br/>
		vue init webpack sell<br/>
		 cd sell<br/>
		 cnpm install<br/>
		 npm run dev<br/>
Vue中用到了SVG图，我们利用icomoon帮忙处理这些SVG图<br/>
icomoon跳转处：https://icomoon.io/app/#/select
Vue 的UI框架
	iview
	mint-ui(移动端)
	Element-UI
## Vue-cli 目录结构
		|-- build                            // 项目构建(webpack)相关代码
	|   |-- build.js                     // 生产环境构建代码
	|   |-- check-version.js             // 检查node、npm等版本
	|   |-- dev-client.js                // 热重载相关
	|   |-- dev-server.js                // 构建本地服务器
	|   |-- utils.js                     // 构建工具相关
	|   |-- webpack.base.conf.js         // webpack基础配置
	|   |-- webpack.dev.conf.js          // webpack开发环境配置
	|   |-- webpack.prod.conf.js         // webpack生产环境配置
	|-- config                           // 项目开发环境配置
	|   |-- dev.env.js                   // 开发环境变量
	|   |-- index.js                     // 项目一些配置变量
	|   |-- prod.env.js                  // 生产环境变量
	|   |-- test.env.js                  // 测试环境变量
	|-- src                              // 源码目录
	|   |-- components                     // vue公共组件
	|   |-- store                          // vuex的状态管理
	|   |-- App.vue                        // 页面入口文件
	|   |-- main.js                        // 程序入口文件，加载各种公共组件
	|-- static                           // 静态文件，比如一些图片，json数据等
	|   |-- data                           // 群聊分析得到的数据用于数据可视化
	|-- .babelrc                         // ES6语法编译配置
	|-- .editorconfig                    // 定义代码格式
	|-- .gitignore                       // git上传需要忽略的文件格式
	|-- README.md                        // 项目说明
	|-- favicon.ico 
	|-- index.html                       // 入口页面
	|-- package.json                     // 项目基本信息
.
Vue中引入elementUI库时，官方文档介绍引入element的文档的时候，在main.js中
	 import 'element-ui/lib/theme-default/index.css'(这个好像是elementUI 1.0的版本写法)，但是你现在去引入这个回出现报错，你很迷茫，所以你要仔细去观察更改，现在引入这个写法如下：
	 import 'element-ui/lib/theme-chalk/index.css'
