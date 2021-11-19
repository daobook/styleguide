# CSS 样式规则

## CSS 有效性

尽可能使用有效的 CSS。

使用有效的 CSS 代码，除非在处理 CSS 验证器 bug 或者是专有的语法时。

使用诸如 [W3C CSS validator](http://jigsaw.w3.org/css-validator/) 等工具验证测试。

使用有效的CSS代码是一个可衡量 CSS 代码质量的指标，可帮你找出不起作用可被删除的CSS代码，从而确保CSS的合理使用。

## `id` 与 `class` 的命名

使用有意义的或者通用的 `id` 和 `class` 名称。

用能反映出元素目的或者通用的 `id`、`class` 名称，代替那些很表象的、难懂的名称。

如果名称需要是易懂的，或不容易被修改，应该首选特定的或者能反映出元素目的的名称。

通用的名称适用于非特殊元素或与兄弟元素无区别的元素。他们常被称为“辅助元素”。

使用功能性或者通用的名称，可减少不必要的文档或者模板变化。

````{warning}
```css
/* 不推荐：无意义 */
#yee-1901 {}

/* 不推荐：表象 */
.button-green {}
.clear {}
```
````

```css
/* 推荐：具体的 */
#gallery {}
#login {}
.video {}
  
/* 推荐：通用的 */
.aux {}
.alt {}
```

## `id` 与 `class` 的命名规范


`id` 和 `class` 命名要尽可能简短，但必要的话就别怕长。

尽可能简洁地传达 `id` 或者 `class` 名称的含义。

使用简洁的 `id` 或者 `class` 名称有助于提高可读性和代码效率。

````{warning}
```css
/* 不推荐 */
#navigation {}
.atr {}
```
````

```css
/* 推荐 */
#nav {}
.author {}
```

## 选择器的类型

应当避免在 `id` 和 `class` 前添加类型选择器。

除了必要情况下（例如辅助的类），不要将元素与 `id` 或 `class` 名称结合做为选择器。

避免不必要的祖先选择器也是出于 [性能原因](http://www.stevesouders.com/blog/2009/06/18/simplifying-css-selectors/) 的考虑。

````{warning}
```css
/* 不推荐 */
ul#example {}
div.error {}
```
````
```html
/* 推荐 */
#example {}
.error {}
```

## 简写属性

尽可能使用简写的属性书写方式。

CSS提供了多种属性 [简写](http://www.w3.org/TR/CSS21/about.html#shorthand) 的方式（如 ``font`` ），即使只显式设置一个值，也应该尽可能地使用。

使用简写属性有助于提高代码效率及可读性。

````{warning}
```css
/* 不推荐 */
border-top-style: none;
font-family: palatino, georgia, serif;
font-size: 100%;
line-height: 1.6;
padding-bottom: 2em;
padding-left: 1em;
padding-right: 1em;
padding-top: 0
```
````
```css
/* 推荐 */
border-top: 0;
font: 100%/1.6 palatino, georgia, serif;
padding: 0 1em 2em;
```

## 0 与单位

省略 "0" 后的单位。

除非必需，否则 0 后不要加单位。

```css
flex: 0px; /* This flex-basis component requires a unit. */
flex: 1 1 0px; /* Not ambiguous without the unit, but needed in IE11. */
margin: 0;
padding: 0;
```

## 前导 0

省略前导 "0" 值。

在 -1 至 1 之间的值无需保留整数位的 `0`。

```css
font-size: .8em;
```

## 十六进制表示法

在可能的情况下使用3个字符的十六进制表示法。

对于可用3字符十六进制表示的颜色值，按此规则书写更短、更简洁。

````{warning}
```css
/* 不推荐 */
color: #eebbcc;
```
````

```css
/* 推荐 */
color: #ebc;
```

## 前缀选择器

加特定应用前缀（可选）

大型项目中以及嵌入在其它项目或外部网站上的代码需要给id和class添加前缀（命名空间）。使用短的、独特的标识符，并在其后跟一个破折号。

使用命名空间有助于防止命名冲突，可以让维护变得简单，例如在搜索和替换操作时。

```css
.adw-help {} /* AdWords */
#maia-note {} /* Maia */
```

## `id` 与 `class` 名称分隔符

用连字符分隔 `id` 和 `class` 名中的单词。

选择器中的词语和缩写中不要使用除了连字符以外的任何字符（包括空字符），以提高可理解性和可读性。

````{warning}
```css
/* 不推荐: 单词未分开 */
  .demoimage {}
  
/* 不推荐：使用下划线而不是连字符 */
.error_status {}
```
````
```css
/* 推荐 */
#video-id {}
.ads-sample {}
```
## Hacks

请先尝试其他的方法，避免用户代理检测以及CSS的“hacks”。

进行用户代理检测或使用特殊的CSS选择器及hacks看起来是处理样式差异的捷径。但为了实现和保持高效性以及代码的可维护性，这两种方案应该放到最后考虑。换句话说，用户代理检测和使用hacks会增大项目推进的阻力，所以从项目的长远利益考虑应尽力避免。一旦允许并无顾忌地使用用户代理检测和 hacks 便很容易滥用，最终一发而不可收。
