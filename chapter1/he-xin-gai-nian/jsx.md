## 什么是JSX? {#什么是jsx}

### 一句话介绍: {#一句话介绍}

* JSX是react特有的一种模板语法,他可以将JS脚本、CSS样式、和HTML标签一起混写
* jsx不能直接在网页显示，需要通过babel转译成标准语法才可以被浏览器解析

---

## JSX写法案例： {#jsx写法案例}

* 嵌入表达式
* 将JSX作为表达式引用
* JSX属性值-字符串
* JSX属性值-表达式
* 闭合标签
* 多层嵌套

### 1.嵌入表达式 {#1嵌入表达式}

```js
let name='world'

const element =<h1>Hello, {name}</h1>;
```

#### JavaScript有以下表达式类型： {#javascript有以下表达式类型}

* 算数: 得出一个数字, 例如 3.14159. \(通常使用 arithmetic operators.\)
* 字符串: 得出一个字符串, 例如, "Fred" 或 "234". \(通常使用 string operators.\)
* 逻辑值: 得出true或者false. \(经常涉及到 logical operators.\)
* 基本表达式: javascript中基本的关键字和一般表达式。
* 左值表达式: 分配给左值。 更多关于JS表达式，请参考

### 2.将JSX作为表达式引用 {#2将jsx作为表达式引用}

```
let name='world'

const element =<h1>Hello, {name}</h1>;

const showJSX=<div>{element}</div>;
```

## 3.JSX属性值-字符串 {#3jsx属性值-字符串}

```
let name='world'

const element =<h1>Hello, {name}</h1>;

const showJSX =<div className="show">{element}</div>;
```

## 4.JSX属性值-表达式 {#4jsx属性值-表达式}

```
let name='world'

const element =<h1>Hello, {name}</h1>;

const showJSX =<div className={{show:true,hidden:false}>{element}</div>;
```

## 5.闭合标签

假如一个标签里面没有内容，你可以使用"/&gt;"来闭合标签，就像 XML 语法一样：

```
const element = <img src={user.avatarUrl} />;
```

## 6.多层嵌套

```
const element = (
  <div>
    <h1>Hello!</h1>
    <h2>Good to see you here.</h2>
  </div>
);
```

## 7.JSX对象

> **Babel 会把 JSX 转译成一个名为**`React.createElement()`**函数调用**
>
> _**以下两种写法完全等效!!**_

```
const element = (
  <h1 className="greeting">
    Hello, world!
  </h1>
);
```

```js
const element = React.createElement(
  'h1',
  {className: 'greeting'},
  'Hello, world!'
);
```



