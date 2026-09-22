<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

It suffices to handle one [single-box up-move](../../../../../../single-box-up-move.md), and then use the chain already constructed. Suppose the affected row sizes are $a=\lambda_i$ and $b=\lambda_j$, $i<j$. Since $\lambda$ is a [partition of an integer](../../../../../../partition-of-an-integer.md), $a\geq b\geq1$. Put $N=a+b$. Over the [complex numbers](../../../../../../complex-number.md), the [two-row Young permutation module decomposition](../../../../../../two-row-young-permutation-module-decomposition.md) gives

$$
M^{(a,b)}\cong\bigoplus_{r=0}^b V^{(N-r,r)},\qquad
M^{(a+1,b-1)}\cong\bigoplus_{r=0}^{b-1}V^{(N-r,r)}.
$$

A zero second row is omitted. Therefore

$$
M^{(a,b)}\cong M^{(a+1,b-1)}\oplus V^{(a,b)}.
$$

Let $K$ be the product of the symmetric groups of the unaffected rows and the symmetric group $S_N$ on the union of the affected rows. The two relevant [Young subgroups](../../../../../../young-subgroup.md) lie in $K$. Transitivity of [induced representations](../../../../../../induced-representation.md) expresses $M^\lambda$ and $M^\nu$ by inducing the preceding two-row modules, tensored with the [trivial representations](../../../../../../trivial-representation.md) of the unaffected factors, from $K$ to $S_n$. Induction preserves this [direct sum](../../../../../../direct-sum.md), so

$$
M^\lambda\cong M^\nu\oplus L_{\lambda,\nu}
$$

for an actual [group representation](../../../../../../group-representation.md) $L_{\lambda,\nu}$, not merely a difference of characters. Iterate along the chain and take the [direct sum](../../../../../../direct-sum.md) of the induced complements. The resulting complement can be realized as an [invariant subspace](../../../../../../invariant-subspace.md) of $M^\lambda$, either through these isomorphisms or by [Maschke's theorem](../../../../../../maschke-s-theorem.md). Thus

$$
\boxed{M^\lambda\cong M^\mu\oplus L_{\lambda,\mu}.}
$$

If $\lambda=\mu$, use the zero complement. The characteristic-zero hypothesis is essential to this use of the irreducible two-row decomposition.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 103](../../../paper-103-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
