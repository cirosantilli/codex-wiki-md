<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [linear operator](../../../../linear-operator.md) has closed graph when $\{(x,Tx):x\in X\}$ is closed in $X\times Y$. The [closed graph theorem](../../../../closed-graph-theorem.md) states that an everywhere-defined [linear operator](../../../../linear-operator.md) between [Banach spaces](../../../../banach-space-split.md) is bounded if and only if it has closed graph. Boundedness gives the closed-graph property by continuity. Conversely a closed graph is Banach in the product [norm](../../../../norm.md) $\|(x,y)\|=\|x\|+\|y\|$. Projection of the graph onto $X$ is a bounded linear bijection, so the [open mapping theorem](../../../../open-mapping-theorem-functional-analysis.md) makes its inverse bounded. Composing that inverse with the second-coordinate projection proves **$T$ is bounded**.

For the composition assertion, suppose $x_n\to x$ and $Tx_n\to y$. Boundedness of $S$ gives $STx_n\to Sy$, and boundedness of $ST$ gives $STx_n\to STx$. Injectivity of $S$ forces $y=Tx$. Hence $T$ has closed graph and is bounded by the theorem.

For the derivative bound take $Y=C^1[0,1]$ with [norm](../../../../norm.md) $\|v\|_{C^1}=\|v\|_\infty+\|v'\|_\infty$, and $Z=C[0,1]$ with its [supremum norm](../../../../supremum-norm.md); both are Banach. Regard $T(x)=Ux$ as a map into $Y$, and let $S:Y\to Z$ be inclusion. This inclusion is bounded and injective, and $ST=U$ is bounded by hypothesis. The preceding result gives a constant $c$ with $\|Ux\|_{C^1}\leq c\|x\|$. In particular **$|(Ux)'(t)|\leq c\|x\|$ uniformly in $t$**.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../split.md)
5. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
