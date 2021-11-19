# 通用样式规则

## 协议

尽可能对嵌入式资源使用 HTTPS。

始终使用 HTTPS（`https:`）来处理图像和其他媒体文件、样式表和脚本，除非相应的文件无法通过 HTTPS 获得。

:::{tab} HTML
````{warning}
```html
<!-- 不推荐 省略该协议 -->
<script src="//ajax.googleapis.com/ajax/libs/jquery/3.4.0/jquery.min.js"></script>
  
<!-- 不推荐 使用 HTTP -->
<script src="http://ajax.googleapis.com/ajax/libs/jquery/3.4.0/jquery.min.js"></script>
```
````

```html
<!-- 推荐 -->
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.0/jquery.min.js"></script>
```
:::

:::{tab} CSS
````{warning}
```css
/* 不推荐 省略该协议 */
@import '//fonts.googleapis.com/css?family=Open+Sans';

/*  不推荐 使用 HTTP  */
@import 'http://fonts.googleapis.com/css?family=Open+Sans';
```
````

```css
/* 推荐 */
@import 'https://fonts.googleapis.com/css?family=Open+Sans';
```
:::
