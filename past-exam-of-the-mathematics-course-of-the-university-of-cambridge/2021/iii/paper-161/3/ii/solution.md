<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Consider the degree-$n$ polynomial

$$
f(x_1,\ldots,x_n)=\prod_{i=1}^n\left(\sum_{j=1}^na_{ij}x_j-b_i\right).
$$

To form the square-free monomial $x_1\cdots x_n$, one must choose each variable exactly once from the $n$ factors. Such choices are indexed by permutations, so

$$
[x_1\cdots x_n]f
=\sum_{\sigma\in S_n}\prod_{i=1}^na_{i,\sigma(i)}
=\operatorname{perm}A.
$$

This coefficient is nonzero by hypothesis. Apply the [Combinatorial Nullstellensatz](../../../../../../combinatorial-nullstellensatz.md) with every $d_i=1$ and the given two-element sets $S_i$. It supplies $x\in\prod_iS_i$ with $f(x)\ne0$. Every factor is then nonzero, so

$$
(Ax)_i\ne b_i
$$

for all $i$. This is [coordinate avoidance from a nonzero permanent](../../../../../../coordinate-avoidance-from-a-nonzero-permanent.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 161](../../../paper-161-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
