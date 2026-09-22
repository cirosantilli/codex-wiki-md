<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**[Forward checking](../../../../../forward-checking.md) makes [minimum remaining values](../../../../../minimum-remaining-values.md) respond to current restrictions rather than the original [constraint domain](../../../../../constraint-domain.md) sizes.** After $X=v$, its neighbors may have fewer choices, become forced or lose all choices. [Minimum remaining values](../../../../../minimum-remaining-values.md) then selects the newly constrained [variable](../../../../../variable-mathematics.md) early, while an empty [constraint domain](../../../../../constraint-domain.md) triggers immediate failure. The two mechanisms expose failure sooner and reduce wasted [backtracking](../../../../../backtracking.md).

[Forward checking](../../../../../forward-checking.md) only tests an unassigned neighbor against the newly assigned value. It need not check whether two still-unassigned [variables](../../../../../variable-mathematics.md) have mutually supporting values. [Arc consistency](../../../../../arc-consistency.md) requires every value at either end of each [binary constraint](../../../../../binary-constraint.md) to have support in the other [constraint domain](../../../../../constraint-domain.md), and [AC-3](../../../../../ac-3.md) propagates deletions until this condition stabilizes or a [constraint domain](../../../../../constraint-domain.md) becomes empty.[§2.3, forward checking and the directed support test](../../../../../cs-188-constraint-filtering-notes.md)

For example, let $X,Y,Z$ initially have [constraint domains](../../../../../constraint-domain.md) $\{1,2\}$ with constraints $X\ne Y$ and $Y\ne Z$. Assigning $X=1$ makes [forward checking](../../../../../forward-checking.md) reduce $D_Y$ to $\{2\}$, but leaves $D_Z=\{1,2\}$. [Arc consistency](../../../../../arc-consistency.md) also deletes $2$ from $D_Z$, leaving $\{1\}$. Neither procedure alone decides every general [constraint satisfaction problem](../../../../../constraint-satisfaction-problem.md): a triangle of two-valued inequalities satisfies [arc consistency](../../../../../arc-consistency.md) but is unsatisfiable.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2020](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
