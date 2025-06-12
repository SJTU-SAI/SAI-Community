# For Contributors

我们诚挚地邀请并鼓励**任何人**积极分享你们在人工智能课程学习中的观点、想法和宝贵感悟。

在学习的旅程中，你们的每一次思考，无论是对课程内容的独到见解，对某个知识点的深入探讨，甚至是对课程的真实吐槽，都将成为后来者的宝贵财富。

我们深知，课程学习并非一帆风顺，其中既有茅塞顿开的喜悦，也有可能面对困惑与挑战。而你们的亲身经历和真诚分享，能为**即将踏上这段旅程的学弟学妹们提供最直接、最真实的参考**。

## 如何做出贡献？

我们鼓励**所有人分享有关课程内容、学习生活等方面的所有内容**！但前提是必须**保证内容的客观、真实、准确**。可以是对培养计划中课程或者老师的评价（吐槽），可以是对其他优质教学资源的推荐或者分享，可以是自己撰写的教程或者其他种种...

在AI时代，知识的迭代速度前所未有，技术的浪潮席卷每一个角落。我们既是时代的见证者，也必须是它的参与者——停滞意味着被淘汰，而学习则是对未来最基本的敬意。  

正如古希腊哲学家赫拉克利特所言："**万物流变，无物常驻。**"在算法重塑世界的今天，保持清醒的批判性思维与持续更新的能力，或许是人类区别于机器的最后堡垒。不要追逐技术，而要理解技术；不要恐惧变化，而要成为变化本身。

无论你的贡献是大是小，我们都非常欢迎。你可以：

* **在评论区发表你的简短想法和疑问**。 如果你对某个知识点有小小的见解，或者某个问题想寻求讨论，直接在相关的评论区留言就非常合适。
* **通过 Pull Request (PR) 提交更正式、更详细的贡献**。 这包括：
    * **上传学习资料**：整理并分享你觉得有用的学习笔记、思维导图、参考资料等。
    * **分享学习经验和感悟**：撰写你的学习心得、踩坑经历、高效学习方法，或是对课程内容的深入剖析。
    * **对课程、作业考核或者任课教师的客观评价**。
    * 对现有内容的修订、补充或优化。
    * 任何能帮助到学弟学妹的原创内容。

**不积小流，何以成江海**？我们相信，每一个点滴的分享都能汇聚成巨大的力量，共同构建一个更丰富、更完善的学习资源库。


## 如何提交你的贡献？

### 简单评论

直接在相关文档或讨论区的评论框内输入你的内容即可。

!!! failure

    评论系统很快会上线

<!-- !todo Add giscus and github discussions -->

### 使用Pull Requests

教程指路: [Pull Requests](https://docs.github.com/en/pull-requests)

#### 添加新页面

如果你希望添加新页面，请完成以下修改：

- 在代码树中新建markdown文件，添加新页面的内容。可以以`template`的markdown文件作为参考。

- 在`/mkdocs.yml`中添加对应的文件索引。

??? example "A simple demo"
    ```yaml
    # 如果你希望在大一第一学期课程中添加一个新的页面，内容是关于课程AI1001的，你可以做如下修改：

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

- 提交Pull Requests。

#### 上传学习资料

推荐使用`PDF`或者`.zip`的形式，上传到自己的交大云盘（或者其他云存储服务），生成分享链接，并将下载链接添加到**课程资料**的表格中。

#### 添加点评 & 学习心得分享

直接修改对应的markdown文件即可，为了保证可读性，我们建议各位点评时使用Admonitions的高亮块包裹，这样既分割了不同的评论，也可以通过Admonitions的选择表达自己对这门课的态度。

??? Note "A simple demo for Admonitions"
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


[具体的使用教程](./markdown_tutorial.md){ .md-button }

我们会尽快审核你的 PR，并在通过后合并到主分支中。


我们期待你的加入，一起为人工智能专业的学习社区添砖加瓦！