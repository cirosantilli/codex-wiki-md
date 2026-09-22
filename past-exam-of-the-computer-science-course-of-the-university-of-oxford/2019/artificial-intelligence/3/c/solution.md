<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Ground $b,x$ as distinct blocks. For $\operatorname{MoveToTable}(b,x)$, take

$$
\begin{aligned}
\operatorname{Pre}&=\{\operatorname{Block}(b),\operatorname{Block}(x),\operatorname{On}(b,x),\operatorname{Clear}(b)\},\\
\operatorname{Add}&=\{\operatorname{On}(b,\tau),\operatorname{Clear}(x)\},\\
\operatorname{Del}&=\{\operatorname{On}(b,x)\}.
\end{aligned}
$$

Thus a clear block leaves its block support, makes that support clear, and joins the unlimited table. **$\operatorname{Clear}(b)$ persists, and table availability is never deleted.** Requiring $x$ to be a block excludes a redundant table-to-table action. The static [predicates](../../../../../predicate.md) need not be stored as time-varying [planning fluents](../../../../../planning-fluent.md).

## ↑ Ancestors (11)

1. [C](../c.md)
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
