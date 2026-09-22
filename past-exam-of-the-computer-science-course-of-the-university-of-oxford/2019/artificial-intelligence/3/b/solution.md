<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use direct-transfer [STRIPS](../../../../../strips.md) actions: one action includes picking up a block and putting it down again. There is no separate holding state. Ground $b,y$ as distinct blocks and $x$ as a support, either a block or the table, with $x\ne b$ and $x\ne y$.

For $\operatorname{Move}(b,x,y)$, take

$$
\begin{aligned}
\operatorname{Pre}&=\{\operatorname{Block}(b),\operatorname{Block}(y),\operatorname{On}(b,x),\operatorname{Clear}(b),\operatorname{Clear}(y)\},\\
\operatorname{Add}&=\{\operatorname{On}(b,y)\}\cup\bigl(\{\operatorname{Clear}(x)\}\text{ if }x\ne\tau\bigr),\\
\operatorname{Del}&=\{\operatorname{On}(b,x),\operatorname{Clear}(y)\}.
\end{aligned}
$$

The [preconditions](../../../../../precondition.md) ensure that $b$ can be picked up and that the destination has room. Moving it frees a block source and occupies the destination, while $\operatorname{Clear}(b)$ persists. When $x=\tau$, table availability remains true; its redundant addition is simply omitted. Since $x$ is fixed in each [ground action](../../../../../ground-action.md), this case distinction constructs ordinary add lists rather than introducing conditional action effects. The [search transition model](../../../../../search-transition-model.md) is **$(S\setminus\operatorname{Del})\cup\operatorname{Add}$**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
