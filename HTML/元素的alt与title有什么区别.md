## ALT 属性

最常见用在 `` 标签上，那我们先来看下 `` 标签的 `alt` 属性。

`alt` 属性是一个必需的属性，它规定在图像无法显示时的替代文本。

假设由于下列原因用户无法查看图像，`alt` 属性可以为图像提供替代的信息：

- 网速太慢
- `src` 属性中的错误
- 浏览器禁用图像
- 用户使用的是屏幕阅读器

<img> 标签的 alt 属性指定了替代文本，用于在图像无法显示或者用户禁用图像显示时，代替图像显示在浏览器中的内容。

强烈推荐您在文档的每个图像中都使用这个属性。这样即使图像无法显示，用户还是可以看到关于丢失了什么东西的一些信息。而且对于残疾人来说，`alt` 属性通常是他们了解图像内容的唯一方式。

**注释和提示：**

注释：`alt` 属性的值是一个最多可以包含 1024 个字符的字符串，其中包括空格和标点。这个字符串必须包含在引号中。这段 `alt` 文本中可以包含对特殊字符的实体引用，但它不允许包含其他类别的标记，尤其是不允许有任何样式标签。

注释：当用户把鼠标移动到 `img` 元素上时，Internet Explorer 会显示出 `alt` 属性的值。这种行为并不正确。所有其他的浏览器正在向规范靠拢，只要当图像无法显示时，才会显示出替代文本。

提示：如果需要为图像创建工具提示，请使用 `title` 属性。

**用法和语法：**

用法：`alt` 属性只能用在 `img`、`area` 和 `input` 元素中（包括 `applet` 元素）。对于 `input` 元素，`alt` 属性意在用来替换提交按钮的图片。比如：

```
<input type="image" src="image.gif" alt="Submit" />
```

语法：
规定图像的替代文本

`alt` 文本的使用原则：

- 如果图像包含信息 - 使用 `alt` 描述图像
- 如果图像在 `a` 元素中 - 使用 `alt` 描述目标链接
- 如果图像仅供装饰 - 使用 `alt=""`

## TITLE 属性

**定义和用法：**

`title` 属性规定关于元素的额外信息。

这些信息通常会在鼠标移到元素上时显示一段工具提示文本（tooltip text）。

提示：`title` 属性常与 `form` 以及 `a` 元素一同使用，以提供关于输入格式和链接目标的信息。同时它也是 `abbr` 和 `acronym` 元素的必需属性。当然 `title` 属性是比较广泛使用的，可以用在除了`base`，`basefont`，`head`，`html`，`meta`，`param`，`script` 和 `title` 之外的所有标签。但是并不是必须的。

`title` 属性有一个很好的用途，即为链接添加描述性文字，特别是当连接本身并不是十分清楚的表达了链接的目的。这样就使得访问者知道那些链接将会带他们到什么地方，他们就不会加载一个可能完全不感兴趣的页面。另外一个潜在的应用就是为图像提供额外的说明信息，比如日期或者其他非本质的信息。

## TITLE 标签

看时间还早，我们继续来看下 `` 标签吧。

`` 元素可定义文档的标题。

浏览器会以特殊的方式来使用标题，并且通常把它放置在浏览器窗口的标题栏或状态栏上。同样，当把文档加入用户的链接列表或者收藏夹或书签列表时，标题将成为该文档链接的默认名称。

提示： `` 标签是 `` 标签中唯一要求包含的东西。