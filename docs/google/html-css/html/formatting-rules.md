# HTML 格式规则

## 常规格式化

对每个块、列表、表格元素都另起一行，每个子元素都缩进。

每个块元素、列表元素或表格元素另起一行，而不必考虑元素的样式（因 CSS 可以改变元素的 ``display`` 属性）。

同样的，如果他们是块、列表或者表格元素的子元素，则将之缩进。

（如果你遇到列表项之间有空白的问题，可以把所有 ``li`` 元素放到一行。Linter 鼓励抛出警告而不是错误。）

:::{tab} HTML
```html
<blockquote>
  <p><em>Space</em>, the final frontier.</p>
</blockquote>
```
```html
<ul>
  <li>Moe
  <li>Larry
  <li>Curly
</ul>
```
```html
<table>
  <thead>
    <tr>
      <th scope="col">Income
      <th scope="col">Taxes
  <tbody>
    <tr>
      <td>$ 5.00
      <td>$ 4.50
</table>
```
:::

##  HTML 换行

断开长行（可选）。

虽然对 HTML 没有列数限制的建议，但如果能明显提高可读性，你可以考虑将长行包裹起来。

裹行时，每一个续行都应该在原行的基础上再缩进至少 4 个空格。

:::{tab} HTML
```html
<md-progress-circular md-mode="indeterminate" class="md-accent"
    ng-show="ctrl.loading" md-diameter="35">
</md-progress-circular>
```
```html
<md-progress-circular
    md-mode="indeterminate"
    class="md-accent"
    ng-show="ctrl.loading"
    md-diameter="35">
</md-progress-circular>
```
```html
<md-progress-circular md-mode="indeterminate"
                      class="md-accent"
                      ng-show="ctrl.loading"
                      md-diameter="35">
</md-progress-circular>
```
:::

## HTML 引号

当引用属性值时，使用双引号。

使用双引号（`""`）而不是单引号（`''`）来包裹属性值。

:::{tab} HTML
````{warning}
```html
<!-- 不推荐 -->
<a class='maia-button maia-button-secondary'>Sign in</a>
```
````

```html
<!-- 推荐 -->
<a class="maia-button maia-button-secondary">Sign in</a>
```
:::