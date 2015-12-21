#### React 元素 

是表现为html元素的js对象，没有真正的存在在浏览器中。最终显示为 div 或 section 等这样的浏览器元素。

#### JSX 

用来创建React元素和components。
如：
    <h1>Hello</h1> 是一个用 JSX 写的 React 元素。

也可以用js写成
     React.DOM.h1(null, 'Hello');

JSX 读写起来更轻松，最终上线之前必须将JSX语句转为js语句。

#### 虚拟DOM 

由 React 元素和 components 组成的 js 树形结构对象。React 将虚拟 DOM 渲染到浏览器中变成最终的用户界面。Reac会观察虚拟DOM的变化，并自动将这些变化渲染到浏览器端。 