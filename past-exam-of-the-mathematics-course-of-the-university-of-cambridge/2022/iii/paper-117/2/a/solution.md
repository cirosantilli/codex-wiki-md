<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Mellin transform](../../../../../../mellin-transform.md) of $F$ is

$$
\widetilde F(s)=\int_0^\infty F(x)x^{s-1}\,dx.
$$

Because the support is a compact subset of $(0,\infty)$, the integral defines an [entire function](../../../../../../entire-function.md) of $s$. The [Mellin inversion formula](../../../../../../mellin-inversion-theorem.md) says that, for every real $\sigma$ and every $y>0$,

$$
F(y)=\frac1{2\pi i}\int_{\sigma-i\infty}^{\sigma+i\infty}
\widetilde F(s)y^{-s}\,ds.
$$

Apply this with $y=n/X$ and initially $\sigma=2$. Absolute convergence of the [Dirichlet series](../../../../../../dirichlet-series.md) for the [logarithmic derivative](../../../../../../logarithmic-derivative.md) permits interchange of sum and integral, giving

$$
\sum_{n\geq1}\Lambda(n)F(n/X)
=\frac1{2\pi i}\int_{(2)}
-\frac{\zeta'(s)}{\zeta(s)}\widetilde F(s)X^s\,ds.
$$

Truncate at height $T=(\log X)^A$, where $A$ is a sufficiently large fixed constant. The assumed bound on $\widetilde F$ makes the discarded tails smaller than the required error. The classical [zero-free region of the Riemann zeta function](../../../../../../zero-free-region-of-the-riemann-zeta-function.md) and the standard bound $\zeta'(s)/\zeta(s)\ll(\log(|t|+3))^{O(1)}$ there allow the truncated contour to move to

$$
\sigma=1-\frac{c_0}{\log T}
=1-\frac{c}{\log\log X}.
$$

The only singularity crossed is the simple pole of $-\zeta'/\zeta$ at $s=1$, whose residue is $1$. Its contribution is

$$
C_{F,X}=X\widetilde F(1)=X\int_0^\infty F(u)\,du.
$$

On the new contour, $|X^s|=X^{1-c/\log\log X}$; the zeta bounds, contour length, and exponential decay of $\widetilde F$ absorb into a slight decrease of $c$. Therefore

$$
\boxed{
\sum_{n\geq1}\Lambda(n)F(n/X)
=X\int_0^\infty F(u)\,du
+O\left(X^{1-c/\log\log X}\right).}
$$

This is the [smoothed prime number theorem from a zero-free region](../../../../../../smoothed-prime-number-theorem-from-a-zero-free-region.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 117](../../../paper-117-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
