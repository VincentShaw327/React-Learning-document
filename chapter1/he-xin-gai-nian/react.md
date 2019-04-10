* react应用由React Dom渲染
* 一个单独的应用有一个根节点
* 用react开发web应用通常只有一个根节点,根据需求可以有任意多个根节点



```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
</head>
<body>
    <div id="root"></div>
<script crossorigin src="https://unpkg.com/react@16/umd/react.development.js"></script>
<script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js" crossorigin></script>
<script>
    const element = React.createElement(
    'h1',
    {className: 'greeting'},
    'Hello, world!'
    );
    ReactDOM.render(element, document.getElementById('root'))
</script>
</body>
</html>
```

![](/assets/import.png)

