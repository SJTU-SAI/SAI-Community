# Advanced Usage for markdown

Here are some advanced usage in markdown specifically in Mkdocs[^1]. Below are some demonstrations.

> A simple demo 的部分是上文markdown代码的实际展示。

更多设置请参考官方文档：[Official Docs](https://squidfunk.github.io/mkdocs-material/reference/)

## Admonitions（文本高亮框）

你可以在自己的文档中创建高亮文本框。

官方教程：[Admonitions](https://squidfunk.github.io/mkdocs-material/reference/admonitions/)

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

!!! Note "Here are all the admonitions"
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

## Fonts

对于有颜色的字体，可以使用HTML块包裹：
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

??? example "A simple demo"
    <!-- 不同大小和颜色的字体 -->
    <span style="font-size:24px; color:#015c43;font-family: 'Microsoft YaHei', '微软雅黑', sans-serif; font-weight: bold;">大号深绿色字体</span>

    <span style="font-size:16px; color:#e67e22;">中号橙色字体</span>这是正常字体。

    <!-- 居中显示 -->
    <p align="center">
    <span style="font-size:20px; color:#023c31;">居中深绿色字体</span>
    </p>

    <!-- 不居中显示 -->
    <span style="font-size:18px; color:#c0392b;">左对齐红色字体</span>

对于更加复杂的字体设置，可以在[官方教程](https://squidfunk.github.io/mkdocs-material/reference/formatting/)中找到支持。


## Buttons

你可以在自己的文档中创建按钮[^2]，实现链接跳转。

```markdown
[Go to SAI!](https://soai.sjtu.edu.cn/){ .md-button }

[See the fonts](#fonts){ .md-button .md-button--primary }
```

??? example "A simple demo"
    [Go to SAI!](https://soai.sjtu.edu.cn/){ .md-button }

    [See the fonts](#fonts){ .md-button .md-button--primary }

## 可视注释

```markdown
你好，这里是SAI，(1) 我是SAI的一名本科生。{ .annotate }

1. :smile: Wow, it is SAIer!
```

??? example "A simple demo"

    你好，这里是SAI, (1) 我是SAI的一名本科生。
    { .annotate }

    1.  :smile: Wow, it is SAIer!

> 注意空格和使用英文括号。

你也可以在代码的注释中添加annotations！

```py title="bubble_sort.py"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j] 
# (1)
```

1.  :confused: Is this correct?

## 代码块

### 代码块行数高亮

```markdown
```py title="bubble_sort.py" hl_lines="2 3"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j] 
```

??? example "a simple demo"
    ```py title="bubble_sort.py" hl_lines="2 3"
    def bubble_sort(items):
        for i in range(len(items)):
            for j in range(len(items) - 1 - i):
                if items[j] > items[j + 1]:
                    items[j], items[j + 1] = items[j + 1], items[j] 
    ```

像 [OI-wiki](https://oi-wiki.org/) 一样，也可以整合多个代码块。

```markdown
=== "C"

    ``` c
    #include <stdio.h>

    int main(void) {
      printf("Hello world!\n");
      return 0;
    }
    ```

=== "C++"

    ``` c++
    #include <iostream>

    int main(void) {
      std::cout << "Hello world!" << std::endl;
      return 0;
    }
    ```
```

??? example "a simple demo"
    === "C"

        ``` c
        #include <stdio.h>

        int main(void) {
        printf("Hello world!\n");
        return 0;
        }
        ```

    === "C++"

        ``` c++
        #include <iostream>

        int main(void) {
        std::cout << "Hello world!" << std::endl;
        return 0;
        }
        ```

## Mermaid 流程图

``` mermaid
graph LR
  A[Start] --> B{Error?};
  B -->|Yes| C[Hmm...];
  C --> D[Debug];
  D --> B;
  B ---->|No| E[Yay!];
```

链接：

- [Mermaid in Mkdocs](https://squidfunk.github.io/mkdocs-material/reference/diagrams/)

- [Official website for mermaid](https://mermaid.js.org/)


## 窗格

可以在文章的目录上使用，获得更好的视觉体验
```html
<div class="grid cards" markdown>

-   :material-clock-fast:{ .lg .middle } __Set up in 5 minutes__

    ---

    Install [`mkdocs-material`](#) with [`pip`](#) and get up
    and running in minutes

    [:octicons-arrow-right-24: Getting started](#)

-   :fontawesome-brands-markdown:{ .lg .middle } __It's just Markdown__

    ---

    Focus on your content and generate a responsive and searchable static site

    [:octicons-arrow-right-24: Reference](#)

-   :material-format-font:{ .lg .middle } __Made to measure__

    ---

    Change the colors, fonts, language, icons, logo and more with a few lines

    [:octicons-arrow-right-24: Customization](#)

-   :material-scale-balance:{ .lg .middle } __Open Source, MIT__

    ---

    Material for MkDocs is licensed under MIT and available on [GitHub]

    [:octicons-arrow-right-24: License](#)

</div>
```

??? example "A simple demo"
    <div class="grid cards" markdown>

    -   :material-clock-fast:{ .lg .middle } __Set up in 5 minutes__

        ---

        Install [`mkdocs-material`](#) with [`pip`](#) and get up
        and running in minutes

        [:octicons-arrow-right-24: Getting started](#)

    -   :fontawesome-brands-markdown:{ .lg .middle } __It's just Markdown__

        ---

        Focus on your content and generate a responsive and searchable static site

        [:octicons-arrow-right-24: Reference](#)

    -   :material-format-font:{ .lg .middle } __Made to measure__

        ---

        Change the colors, fonts, language, icons, logo and more with a few lines

        [:octicons-arrow-right-24: Customization](#)

    -   :material-scale-balance:{ .lg .middle } __Open Source, MIT__

        ---

        Material for MkDocs is licensed under MIT and available on [GitHub]

        [:octicons-arrow-right-24: License](#)

    </div>

## 符号和表情

本站支持**FontAwesome**[^4]，一款广受欢迎的免费开源图标库，提供超过 2,000+ 个可缩放矢量图标。

```markdown
:smile:
:fontawesome-solid-file-zipper:{ .saic }
```

:smile:
:fontawesome-solid-file-zipper:{ .saic }

如果需要添加新的css，请发起PR。

## 数学公式

环境配置完成，可正常使用。

$$
\cos x=\sum_{k=0}^{\infty}\frac{(-1)^k}{(2k)!}x^{2k}
$$

## markdown 书写排版规范

建议参考：

- [https://github.com/sparanoid/chinese-copywriting-guidelines/blob/master/README.zh-Hans.md](https://github.com/sparanoid/chinese-copywriting-guidelines/blob/master/README.zh-Hans.md)

- [https://github.com/PKUFlyingPig/cs-self-learning/issues/114](https://github.com/PKUFlyingPig/cs-self-learning/issues/114)


[^1]: [Official website for mkdocs material](https://squidfunk.github.io/mkdocs-material/)
[^2]: [Buttons in mkdocs](https://squidfunk.github.io/mkdocs-material/reference/buttons/)
[^3]: [Admonitions in mkdocs](https://squidfunk.github.io/mkdocs-material/reference/admonitions/)
[^4]: [Font Awesome](https://fontawesome.com/)