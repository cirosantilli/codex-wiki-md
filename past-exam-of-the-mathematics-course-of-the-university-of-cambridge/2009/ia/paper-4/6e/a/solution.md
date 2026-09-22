<h1 id="6e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For finite sets $X_1,\ldots,X_N$, the [inclusion-exclusion principle](../../../../../../inclusion-exclusion-principle.md) states

$$
\boxed{\left|\bigcup_{i=1}^NX_i\right|=\sum_{r=1}^N(-1)^{r-1}\sum_{1\leq i_1<\cdots<i_r\leq N}|X_{i_1}\cap\cdots\cap X_{i_r}|.}
$$

To prove it, fix an element belonging to exactly $s\geq1$ of these sets. At level $r$ it is counted in precisely $\binom sr$ intersections, so its total multiplicity on the right is

$$
\sum_{r=1}^s(-1)^{r-1}\binom sr=1-(1-1)^s=1
$$

by the [binomial theorem](../../../../../../binomial-theorem.md). An element in no set contributes zero. Summing these equal multiplicities over the finite union proves [inclusion-exclusion](../../../../../../inclusion-exclusion-principle.md). This also explains why pairwise subtraction alone is insufficient: elements in triple and higher intersections must receive the alternating corrections.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6E](../../6e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
