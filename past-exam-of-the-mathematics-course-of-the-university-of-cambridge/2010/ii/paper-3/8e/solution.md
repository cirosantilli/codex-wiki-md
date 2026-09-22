<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

For $x>0$, differentiate the absolutely convergent [geometric series](../../../../../geometric-series.md) to obtain

$$
(1-e^{-x})^{-2}=\sum_{j=0}^\infty(j+1)e^{-jx},\qquad
(e^x-1)^{-2}=\sum_{m=2}^\infty(m-1)e^{-mx}.
$$

If $\sigma=\Re z>1$, the sum of [integrals](../../../../../integral.md) of absolute values is

$$
\sum_{m\ge2}(m-1)\int_0^\infty x^\sigma e^{-mx}\,dx
=\Gamma(\sigma+1)\sum_{m\ge2}\frac{m-1}{m^{\sigma+1}}<\infty.
$$

Thus [Fubini theorem](../../../../../fubini-s-theorem.md) permits termwise integration, even for complex $z$. The substitution $u=mx$ and the definition of the [Gamma function](../../../../../gamma-function.md) give

$$
\boxed{\int_0^\infty\frac{x^z}{(e^x-1)^2}\,dx
=\Gamma(z+1)\sum_{m\ge2}\left(m^{-z}-m^{-z-1}\right)
=\Gamma(z+1)\bigl(\zeta(z)-\zeta(z+1)\bigr).}
$$

The missing $m=1$ terms cancel in the difference of the two [Riemann zeta functions](../../../../../riemann-zeta-function.md).

## ↑ Ancestors (10)

1. [8E](../8e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
