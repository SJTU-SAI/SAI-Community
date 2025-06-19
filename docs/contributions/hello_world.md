---
title: Welcome Contributors
---
# For Contributors

!!! tip "Welcome!"
    我们诚挚地邀请并鼓励**任何人**积极分享你们在人工智能课程学习中（无论是课内还是课外）的**任何观点、想法和宝贵感悟**。在学习的旅程中，你们的每一次思考，无论是对课程内容的独到见解，对某个知识点的深入探讨，甚至是对课程的真实吐槽或者对其他优质教学资源的推荐分享，都将成为后来者的宝贵财富。

在AI时代，知识的迭代速度前所未有，技术的浪潮席卷每一个角落。我们既是时代的见证者，也必须是它的参与者——停滞意味着被淘汰，而学习则是对未来最基本的敬意。

正如古希腊哲学家赫拉克利特所言："**万物流变，无物常驻。**"在算法重塑世界的今天，保持清醒的批判性思维与持续更新的能力，或许是人类区别于机器的最后堡垒。不要追逐技术，而要理解技术；不要恐惧变化，而要成为变化本身。

我们深知，课程学习并非一帆风顺，其中既有茅塞顿开的喜悦，也有可能面对困惑与挑战。而你们的亲身经历和真诚分享，能为**即将踏上这段旅程的学弟学妹们提供最直接、最真实的参考**。

## 如何做出贡献？

无论你的贡献是大是小，我们都非常欢迎。你可以：

* **在评论区发表你的简短想法和疑问**。 如果你对某个知识点有小小的见解，或者某个问题想寻求讨论，直接在相关的评论区留言就非常合适。


* **通过 Pull Request (PR) 提交更正式、更详细的贡献**。 这包括：
    * **上传学习资料**：整理并分享你觉得有用的学习笔记、思维导图、参考资料等。
    * **分享学习经验和感悟**：撰写你的学习心得、踩坑经历、高效学习方法，或是对课程内容的深入剖析。
    * **对课程、作业考核或者任课教师的客观评价**。
    * 对其他优质教学资源的分享。
    * 对现有内容的修订、补充或优化。
    * 任何能帮助到学弟学妹的原创内容（或者转载，请务必声明来源和出处并符合规范）。

!!! info "MIT LICENSE"

    社区秉持着开放而包容的 [MIT 开源精神](https://opensource.org/license/mit)，鼓励任何内容和任何形式的贡献，但**请务必保证真实准确可靠的信息来源**。

    Sharing Drives Innovations!

## How to make Pull Requests?

PR教程指路: [Pull Requests](https://docs.github.com/en/pull-requests)

- 如果你认为网站的现有页面无法涵盖你需要更新的内容，请[**添加新页面**](#_2)。

- 如果你希望对网站现有课程添加你的新评论，请参考[**添加点评 & 学习心得分享**](#_3)。

- 如果你希望上传你的课程材料，请参考[**上传课程材料**](#_4)。

为了保证页面的整洁和一致性，我们欢迎各位在书写 markdown 文件的时候使 MkDocs 支持的一些高级 markdown 语法：

- [官方文档指南](https://squidfunk.github.io/mkdocs-material/reference/)

- [本站提供极简版中文翻译文档写作指南](markdown_tutorial.md)



!!! Danger 
    在完成相对应的修改后，请在**本地运行网站确认无误后再提交 PR**。本地运行需要进行一些环境配置，详见 [本地网页运行和环境配置](local_run.md)。

### 添加新页面

如果你希望添加新页面，请完成以下修改：

- 在 `template` 的 markdown 文件作为模版，创建一个新的 markdown 文件，放在对应的文件夹中。

- 在仓库的 `mkdocs.yml` 文件中添加对应的文件索引。

??? example "A simple demo"
    ```yaml
    # 如果你希望在大一第一学期课程中添加一个新的页面，内容是关于课程AI1001的，你可以做如下修改：

    # before the modificiations
    nav:
    - Hello World: "index.md"
    - About: "about.md"
    - Courses:
        - Semester 1.1:
            - 总结: "courses/Semester1.1/index.md"
    - Contributions:
        - README: "contributions/contributions.md"
        - Contributors: "contributions/contributors.md"
        - Pull Requests: "contributions/PR.md"
        - Markdown Usage: "templates/template_markdown.md"
        - Template: "templates/template.md"

    # after the modifications
    nav:
    - Hello World: "index.md"
    - About: "about.md"
    - Courses:
        - Semester 1.1:
            - 总结: "courses/Semester1.1/index.md"
            #   你需要修改的地方
            - SJTU-AI1001: "courses/Semester1.1/your_file.md"
    - Contributions:
        - README: "contributions/contributions.md"
        - Contributors: "contributions/contributors.md"
        - Pull Requests: "contributions/PR.md"
        - Markdown Usage: "templates/template_markdown.md"
        - Template: "templates/template.md"
    ```

- 提交 Pull Requests。

### 上传学习资料

推荐使用 `PDF` 或者 `.zip` 的形式，上传到自己的交大云盘（或者其他云存储服务），生成分享链接，并将下载链接添加到对应 markdown 文件末尾**课程资料**的表格中，提交 Pull Requests。

> 你不需要把文件整个提交到本仓库中，只需要提交文件的下载链接或者其他跳转链接即可。

Demo请跳转至 [A simple demo](../templates/template.md/#_4)。

### 添加点评 & 学习心得分享

直接修改对应的 markdown 文件后提交 Pull Requests 即可。为了保证可读性，我们建议**各位点评时使用 Admonitions 的高亮块包裹**，这样既分割了不同的评论，也可以通过不同颜色的选择的选择表达自己对这门课的态度。

我们认为一门课的评价应该是**多向度、因人而异的**，过于量化的评分结果只会适得其反造成判断失真。我们建议同学们在评价课程时**减少简单打分，多写具体感受**。数字评分容易掩盖课程的真正价值——同一门课可能让擅长理论的同学受益匪浅，却让偏好实践的同学无所适从。用文字描述你的真实学习体验：哪些内容让你豁然开朗？哪些环节有待改进？这样既能帮助老师优化教学，也能让其他同学根据自身特点做出更明智的选择。

!!! quote "a simple demo"

    例如：你可以这样：

    !!! success "Student A"
        A very Good Course!

    ??? danger "Student B (He/She chooses to hide his/her comments!)"
        分低事多，谁来谁后悔。

官方教程: [如何使用 Admonitions 包裹 markdown 块](https://squidfunk.github.io/mkdocs-material/reference/admonitions/)

我们提供了一份丐版的中文版教程，详见：[Tutorials for advanced markdown](markdown_tutorial.md/#admonitions)

!!! Note "All admonitions are demonstrated here"
    ??? note "this is a note"
        This is a note.
    ??? abstract "this is an abstract"
        This is an abstract.
    ??? info "this is an info"
        This is an info.
    ??? tip "this is a tip"
        This is a tip.
    ??? success "this is a success"
        This is a success.
    ??? question "this is a question"
        This is a question.
    ??? warning "this is a warning"
        This is a warning.
    ??? failure "this is a failure"
        This is a failure.
    ??? danger "this is a danger"
        This is a danger.
    ??? bug "this is a bug"
        This is a bug.
    ??? example "this is an example"
        This is an example.
    ??? quote "this is a quote"
        This is a quote.

---

**不积小流，何以成江海**？我们相信，每一个点滴的分享都能汇聚成巨大的力量，共同构建一个更丰富、更完善的学习资源库。我们期待你的加入，一起为人工智能专业的学习社区添砖加瓦！