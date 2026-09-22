<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $p(x)=x^3-x$. Since $A$ is multiplication by $p$, its spectral projection is multiplication by $\mathbf1_{p^{-1}(S)}$. Hence

$$
\mu_{f,g}(S)=\int_{p^{-1}(S)}f(x)\overline{g(x)}\,dx.
$$

Split $[-1,1]$ at the two critical points $\pm1/\sqrt3$. On each resulting interval, $p$ is monotone, so one-dimensional change of variables shows that the measure is absolutely continuous. For almost every $t$,

$$
\boxed{
\frac{d\mu_{f,g}}{dt}(t)
=\sum_{\substack{x\in[-1,1]\\x^3-x=t}}
\frac{f(x)\overline{g(x)}}{|3x^2-1|}}.
$$

The density vanishes outside

$$
\left[-\frac{2}{3\sqrt3},\frac{2}{3\sqrt3}\right].
$$

Its inverse-square-root singularities at the two critical values are locally integrable, so they do not create singular spectral measure.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 358](../../../paper-358-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
