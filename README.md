# learning-react
step by step learning react


+ React不是完整的mvc框架？不太认可mvc的开发模式
+ React不是一个新的模板语言，JSX只是一个表象，没有JSX的React也能工作。

遇到的坑：
有的文档写的使用 JSX的地方加上text/jsx，如：
    <script type="text/jsx"></script>
    <script src="build/react.js"></script>
    <script src="build/JSXTransformer.js"></script> <!-- 将JSX语法转为js语法 -->

而有些文档又写的需要加上text/babel，
    <script type="text/babel"></script>
    <script src="build/react.js"></script>
    <script src="build/react-dom.js"></script> <!-- 提供与 DOM 相关的功能 -->
    <script src="build/browser.min.js"></script> <!-- 将JSX语法转为js语法 -->

最新版的都是加上text/babel，因为改成了0.14版本后，"text/jsx"修改为"text/babel"解析,JSXTransformer.js官方也不再发布了, 具体见：http://www.tuicool.com/articles/NFvYfeB


# links:
+ [react-native-lesson](https://github.com/vczero/react-native-lesson)
+ [一看就懂的ReactJs入门教程（精华版）](http://www.cocoachina.com/webapp/20150721/12692.html)
+ [React 入门] (http://segmentfault.com/a/1190000002759878]
+ [React Native通信机制详解] (http://blog.cnbang.net/tech/2698/]
+ [React中文文档]  (http://reactjs.cn/react/docs/getting-started.html]