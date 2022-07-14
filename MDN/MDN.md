## script 标签

- async

```markdown
对于普通脚本，如果存在 `async` 属性，那么普通脚本会被并行请求，并尽快解析和执行。
对于[模块脚本](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Guide/Modules)，如果存在 `async` 属性，那么脚本及其所有依赖都会在延缓队列中执行，因此它们会被并行请求，并尽快解析和执行。
该属性能够消除解析阻塞的 JavaScript。解析阻塞的 JavaScript 会导致浏览器必须加载并且执行脚本，之后才能继续解析。`defer` 在这一点上也有类似的作用。
```

- defer

```markdown
这个布尔属性被设定用来通知浏览器该脚本将在文档完成解析后，触发 `DOMContentLoaded (en-US)` 事件前执行。

有 `defer` 属性的脚本会阻止 `DOMContentLoaded` 事件，直到脚本被加载并且解析完成。
```

- type

```markdown
该属性定义 script 元素包含或src引用的脚本语言。属性的值为MIME类型; 支持的MIME类型包括text/javascript, text/ecmascript, application/javascript, 和application/ecmascript。如果没有定义这个属性，脚本会被视作 JavaScript。
如果MIME类型不是 JavaScript 类型（上述支持的类型），则该元素所包含的内容会被当作数据块而不会被浏览器执行。
如果 type 属性为module，代码会被当作 JavaScript 模块
```

