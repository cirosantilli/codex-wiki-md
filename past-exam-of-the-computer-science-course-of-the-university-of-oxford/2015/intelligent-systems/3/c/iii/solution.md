<h1 id="3/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**True in some cases and false in others.** Equality of the [constraint domain](../../../../../../constraint-domain.md) size and [treewidth](../../../../../../treewidth.md) does not decide satisfiability.

For an unsatisfiable example, let $D=\{0,1\}$ and impose the three binary [all-different constraints](../../../../../../all-different-constraint.md) $X_1\ne X_2$, $X_2\ne X_3$, and $X_3\ne X_1$. The [primal graph](../../../../../../primal-graph.md) is a triangle, with [treewidth](../../../../../../treewidth.md) two. It needs three different values, so no solution exists despite $|D|=\operatorname{tw}(P)=2$.

For a satisfiable example, take four [variables](../../../../../../variable-mathematics.md) with the same [constraint domain](../../../../../../constraint-domain.md) and constraints

$$
X_1\ne X_2,\quad X_2\ne X_3,\quad X_3\ne X_4,\quad X_4\ne X_1.
$$

Its [primal graph](../../../../../../primal-graph.md) is a four-cycle of [treewidth](../../../../../../treewidth.md) two: bags $\{1,2,3\}$ and $\{1,3,4\}$ give width two, while width one would require a [forest](../../../../../../forest.md). The assignment $(0,1,0,1)$ satisfies all constraints.

$$
\boxed{|D|=\operatorname{tw}(P)\text{ allows both satisfiable and unsatisfiable instances}.}
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Intelligent systems](../../../../intelligent-systems-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
