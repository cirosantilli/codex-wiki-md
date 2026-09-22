<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $G(k)=\widetilde g(k)$. Since $g'=-xg$, [differentiation](../../../../../differentiation.md) under the [Fourier transform](../../../../../fourier-transform-split.md) integral and [integration by parts](../../../../../integration-by-parts.md) give

$$
G'(k)=-i\,\widetilde{xg}(k)=i\,\widetilde{g'}(k)=i(ik)G(k)=-kG(k).
$$

Thus $G(k)=G(0)e^{-k^2/2}$. The [Gaussian integral](../../../../../gaussian-integral.md) gives $G(0)=\sqrt{2\pi}$, proving the [Fourier transform of a Gaussian](../../../../../fourier-transform-of-a-gaussian.md) formula

$$
\boxed{\widetilde g(k)=\sqrt{2\pi}\,e^{-k^2/2},\qquad c=\sqrt{2\pi}.}
$$

For the higher [derivatives](../../../../../derivative.md), start with $r_0=1$. If $g^{(m)}=r_mg$, the [product rule](../../../../../product-rule.md) gives

$$
g^{(m+1)}=(r_m'-xr_m)g,\qquad\boxed{r_{m+1}=r_m'-xr_m.}
$$

If $r_m$ has degree $m$ and leading coefficient $(-1)^m$, the recurrence gives degree $m+1$ and leading coefficient $(-1)^{m+1}$. Induction proves the assertion for every $m$. These polynomials are $r_m=(-1)^m\operatorname{He}_m$, where $\operatorname{He}_m$ is the [Probabilists' Hermite polynomial](../../../../../probabilists-hermite-polynomial.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
