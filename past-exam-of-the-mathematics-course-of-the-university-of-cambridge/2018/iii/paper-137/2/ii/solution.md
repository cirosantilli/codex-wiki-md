<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Extend each [Dirichlet character](../../../../../../dirichlet-character.md) periodically to all integers by setting $\chi(n)=0$ when $\gcd(n,N)>1$. Its [Dirichlet L-function](../../../../../../dirichlet-l-function.md) is initially the absolutely convergent [Dirichlet series](../../../../../../dirichlet-series.md)

$$
\boxed{L(\chi,s)=\sum_{n\geq1}\frac{\chi(n)}{n^s}
\quad(\operatorname{Re}s>1).}
$$

The group $(\mathbb Z/N\mathbb Z)^\times$ has $\varphi(N)$ elements. Part (i) gives, for every integer $n$, including nonunits,

$$
\sum_{\chi\in\widehat G}\chi(a)^{-1}\chi(n)
=\varphi(N)\,\mathbf1_{n\equiv a\bmod N}.
$$

For a nonunit both sides are zero, because the fixed class $a$ is a unit. Interchanging the finite character sum and the absolutely convergent [Dirichlet series](../../../../../../dirichlet-series.md) therefore proves

$$
\boxed{\sum_{\chi\in\widehat G}\chi(a)^{-1}L(\chi,s)
=\varphi(N)\sum_{n\geq1\atop n\equiv a\bmod N}n^{-s}
\quad(\operatorname{Re}s>1).}
$$

This is [Orthogonality of Dirichlet characters](../../../../../../orthogonality-of-dirichlet-characters.md) applied to a residue-class indicator. Any meromorphic continuations of the two sides agree by uniqueness of [analytic continuation](../../../../../../analytic-continuation.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
