# SJTU-CS2501H: 离散数学（荣誉）

<!-- 课程的基本信息简介 -->
<!-- 这一部分主要记录老师们上课的客观信息，例如考核方式和授课范围等 -->
## 课程基本信息简介

<!-- 下面一行请勿删除，注意缩进 -->
<!-- markdown 格式详见: https://squidfunk.github.io/mkdocs-material/reference/admonitions/ -->
!!! info "Basic information"

    :fontawesome-solid-bolt:{ .lightning } 课程教师：曹钦翔

    :fontawesome-solid-bolt:{ .lightning } 授课内容与范围：集合论，数理逻辑，基础图论（详细见下面）

    :fontawesome-solid-bolt:{ .lightning } 学时 & 学分：3 学时，3 学分

    :fontawesome-solid-bolt:{ .lightning } 考核方式：课程参与分 10% + 课后作业 35% + 课前作业 5% + 期末 50%，大作业加分，但名额较少


<!-- You are free to add some contents in it! -->
### 其他信息

!!! warning "特别提醒"
    - 这是一门双语课，上课用中文，而 slides、lecture notes、homework、exams 都是英文，考试不得使用翻译工具。

    - 作业允许使用 AI 以及和别人讨论，但是必须标明出处（如 AI 提供答案需要有和 AI 对话的截图），且一般使用 AI 不会影响作业成绩。

??? tip "教科书 + 参考资料"

    Kenneth H. Rosen, Discrete Mathematics and Its Applications, 8th edition [R], 教科书

    Elements of Set Theory, Herbert B. Enderton, Academic Press Inc., 1977, ISBN 0-12-238440-7, 教科书

    Ebbinghaus, Heinz-Dieter. Mathematical Logic. Springer, 1996. 参考资料（同学 B 推荐学习数理逻辑时参考这个）

    Thomas Jech. Set Theory. Springer, correct 4th printing 2006. 参考资料（很难，无需掌握）

    《图论与代数结构》，戴一奇，清华大学出版社，1995, ISBN 7-302-01814-6， 参考资料

    Daniel Kroening, Ofer Strichman. Decision Procedures, An Algorithmic Point of View. Springer, 2008. 参考资料

    《数理逻辑与集合论》，石纯一等，清华大学出版社，2000, 第二版, ISBN 7-302-04042-7，参考资料（同学 A 推荐学习数理逻辑时参考这个）

!!! tip "课程分数详细评价机制："

    课后作业 35 分。每节课后发一次作业，3 分制且向下取整，只有全对才能 3 分拿满，多小问的题错一问等价于错这一整个题。

    课前可能在 canvas 上面发选择题预习作业（图论部分因和数据结构课程重叠，没有预习作业）。

    课堂参与分机制（满分 10，先作用加分项，再与 10 取 min，然后作用扣分项，再与 0 取 max）：

    - 缺勤一次扣 2 分，签过一次到

    - 课堂提问、回答问题一次加 2-3 分

    - 课程群每次有意义的提问、发言算 0.5/1 分

    - 完成可选大作业直接10分，但是大作业名额只有 1/5，分配方式同抢课，很可能抢不到

    {==注意，就算你每节课都到勤，如果不提问发言，课堂参与分也是 0 分。==}


??? tip "24 届大纲"
    (Naive, for most of the part) Set Theory:

    - sets, operations on sets (power sets, indexed union and intersection, general union)

    - relations, inverses and compositions, their properties 

    - equivalence relations, equivalence classes, partitions

    - transitive closures, reflexive transitive closures

    - functions, injections and surjections and bijections

    - equinumerosity and countability (including the sets of functions)

    - Bernstein theorem, Cantor theorem

    - inductive sets, the set of natural numbers

    - Russell's paradox and axiomatic set theory (ZFC)

	- construction of $\mathbb Z, \mathbb Q, \mathbb R, \mathbb C$ and integer arithmetic based on axiomatic set theory

	- construction of (reflexive) transitive closure based on axiomatic set theory


	(Propositional and First-Order) Logic:

    - propositional logic, logical connectives

    - first order logic, semantics of first-order logic 

    - consequence lelation, logical equivalence

    - interpreting logic behind natural language proof

    - tautology, contradiction, satisfiability, their conversion

    - CNF, DNF, algorithms for generating CNF

    - SAT solver algorithms (brute-force, DPLL, CDCL)

    - proof theory and inference rules

    - Coq basics

	Graph theory:

	- basic concepts

    - the handshaking theorem

    - properties of connectivity, (strongly) connected components

    - definitions and properties of trees and rooted trees

    - minimum spanning trees, Prim's and Kruskal's algorithm

    - DFS, its properties, its applications (Tarjan's algorithm for finding bridges)

    - Huffman encoding 


<!-- 对课程的主观性评价请放在这里，包括对学弟学妹的建议等等 -->
<!-- markdown 格式详见: https://squidfunk.github.io/mkdocs-material/reference/admonitions/ -->
## 课程评价

??? warning "来自一位 SAI 学生"
    选课评分不好，结合个人体验分析一下这门课的一些问题：

    1. 教学内容问题：

        - 整门课明显偏数学而非偏算法，和 AI 专业学生的需求有些脱节

        - 数理逻辑讲的顺序有些奇怪，和清华教材完全反着，上来就讲一阶逻辑和 interpretation 很让人费解

        - 数理逻辑知识过于零散，导致除了一堆符号感觉啥都没学到

        - 图论部分和同期数据结构重合太多，图论中的哈密顿回路、欧拉定理都没讲

        - 整门课对于一些概念的定义和普遍定义不同（{==例如为什么 simple paths 的定义是不重复边而不是直接不重复点？==}），导致学生在概念理解上浪费了太多时间

    2. 教学评价问题：（最大痛点）

        - 作业3 分向下取整的评分机制让人很有挫败感，且本身作业花费时间就多，体验比较差

        - 课堂参与分非常难评，本身 160 人大教室听课效果就差，还强制学生在课上发言，导致很多人为了参与分提问拖慢课堂进度

        - 大作业刻意限制名额，学生要像抢课一样抢大作业名额，比较不公平（有一项作业我很想写却没抢到）

        - 考试不定项选择题过于恶心，且似乎不管漏选多选都是0分

        - lecture notes 太过粗略，我看 lecture notes 很难理解课程内容，且作业不发答案，设置了很多额外的困难



??? success "来自另一位 SAI 学生"
	我个人很喜欢这门课，我认为它瑕不掩瑜。是的，这门课的评价就是这么两极分化。我挽尊一些负面评价。

	1. 关于授课内容。我认为曹钦翔老师讲的很清晰。数理逻辑的讲法是完全没问题的，不要用对一本教材的认知去否定其他的教材与讲法，更不要因为自己没学过一阶逻辑就认为这奇怪甚至没用。集合论与数理逻辑本就是数学大厦的根基，有时显得有些枯燥而缺乏实际的 insight，这是这两个学科的特点，我认为它们也自有其魅力所在。菜就多练。

	2. 关于评分标准。是的，作业的评分标准很严格，但我认为大部分时候的评分都是公允、无可挑剔的。菜就多练。

	3. 曹钦翔老师期末海底捞，给分很好。

	4. Lecture Notes 有时候的确有点抽象，有时候会有抽象的英语语法和拼写错误。我认为如果你听了课，Lecture Notes 应当是能看懂的，也能够作为不错的复习资料。



## 课程资源

<!-- PDF or zip-->
<!-- icons for pdf :fontawesome-solid-file-pdf:{ .saic } -->
<!-- icons for zip :fontawesome-solid-file-zipper:{ .saic } -->
<!-- 存储链接推荐使用jbox云盘或者其他云服务器，在表格中只需要贴上下载链接即可，建议zip或者PDF文件，贴其他网站的链接也可以 -->


| 贡献者            |   Description        |     Download Link                  |
| ----            |------                | ------------------------------------ |
| 陈志杰 | 个人的作业参考答案 | [仅供参考，抄袭后果自负](https://github.com/melonTree68/discrete-mathematics-homework) |



