<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Identify the additive group $G$ with the finite field $\mathbb F_q$, where $q=p^\gamma$. The sets $A$ and $B$ each have size $k<p$, and the field has odd characteristic. The [Snevily matching theorem for an elementary abelian group](../../../../../../snevily-matching-theorem-for-an-elementary-abelian-group.md) states precisely that for two $k$-element subsets of the additive group of such a field, there is a bijection $\pi:A\to B$ for which the sums $a+\pi(a)$ are pairwise distinct.

For context, its polynomial proof antisymmetrizes the Vandermonde polynomial

$$
\prod_{i<j}\bigl((a_i+x_i)-(a_j+x_j)\bigr)
$$

over all orderings of $B$. The coefficient furnished by the [Dyson constant-term identity](../../../../../../dyson-constant-term-identity.md) is a nonzero multiple of $k!$; it cannot vanish because $k<p$. Therefore at least one ordering $(b_1,\ldots,b_k)$ makes the Vandermonde product nonzero, which says exactly that

$$
\boxed{a_1+b_1,\ldots,a_k+b_k\text{ are pairwise distinct}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
