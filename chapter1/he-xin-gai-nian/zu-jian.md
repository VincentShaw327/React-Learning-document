* 组件的优势

  * 代码复用,减少工作量

  * 更有利于模块化开发和维护

  * 便于设计和团队协作开发

* 创建组件的方式

  1. 纯函数组件

  2. ES6语法创建

  3. ES5creatClass创建_\(从react16.0版本开始已经剔除了\)_

* 组件的引用

---

## 创建组件的方式:

### 1.纯函数组件

```js
import React from 'react';

function pureComponent(props){
    return <h1>Hello, {props.name}</h1>;
}
```

### 2.ES6语法创建

```js
class Welcome extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}
```

## 组件的引用:

* 组件以标签方式引用
* 标签中的属性将以props方式传递

> 注:标签名第一个字母必须是大写

```js
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}
ReactDOM.render(
  <Welcome name="Sara" />,
  document.getElementById('root')
);
```

## 组件的嵌套:

* 组件可以无限的任意嵌套
* * 嵌套的子组件在props.children中传递

## 

## 一个React组件包含的内容:

* dom标签
* 数据
* 样式



