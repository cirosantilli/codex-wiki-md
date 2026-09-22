<h1 id="22h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Given $x\in\ell^p$, choose a sequence $x^{(m)}\in F$ with $x^{(m)}\to x$, which is possible by part (a). The bound gives

$$
\lVert Tx^{(m)}-Tx^{(l)}\rVert_p
\leq C\lVert x^{(m)}-x^{(l)}\rVert_p,
$$

so $(Tx^{(m)})$ is a [Cauchy sequence](../../../../../../cauchy-sequence.md). Since $\ell^p$ is a [Banach space](../../../../../../banach-space-split.md), it converges. Define

$$
\widetilde Tx=\lim_{m\to\infty}Tx^{(m)}.
$$

The same estimate shows that this limit does not depend on the approximating sequence. Passing to the limit proves linearity and

$$
\lVert\widetilde Tx\rVert_p\leq C\lVert x\rVert_p,
$$

so $\lVert\widetilde T\rVert\leq C$. It agrees with $T$ on $F$. If two bounded extensions existed, their difference would vanish on the dense subspace $F$ and, by continuity, on its closure $\ell^p$. Thus the extension is unique. This is the [extension of a bounded linear operator from a dense subspace](../../../../../../extension-of-a-bounded-linear-operator-from-a-dense-subspace.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [22H](../../22h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
