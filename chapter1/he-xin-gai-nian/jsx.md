##  什么是JSX? {#什么是jsx}

### 一句话介绍: {#一句话介绍}

* JSX是react特有的一种模板语法,他可以将JS脚本、CSS样式、和HTML标签一起混写
* jsx不能直接在网页显示，需要通过babel转译成标准语法才可以被浏览器解析

---

## JSX写法案例： {#jsx写法案例}

### 1.嵌入表达式 {#1嵌入表达式}

```js
let name='world'

const element =<h1>Hello, {name}</h1>;//大括号内可嵌入任何合法JS表达式
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



