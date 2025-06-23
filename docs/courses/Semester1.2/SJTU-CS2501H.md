# SJTU-CS2501H: 离散数学（荣誉）

<!-- 课程的基本信息简介 -->
<!-- 这一部分主要记录老师们上课的客观信息，例如考核方式和授课范围等 -->
## 课程基本信息简介

<!-- 下面一行请勿删除，注意缩进 -->
<!-- markdown 格式详见: https://squidfunk.github.io/mkdocs-material/reference/admonitions/ -->
!!! info "Basic information"

    :fontawesome-solid-bolt:{ .lightning } 课程教师：曹钦翔

    :fontawesome-solid-bolt:{ .lightning } 授课内容与范围：集合论，数理逻辑，基础图论（详细见下面）

    :fontawesome-solid-bolt:{ .lightning } 学时&学分：3学时，3学分

    :fontawesome-solid-bolt:{ .lightning } 考核方式：课程参与分10%+课后作业35%+课前作业5%+期末50%，大作业加分，但名额较少


<!-- You are free to add some contents in it! -->
### 其他信息

!!! warning "特别提醒"
    - 这是一门双语课，上课用中文，PPT、lecture notes、homework、exams都是英文，考试不得使用翻译工具

    - 作业允许使用AI以及和别人讨论，但是必须标明出处（如AI提供答案需要有和AI对话的截图），且一般使用AI不会影响作业成绩

??? tip "教科书+参考资料"

    Kenneth H. Rosen, Discrete Mathematics and Its Applications, 8th edition [R], 教科书

    Elements of Set Theory, Herbert B. Enderton, Academic Press Inc., 1977, ISBN 0-12-238440-7, 教科书

    Ebbinghaus, Heinz-Dieter. Mathematical Logic. Springer, 1996. 参考资料

    Thomas Jech. Set Theory. Springer, correct 4th printing 2006. 参考资料

    《图论与代数结构》，戴一奇，清华大学出版社，1995, ISBN 7-302-01814-6， 参考资料

    Daniel Kroening, Ofer Strichman. Decision Procedures, An Algorithmic Point of View. Springer, 2008. 参考资料

    《数理逻辑与集合论》，石纯一等，清华大学出版社，2000, 第二版, ISBN 7-302-04042-7，参考资料（推荐学习数理逻辑时参考这个）

!!! tip "课程分数详细评价机制："

    课后作业35分，每节课后发一次作业，一次3分，只有全对才能3分拿满，多小问的题错一问等价于错这一整个题

    课前可能在canvas上面发选择题作业（不过这项貌似只执行了一个月）

    课堂参与分机制{--较为离谱--}，具体如下

    - 缺勤一次扣2分（上限 -2），签过一次到

    - 课堂提问、回答问题一次加 2-3 分

    - 课程群每次有意义的提问、发言算 0.5/1 分

    - 完成可选大作业直接10分，但是大作业名额只有 1/5 ，分配方式同抢课，很可能抢不到

    {==注意，就算你每节课都到勤，如果不提问发言，课堂参与分也是0分==}


??? tip "24届同学上课大纲（为了术语准确性，用英文）"
    集合论：

    - Sets, Operations on sets ( Power sets, Indexed union, Indexed intersection, General Union )

    - Binary Relations and their affiliated operators ( especially composition )

    - Equivalence relations, equivalence classes and partitions

    - Transitive closures and their properties

    - Functions, injections, surjections and bijections

    - Cardinality, properties of equinumerosity and countability ( including function sets )

    - Proof of Bernstein theorem and Cantor theorem

    - Inductive Sets, Construction of numbers based on axiomatic set theory

    - Russel Paradox, ZFC

    逻辑：

    - Propositional Logic, Logic Connectives

    - First Order Logic and semantic theory ( interpretation )

    - Consequence Relation, Logical Equivalence and their proofs based on semantic theory

    - Quantifiers in First Order Logic

    - Interpreting logic behind natural language proof

    - Tautology, contradiction, satisfiable statements and their conversion

    - CNF, DNF and algorithms for generating CNF

    - Algorithms for solving SAT

    - Proof theory and inference rules

    - Properties of Coq

    图论：

    - Concepts and classifications regarding graphs

    - Handshaking theorem

    - (Simple) paths, circuits and properties of connectivity

    - Definitions and properties of trees

    - Minimum spanning tree and its proof

    - Depth-first search, its properties and applications ( Tarjan algorithm for bridges )

    - Huffman coding and its proof


<!-- 对课程的主观性评价请放在这里，包括对学弟学妹的建议等等 -->
<!-- markdown 格式详见: https://squidfunk.github.io/mkdocs-material/reference/admonitions/ -->
## 课程评价

??? warning "来自一位SAI学生"
    选课评分不好，结合个人体验分析一下这门课的一些问题：

    1. 教学内容问题：

        - 整门课明显偏数学而非偏算法，和AI专业学生的需求有些脱节

        - 数理逻辑讲的顺序有些奇怪，和清华教材完全反着，上来就讲一阶逻辑和 interpretation 很让人费解

        - 数理逻辑知识过于零散，导致除了一堆符号感觉啥都没学到

        - 图论部分和同期数据结构重合太多，图论中的哈密顿回路、欧拉定理都没讲

        - 整门课对于一些概念的定义和普遍定义不同（{==例如为什么 simple paths 的定义是不重复边而不是直接不重复点？==}），导致学生在概念理解上浪费了太多时间

    2. 教学评价问题：（最大痛点）

        - 作业3分向下取整的评分机制让人很有挫败感，且本身作业花费时间就多，体验比较差

        - 课堂参与分非常难评，本身160人大教室听课效果就差，还强制学生在课上发言，导致很多人为了参与分提问拖慢课堂进度

        - 大作业刻意限制名额，学生要像抢课一样抢大作业名额，比较不公平（有一项作业我很想写却没抢到）

        - 考试不定项选择题过于恶心，且似乎不管漏选多选都是0分

        - lecture notes 太过粗略，我看 lecture notes 很难理解课程内容，且作业不发答案，设置了很多额外的困难



## 课程资源

<!-- PDF or zip-->
<!-- icons for pdf :fontawesome-solid-file-pdf:{ .saic } -->
<!-- icons for zip :fontawesome-solid-file-zipper:{ .saic } -->
<!-- 存储链接推荐使用jbox云盘或者其他云服务器，在表格中只需要贴上下载链接即可，建议zip或者PDF文件，贴其他网站的链接也可以 -->


| 贡献者            |   Description        |     Download Link                  |
| ----            |------                | ------------------------------------ |
|||



