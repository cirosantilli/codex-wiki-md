<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Young permutation module](../../../../../../young-permutation-module.md) $M^{(n-k,k)}$ is the [symmetric-group subset permutation representation](../../../../../../symmetric-group-subset-permutation-representation.md) on the $k$-element subsets of $\{1,\ldots,n\}$: the second row of a [tabloid](../../../../../../tabloid.md) specifies the subset. For $k\geq1$, [restriction of a character](../../../../../../restriction-of-a-character.md) to $S_{n-1}$ fixing $n$ splits these subsets into two [orbits of a group action](../../../../../../orbit-of-a-group-action.md), according as they contain $n$.

The corresponding [permutation representations](../../../../../../permutation-representation.md) are on the $k$-subsets and the $(k-1)$-subsets of $\{1,\ldots,n-1\}$. Their [Young permutation modules](../../../../../../young-permutation-module.md) have two row sizes $n-1-k,k$ and $n-k,k-1$, respectively. Sort each pair into decreasing order and omit any zero part; swapping the two row labels gives an isomorphic [permutation representation](../../../../../../permutation-representation.md). This sorting matters at $n=2k$.

We use [Young's rule](../../../../../../young-s-rule.md): over the [complex numbers](../../../../../../complex-number.md), the multiplicity of $S^\rho$ in $M^\eta$ is the [Kostka number](../../../../../../kostka-number.md) $K_{\rho\eta}$, and it can be nonzero only if $\rho$ dominates $\eta$ in the [dominance order on partitions](../../../../../../dominance-order-on-partitions.md). Since each $\eta$ above has at most two parts and size $n-1$, dominance gives

$$
\rho_1+\rho_2\geq\eta_1+\eta_2=n-1.
$$

Thus $\rho$ has at most two nonzero parts. The [character inner product](../../../../../../character-inner-product.md) measures this constituent multiplicity, so

$$
\boxed{\left\langle\operatorname{Res}_{S_{n-1}}^{S_n}\pi^{(n-k,k)},\chi^\rho\right\rangle=0\quad\text{when }\ell(\rho)\geq3.}
$$

If $k=0$, the original and restricted modules are the [trivial representations](../../../../../../trivial-representation.md), giving the same conclusion. For $n=1$, there is no partition of $n-1=0$ with three parts, so the assertion is vacuous.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 103](../../../paper-103-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
