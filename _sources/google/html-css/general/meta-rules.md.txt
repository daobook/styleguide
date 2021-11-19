# 通用文档级元数据规则

## 编码

使用 UTF-8 无 BOM 编码。

请确保你的编辑器使用 UTF-8 作为字符编码，没有字节顺序标记。

在 HTML 模板和文档中使用 ``<meta charset="utf-8">`` 指定编码。不需要为样式表指定编码，它默认是 UTF-8。

（想了解更多关于应该何时并如何指定编码，请查看 [处理 HTML 和 CSS 中的字符编码](https://www.w3.org/International/tutorials/tutorial-char-enc/)）

## 注释

在可能的情况下，根据需要对代码进行解释。

使用注释来解释代码。它涵盖了什么，它的目的是什么，为什么使用或偏爱各自的解决方案？

（这一条是可选的，没必要为每个文件写上详细的注释，会增重 HTML/CSS 的代码，主要取决于项目的复杂度。）

## 行动事项

用 `TODO` 来标记待办事宜和行动事项。

只用关键字 `TODO` 来高亮待办事宜，而不是其他常见的格式如 `@@`。

在括号里添加联系方式（姓名或邮箱），格式为 `TODO（联系方式）`。

在冒号后面添加处理内容，格式为 `TODO: action item`。

:::{tab} HTML
```html
{# TODO(john.doe): revisit centering #}
<center>Test</center>
```

```html
<!-- TODO: 移除可选的标签 -->
<ul>
  <li>Apples</li>
  <li>Oranges</li>
</ul>
```
:::