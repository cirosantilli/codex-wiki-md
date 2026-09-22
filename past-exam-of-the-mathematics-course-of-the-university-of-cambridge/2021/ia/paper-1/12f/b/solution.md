<h1 id="12f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $w=e^z$. Then

$$
\sum_{n=0}^\infty b_ne^{nz}
=\sum_{n=0}^\infty b_nw^n.
$$

The hypothesis that convergence and divergence both occur implies that this ordinary power series has a radius $R$ with $0<R<\infty$. Since $|w|=e^{\operatorname{Re}z}$, the [half-plane of convergence of an exponential power series](../../../../../../half-plane-of-convergence-of-an-exponential-power-series.md) is determined by

$$
\boxed{S=\log R}:
$$

the series converges for $\operatorname{Re}z<S$ and diverges for $\operatorname{Re}z>S$.

For the specified series,

$$
\frac{2^ne^{inz}}{(n+1)^2}
=\frac{(2e^{iz})^n}{(n+1)^2}.
$$

Writing $z=x+iy$ gives $|2e^{iz}|=2e^{-y}$. The series converges absolutely when $y>\log2$ and diverges by the term test when $y<\log2$. On $y=\log2$, its absolute values are $(n+1)^{-2}$, so it still converges absolutely. Therefore the exact convergence set is

$$
\boxed{\{z\in\mathbb C:\operatorname{Im}z\geq\log2\}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12F](../../12f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
