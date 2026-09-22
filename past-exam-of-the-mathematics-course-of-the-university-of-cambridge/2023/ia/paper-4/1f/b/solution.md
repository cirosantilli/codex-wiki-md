<h1 id="1f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

By part (a), there are $A_{n+1}$ permutations of each alternating type. In an up-down permutation the maximum $n+1$ can occur only at a peak, while in a down-up permutation it can occur only at the complementary positions. Thus, after combining the two types, each possible number $k$ of entries to the left of the maximum occurs once.

Choose those $k$ labels in $\binom nk$ ways. The entries on the two sides must independently alternate, and after order-preserving relabelling can be chosen in $A_k$ and $A_{n-k}$ ways. This [alternating-permutation convolution](../../../../../../alternating-permutation-convolution.md) is

$$
\boxed{2A_{n+1}=\sum_{k=0}^n\binom nkA_kA_{n-k}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1F](../../1f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
