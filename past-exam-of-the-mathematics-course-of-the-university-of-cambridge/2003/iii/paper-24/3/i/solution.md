<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use $q=e^{2\pi i\tau}$, so $g(iy)=\sum_{n\geq1}b_ne^{-2\pi ny}$. Put $u=\operatorname{Re}s$. For $u>\max\{0,\sigma+1\}$,

$$
\sum_{n\geq1}|b_n|\int_0^\infty e^{-2\pi ny}y^{u-1}\,dy=\Gamma(u)(2\pi)^{-u}\sum_{n\geq1}|b_n|n^{-u}<\infty.
$$

The [Gamma integral](../../../../../../gamma-integral.md) and [absolute convergence](../../../../../../absolute-convergence.md) therefore justify exchanging summation and integration. For every positive integer $n$, substitution $t=2\pi ny$ gives

$$
\int_0^\infty e^{-2\pi ny}y^{s-1}\,dy=(2\pi n)^{-s}\Gamma(s).
$$

Summing these identities proves the [Mellin transform](../../../../../../mellin-transform.md) formula for the [Dirichlet series](../../../../../../dirichlet-series.md):

$$
\boxed{\int_0^\infty g(iy)y^s\frac{dy}{y}=(2\pi)^{-s}\Gamma(s)L(g,s).}
$$

The power of the positive real variable $y$ uses the real logarithm; the initial half-plane stated above is a sufficient one even when $\sigma$ is negative.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
