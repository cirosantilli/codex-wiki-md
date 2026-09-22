<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The real [vector space](../../../../../../vector-space-split.md) of [symmetric matrices](../../../../../../symmetric-matrix.md) has [dimension](../../../../../../dimension-vector-space.md) $N=n(n+1)/2$. By the [conic Carathéodory theorem](../../../../../../conic-caratheodory-theorem.md), every member of $C_0$ is a [conic combination](../../../../../../conic-combination.md) of at most $N$ generators. Absorb each nonnegative [coefficient](../../../../../../coefficient.md) into its [vector](../../../../../../vector.md) through $\lambda xx^T=(\sqrt\lambda x)(\sqrt\lambda x)^T$.

If $B_\ell\in C_0$ converges to $B$, write, padding with zero [vectors](../../../../../../vector.md) if necessary,

$$
B_\ell=\sum_{j=1}^N x_{\ell j}x_{\ell j}^T,\qquad x_{\ell j}\geq0.
$$

The [matrix trace](../../../../../../matrix-trace.md) satisfies

$$
\operatorname{tr}B_\ell=\sum_{j=1}^N\|x_{\ell j}\|_2^2.
$$

The left side is bounded because $B_\ell$ converges. Thus the finite tuple $(x_{\ell1},\ldots,x_{\ell N})$ is bounded. The [Bolzano-Weierstrass theorem](../../../../../../bolzano-weierstrass-theorem.md) gives a subsequence on which every [vector](../../../../../../vector.md) converges, say $x_{\ell j}\to x_j\geq0$. [Continuity](../../../../../../continuous-function.md) of the [outer product](../../../../../../outer-product.md) now gives $B=\sum_{j=1}^N x_jx_j^T\in C_0$. Hence

$$
\boxed{C_0\text{ is closed},\qquad K^*=C=C_0}.
$$

This proves [closedness of the completely positive cone](../../../../../../closedness-of-the-completely-positive-cone.md). The uniform bound on the number of factors and the [matrix trace](../../../../../../matrix-trace.md) bound are both essential: an arbitrary [conic hull](../../../../../../conic-hull.md) of a closed generating set need not be closed.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
