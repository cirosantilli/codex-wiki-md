<h1 id="21f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $x\in X$, choose $x_m\in D$ with $x_m\to x$ and define

$$
\widetilde Tx=\lim_{m\to\infty}Tx_m.
$$

The sequence on the right is Cauchy because

$$
\lVert Tx_m-Tx_l\rVert\leq\lVert T\rVert\lVert x_m-x_l\rVert,
$$

and it converges because $Y$ is complete. The same estimate shows that the limit is independent of the approximating sequence, is linear, and satisfies

$$
\lVert\widetilde Tx\rVert\leq\lVert T\rVert\lVert x\rVert.
$$

Its norm is at most $\lVert T\rVert$, while restriction to $D$ gives the reverse inequality, so

$$
\boxed{\lVert\widetilde T\rVert=\lVert T\rVert.}
$$

Any two continuous extensions agree on the dense set $D$ and hence everywhere, proving uniqueness. This is the [extension of a bounded linear operator from a dense subspace](../../../../../../extension-of-a-bounded-linear-operator-from-a-dense-subspace.md).

Completeness of $X$ was never used, so the result remains true when $X$ is incomplete. Completeness of $Y$ is essential. For example, with $D=c_{00}\subset X=\ell^2$, let the codomain be the incomplete normed space $Y=c_{00}$ with the $\ell^2$ norm and let $T$ be the identity. An extension would have to send every limit in $\ell^2$ to itself and therefore could not take values in $c_{00}$. This is the [failure of dense-subspace extension into an incomplete codomain](../../../../../../failure-of-dense-subspace-extension-into-an-incomplete-codomain.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [21F](../../21f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
