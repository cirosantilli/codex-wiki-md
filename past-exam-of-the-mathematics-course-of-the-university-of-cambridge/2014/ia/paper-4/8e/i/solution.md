<h1 id="8e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For [finite sets](../../../../../../finite-set.md) $A_1,\ldots,A_r$, the [inclusion-exclusion principle](../../../../../../inclusion-exclusion-principle.md) states

$$
\boxed{\left|\bigcup_{i=1}^rA_i\right|=\sum_{\varnothing\ne J\subseteq\{1,\ldots,r\}}(-1)^{|J|+1}\left|\bigcap_{j\in J}A_j\right|.}
$$

To prove it, count the contribution of one element. If it belongs to exactly $q\geq1$ of the [sets](../../../../../../set-split.md), it is counted by $\binom qk$ intersections of size $k$. Its total weight is

$$
\sum_{k=1}^q(-1)^{k+1}\binom qk=1-(1-1)^q=1,
$$

using the [binomial theorem](../../../../../../binomial-theorem.md). An element belonging to none contributes zero. Summing these weights gives the [cardinality](../../../../../../cardinality.md) of the union and proves the [inclusion-exclusion principle](../../../../../../inclusion-exclusion-principle.md). Equivalently, within a finite ambient [set](../../../../../../set-split.md) $U$, the number avoiding every $A_i$ is the sum over all $J$, with sign $(-1)^{|J|}$ and the empty intersection interpreted as $U$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [8E](../../8e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
