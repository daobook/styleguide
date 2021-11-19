# 谷歌风格指南

{guilabel}`来源`：{google}`styleguide`

```{toctree}
:maxdepth: 2
:hidden:

cpp/index
python/index
html-css/index
shell/index
typescript/index
javascript/index
```

每个主要的开源项目都有自己的风格指南：一套关于如何为该项目编写代码的惯例（有时是任意的）。风格一致时，理解一个大型代码库要容易得多。

"风格" 涵盖了很多方面，从 "对变量名使用 camelCase" 到 "绝不使用全局变量" 再到 "绝不使用异常"。项目 [google/styleguide](https://github.com/google/styleguide) 链接到谷歌的代码风格指南。如果你正在修改一个 的项目，你可能会被引导到这个页面，来查看适用于该项目的风格指南。

项目持有 [C++ 风格指南][cpp]、[C# 风格指南][csharp]、[Swift 风格指南][swift], [Objective-C 风格指南][objc]、[Java 风格指南][java], [Python 风格指南][py]、[R 风格指南][r]、[Shell 风格指南][sh]、[HTML/CSS 风格指南][htmlcss]、[JavaScript 风格指南][js]、[TypeScript 风格指南][ts]、[AngularJS 风格指南][angular]、[Common Lisp Style Guide][cl] 和 [Vimscript Style Guide][vim]。项目还包含 [cpplint][cpplint] （一个帮助遵守风格指南的工具）和 [google-c-style.el][emacs]（一个用于谷歌风格的 Emacs 设置文件）。

如果你的项目要求你创建一个新的 XML 文档格式，[XML 文档格式风格指南][xml] 可能会有帮助。除了实际的风格规则外，它还包含了关于设计你自己的与适应现有格式的建议，关于 XML 实例文件格式的建议，以及关于元素与属性的建议。

本项目中的风格指南是在 CC-By 3.0 许可下授权的。它鼓励你分享这些文件。更多细节请参见 [https://creativecommons.org/licenses/by/3.0/][ccl]。

以下的谷歌风格指南是在本项目之外的：[Go Code Review Comments][go] 和 [Effective Dart][dart]。

```{rubric} 贡献
```

除了少数例外，这些风格指南是谷歌内部风格指南的副本，以协助开发人员在谷歌拥有的和原创的开源项目中工作。风格指南的修改首先在内部风格指南中进行，最终复制到这里的版本中。**不接受外部贡献。**

拉取请求经常被关闭，没有评论。提出问题、证明技术上的变化或指出明显的错误的问题可能会得到一些参与，并在理论上可能会导致变化，但我们主要是为谷歌的内部需求进行优化。

<a rel="license" href="https://creativecommons.org/licenses/by/3.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/3.0/88x31.png" /></a>

[cpp]: https://google.github.io/styleguide/cppguide.html
[csharp]: https://google.github.io/styleguide/csharp-style.html
[objc]: https://google.github.io/styleguide/objcguide.html
[swift]: https://google.github.io/swift/
[java]: https://google.github.io/styleguide/javaguide.html
[py]: https://google.github.io/styleguide/pyguide.html
[r]: https://google.github.io/styleguide/Rguide.html
[sh]: https://google.github.io/styleguide/shellguide.html
[htmlcss]: https://google.github.io/styleguide/htmlcssguide.html
[js]: https://google.github.io/styleguide/jsguide.html
[ts]: https://google.github.io/styleguide/tsguide.html
[angular]: https://google.github.io/styleguide/angularjs-google-style.html
[cl]: https://google.github.io/styleguide/lispguide.xml
[vim]: https://google.github.io/styleguide/vimscriptguide.xml
[cpplint]: https://github.com/google/styleguide/tree/gh-pages/cpplint
[emacs]: https://raw.githubusercontent.com/google/styleguide/gh-pages/google-c-style.el
[xml]: https://google.github.io/styleguide/xmlstyle.html
[go]: https://golang.org/wiki/CodeReviewComments
[dart]: https://www.dartlang.org/guides/language/effective-dart
[ccl]: https://creativecommons.org/licenses/by/3.0/

