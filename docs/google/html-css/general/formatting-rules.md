# 通用排版规则

## 缩进

每次缩进使用两个空格。

不使用 TAB 键或者混合使用 TAB 键和空格进行缩进。

:::{tab} HTML
```html
<ul>
  <li>Fantastic
  <li>Great
</ul>
```
:::

:::{tab} CSS
```css
.example {
  color: blue;
}
```
:::

## 大小写

只使用小写字母。

所有的代码都使用小写字母：适用于 HTML 元素、属性、属性值（除了 `text/CDATA`）、CSS 选择器、属性名以及属性值（字符串除外）。

:::{tab} HTML
````{warning}
```html
<!-- 不推荐 -->
<A HREF="/">Home</A>
```
````
```html
<!-- 推荐 -->
<img src="google.png" alt="Google">
```
:::

:::{tab} CSS
````{warning}
```css
/* 不推荐 */
color: #E5E5E5;
```
````

```css
/* 推荐 */
color: #e5e5e5;
```
:::

## 尾部的空格

删除尾部的空格。

尾部的空白是不必要的，会使差异复杂化。

:::{tab} HTML
````{warning}
```html
<!-- 不推荐 -->
<p>What?_ 
```
````
```html
<!-- 推荐 -->
<p>Yes please.
```
:::