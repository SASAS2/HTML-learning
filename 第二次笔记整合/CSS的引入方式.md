## CSS的引入方式

### 1. 外部样式表

使用 `<link>` 标签引入外部样式表。`rel` 属性表示关系，`href` 属性指定样式表文件的路径。

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS 引入方法</title>
    <!-- link引入外部样式表；rel:关系，样式表 -->
    <link rel="stylesheet" href="./1.css">
</head>
<body>
    <p>这是粉色的p标签</p>
</body>
</html>
```

### 2. 内部样式表

在 `<head>` 标签内使用 `<style>` 标签定义样式。

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS 引入方法</title>
    <style>
        p {
            color: pink;
        }
    </style>
</head>
<body>
    <p>这是粉色的p标签</p>
</body>
</html>
```

### 3. 行内样式

直接在HTML标签内使用 `style` 属性定义样式。

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS 引入方法</title>
</head>
<body>
    <p style="color: pink;">这是粉色的p标签</p>
    <div style="color: aqua; font-size: 50px;">这是青色的div标签</div>
</body>
</html>
```

希望这些内容对你有帮助！如果你有任何问题或需要进一步的解释，请随时告诉我。

源: 与 Copilot 的对话， 2024/11/20
(1) github.com. https://github.com/bgoonz/UsefulResourceRepo2.0/tree/077e4c1ea7981abd049f91dd5084f66c968806c6/MY_REPOS%2FProject-Showcase%2Fjsanimate-master%2Fjsanimate-master%2FREADME.md.