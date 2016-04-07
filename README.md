# learning-react
step by step learning react


+ React不是完整的mvc框架？不太认可mvc的开发模式
+ React不是一个新的模板语言，JSX只是一个表象，没有JSX的React也能工作。

遇到的坑：
有的文档写的使用 JSX的地方加上text/jsx，如：

    <script type="text/jsx"></script>
    <script src="build/react.js"></script>
    <script src="build/JSXTransformer.js"></script> <!-- 将JSX语法转为js语法 -->

而有些文档又写的需要加上text/babel

    <script type="text/babel"></script>
    <script src="build/react.js"></script>
    <script src="build/react-dom.js"></script> <!-- 提供与 DOM 相关的功能 -->
    <script src="build/browser.min.js"></script> <!-- 将JSX语法转为js语法 -->

最新版的都是加上text/babel，因为改成了0.14版本后，"text/jsx"修改为"text/babel"解析,JSXTransformer.js官方也不再发布了, 具体见：http://www.tuicool.com/articles/NFvYfeB

# 通过 npm 使用 React
建议在 React 中使用 CommonJS 模块系统，比如 browserify 或 webpack，本教程使用 webpack。

第一步、安装全局包

	npm install babel -g
	npm install webpack -g
	npm install webpack-dev-server -g

第二步、创建根目录

创建一个根目录，目录名：reactTest，再使用 npm init 初始化，生成 package.json 文件

第三步、添加越来包及插件

因为我们要使用 React, 所以我们需要先安装它，--save 命令用于将包添加至 package.json 文件。

	npm install react --save
	npm install react-dom --save

同时也要安装一些 babel 插件

	npm install babel-core
	npm install babel-loader
	npm install babel-preset-react
	npm install babel-preset-es2015


注：npm install 装不上的时候可以：npm --registry=http://r.cnpmjs.org install



# links:
+ [React 安装](http://www.runoob.com/react/react-install.html)
+ [React 入门实例教程](http://www.ruanyifeng.com/blog/2015/03/react.html)
+					(http://hao.jser.com/archive/8466/)
+ [react-native-lesson](https://github.com/vczero/react-native-lesson)
+ [一看就懂的ReactJs入门教程（精华版）](http://www.cocoachina.com/webapp/20150721/12692.html)
+ [React 入门](http://segmentfault.com/a/1190000002759878)
+ [React Native通信机制详解](http://blog.cnbang.net/tech/2698/)
+ [React中文文档](http://reactjs.cn/react/docs/getting-started.html)
+ [React 入门教程]http://i5ting.github.io/reactjs-getting-start/#
+ [React 入门教程]https://hulufei.gitbooks.io/react-tutorial/content/introduction.html

+ [React 入门教程]http://www.phperz.com/article/15/0712/140539.html
+ [使用React、Node.js、MongoDB、Socket.IO开发一个角色投票应用](http://www.kancloud.cn/kancloud/create-voting-app/63977)