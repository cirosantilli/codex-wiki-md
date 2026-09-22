<h1 id="5d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Applying a [permutation](../../../../../../permutation.md) to the elements of an $r$-element subset preserves its cardinality. The identity fixes each subset and

$$
\sigma\cdot(\tau\cdot U)=\{\sigma(\tau(u)):u\in U\}=(\sigma\tau)\cdot U,
$$

so this is the [symmetric group action on subsets](../../../../../../symmetric-group-action-on-subsets.md). For two $r$-element subsets $U,W$, choose a bijection $U\to W$ and a bijection between their complements; together they define a [permutation](../../../../../../permutation.md) of the full $n$-element set. Hence **the action is transitive**.

A member of the [stabiliser subgroup](../../../../../../stabilizer-subgroup.md) must permute $U$ internally and its complement internally, with independent choices. Thus

$$
\boxed{|(S_n)_U|=r!(n-r)!,\qquad |\operatorname{Orb}(U)|=\binom nr.}
$$

This also agrees with the [orbit-stabilizer theorem](../../../../../../orbit-stabilizer-theorem.md); $0!=1$ handles $r=n$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5D](../../5d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
