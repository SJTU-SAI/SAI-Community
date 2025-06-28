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


??? success "来自一位 SAI 学生"
    **“痛恨cqx，理解cqx，成为cqx。”**

    选课社区里的这句话，精准地概括了许多人（包括我）对这门课的感受。

    平心而论，这门课起初并不合我的胃口，相信不少同学也是如此。相比于目标明确、反馈直接的算法学习，数理逻辑这门课所探讨的，是更为抽象、底层的思维方式。它很难，需要投入大量时间，过程也时常伴随着挫败感。

    这种挫败感，部分源于不甚理想的上课体验。比如，在大教室里，听讲效果难免打折扣；初次接触一阶逻辑，面对老师板书上如同天书般的 $[[∃xP(x)]]_J[x↦a]$符号，会感到不知所措；
    作业评分非常严格，有时甚至是“向下取整”，再加上一些强制参与的机制，难免让人心生怨言。

    然而，当一学期结束，我才真正理解这门课的价值——它所带来的思维训练，其收获远非一个好成绩所能衡量。

    想要学好这门课，关键在于学习态度。**你的课堂投入程度，几乎直接决定了你的学习体验。** 如果从一开始就抱着抵触心理，上课分心，课后想“亡羊补牢”会非常吃力，很容易陷入“听不懂—更厌恶—更听不懂”的负面循环。
    相反，如果你能从一开始就紧跟老师的思路和符号体系，课后及时消化，你会发现那些看似艰涩的内容，其实并没有想象中那么遥不可及。

    这里也给后来的同学一些建议：

    1. **适应符号体系是关键。** 数理逻辑的“劝退”感多源于此，一旦适应，便会豁然开朗。

    2. **寻求外部辅助。** 我个人认为清华大学的教材讲法更容易入门，可以作为辅助理解的材料。此外，我也强烈推荐 Gemini，它在我期末复习时帮了大忙。

    3. **未来的体验会更好。** 据我所知，下一届课程会对大教室、参与机制和大作业分配等问题进行调整。同时，有了我们这一届的作业作为参考，大家的学习压力应该会小很多。

    当然，课程也有其他可以改进的地方。比如图论部分与数据结构重合较多，让人感觉新知识不多，但这部分未来也可能会调整。此外，课程的讲义（Lecture Notes）确实略显粗略，如果能更详尽一些，对自学将会更有帮助。

    最后，必须承认课程的给分是相当不错的。尤其是期末慷慨的“捞人”环节，我即使有十分的判断题因方向错误而丢分，且整门课掌握的不算扎实，最终成绩也依然体面。

    但这又引出了一个更深层的问题：当我们评价一门课时，我们究竟在期待什么？是宽松的作业、自由的考勤和漂亮的分数吗？还是那些真正能挑战我们、启发我们，甚至重塑我们思维方式的东西？

    对我而言，这门课的意义远大于此。它是一次真正的思维淬炼。

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



