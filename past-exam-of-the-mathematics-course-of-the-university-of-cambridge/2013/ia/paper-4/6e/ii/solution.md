<h1 id="6e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For finitely many finite sets $A_1,\ldots,A_k$, the [inclusion-exclusion principle](../../../../../../inclusion-exclusion-principle.md) states

$$
\boxed{\left|\bigcup_{i=1}^kA_i\right|
=\sum_{\varnothing\ne J\subseteq\{1,\ldots,k\}}
(-1)^{|J|+1}\left|\bigcap_{j\in J}A_j\right|.}
$$

To see why, an element belonging to exactly $t\geq1$ of the sets contributes

$$
\sum_{j=1}^t(-1)^{j+1}\binom tj=1
$$

by the [binomial theorem](../../../../../../binomial-theorem.md). Elements outside the union contribute zero. Equivalently, if these sets lie in a finite universe $U$, the number avoiding all of them is

$$
|U|+\sum_{\varnothing\ne J}(-1)^{|J|}
\left|\bigcap_{j\in J}A_j\right|.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6E](../../6e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
