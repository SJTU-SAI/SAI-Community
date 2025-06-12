# Template Markdown in this Website

本网站采用**mkdocs**[^1]框架，省去了网站搭建复杂的流程，利用自动化的github actions和HTML渲染搭建静态网页。用户只需要提交markdown格式的内容即可。

下文是对markdown格式的快速梳理，包括**在mkdocs中自定义的高级语法**和**markdown写作规范**，供各位开发者参考。

## Markdown基本语法快速指南

### Headers:

```markdown
# Header 1
## Header 2
...
###### Header 6
```

### Fonts

```markdown
**这是加粗字体**
*这是斜线*
***这是加粗的斜线字体***
```

对于有颜色的字体，可以使用：
```html
<!-- 不同大小和颜色的字体 -->
<span style="font-size:24px; color:#015c43;font-family: 'Microsoft YaHei', '微软雅黑', sans-serif; font-weight: bold;">大号深绿色字体</span>

<span style="font-size:16px; color:#e67e22;">中号橙色字体</span>这是正常字体。

<!-- 居中显示 -->
<p align="center">
  <span style="font-size:20px; color:#023c31;">居中深绿色字体</span>
</p>

<!-- 不居中显示 -->
<span style="font-size:18px; color:#c0392b;">左对齐红色字体</span>
```

!!! note "A simple demo"
    <!-- 不同大小和颜色的字体 -->
    <span style="font-size:24px; color:#015c43;font-family: 'Microsoft YaHei', '微软雅黑', sans-serif; font-weight: bold;">大号深绿色字体</span>

    <span style="font-size:16px; color:#e67e22;">中号橙色字体</span>这是正常字体。

    <!-- 居中显示 -->
    <p align="center">
    <span style="font-size:20px; color:#023c31;">居中深绿色字体</span>
    </p>

    <!-- 不居中显示 -->
    <span style="font-size:18px; color:#c0392b;">左对齐红色字体</span>

## Advanced Settings

除了基础的 Markdown 语法，MkDocs 还支持一些**高级扩展语法**，让你的文档更加丰富和强大。

### Admonitions

你可以在自己的文档中创建高亮文本框。

??? abstract "Lists"
    - note: fontawesome/solid/note-sticky
    - abstract: fontawesome/solid/book
    - info: fontawesome/solid/circle-info
    - tip: fontawesome/solid/bullhorn
    - success: fontawesome/solid/check
    - question: fontawesome/solid/circle-question
    - warning: fontawesome/solid/triangle-exclamation
    - failure: fontawesome/solid/bomb
    - danger: fontawesome/solid/skull
    - bug: fontawesome/solid/robot
    - example: fontawesome/solid/flask
    - quote: fontawesome/solid/quote-left

```markdown
!!! Note "A simple demo"
    ??? note "this is a note"
        This is a note
    ??? abstract "this is an abstract"
        This is an abstract
    ??? info "this is an info"
        This is an info
    ??? tip "this is a tip"
        This is a tip
    ??? success "this is a success"
        This is a success
    ??? question "this is a question"
        This is a question
    ??? warning "this is a warning"
        This is a warning
    ??? failure "this is a failure"
        This is a failure
    ??? danger "this is a danger"
        This is a danger
    ??? bug "this is a bug"
        This is a bug
    ??? example "this is an example"
        This is an example
    ??? quote "this is a quote"
        This is a quote
```

!!! Note "A simple demo"
    ??? note "this is a note"
        This is a note
    ??? abstract "this is an abstract"
        This is an abstract
    ??? info "this is an info"
        This is an info
    ??? tip "this is a tip"
        This is a tip
    ??? success "this is a success"
        This is a success
    ??? question "this is a question"
        This is a question
    ??? warning "this is a warning"
        This is a warning
    ??? failure "this is a failure"
        This is a failure
    ??? danger "this is a danger"
        This is a danger
    ??? bug "this is a bug"
        This is a bug
    ??? example "this is an example"
        This is an example
    ??? quote "this is a quote"
        This is a quote

具体使用方法详见：[Admonitions](https://squidfunk.github.io/mkdocs-material/reference/admonitions/)[^3]

### Buttons[^2]

你可以在自己的文档中创建按钮，实现链接跳转。

```markdown
[Go to SAI!](https://soai.sjtu.edu.cn/){ .md-button }

[See the references](#references){ .md-button .md-button--primary }
```

??? Note "A simple demo"
    [Go to SAI!](https://soai.sjtu.edu.cn/){ .md-button }

    [See the references](#references){ .md-button .md-button--primary }

### Else

以上是最常用的两个功能，其他有关**字体、表格、代码块等的高级设置**均可以在[mkdocs 官方文档](https://squidfunk.github.io/mkdocs-material/reference/)找到References。

## Syntax Format

为了保证markdown渲染的一致性和统一性，我们建议各位贡献者规范markdown的书写格式。

建议参考：

- [https://github.com/sparanoid/chinese-copywriting-guidelines/blob/master/README.zh-Hans.md](https://github.com/sparanoid/chinese-copywriting-guidelines/blob/master/README.zh-Hans.md)

- [https://github.com/PKUFlyingPig/cs-self-learning/issues/114](https://github.com/PKUFlyingPig/cs-self-learning/issues/114)

## References

更多内容可参考以下文件：

- [commonmark](https://spec.commonmark.org/0.31.2/)


[^1]: https://squidfunk.github.io/mkdocs-material/
[^2]: [Buttons in mkdocs](https://squidfunk.github.io/mkdocs-material/reference/buttons/)
[^3]: [Admonitions in mkdocs](https://squidfunk.github.io/mkdocs-material/reference/admonitions/)