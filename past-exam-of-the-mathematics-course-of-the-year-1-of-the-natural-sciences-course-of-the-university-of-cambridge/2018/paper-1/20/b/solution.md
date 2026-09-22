<h1 id="20/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The stated derivative formula needs a domain qualification. The original PDF calls $\alpha$ real, but the integral is even in $\alpha$; its derivative therefore cannot equal the printed positive expression on both sides of zero.

First take $\alpha>0$. The [improper integral](../../../../../improper-integral.md) converges, with an $O(x^2)$ integrand near zero and $O(\ln x/x^2)$ decay at infinity. On compact positive parameter intervals, an integrable bound also justifies [differentiation under the integral sign](../../../../../differentiation-under-the-integral-sign.md):

$$
E'(\alpha)=\int_0^\infty\frac{2\alpha x^2}{(1+\alpha^2x^2)(1+x^2)}\,dx.
$$

For $\alpha\ne1$, the [partial fraction decomposition](../../../../../partial-fraction-decomposition.md) is

$$
\frac{x^2}{(1+\alpha^2x^2)(1+x^2)}
=\frac1{\alpha^2-1}\left(\frac1{1+x^2}-\frac1{1+\alpha^2x^2}\right).
$$

Integrating the rational functions gives

$$
E'(\alpha)=\frac{2\alpha}{\alpha^2-1}\left(\frac\pi2-\frac\pi{2\alpha}\right)
=\boxed{\frac\pi{1+\alpha}\quad(\alpha>0).}
$$

At $\alpha=1$, the same result follows by continuity, or directly from $2\int_0^\infty x^2/(1+x^2)^2\,dx=\pi/2$.

Integrating gives $E(\alpha)=\pi\ln(1+\alpha)+C$ on the positive half-line. To fix $C$, take $\alpha\to0^+$: for $0\le\alpha\le1$ the integrand is bounded by $\ln(1+x^2)/(1+x^2)$, an integrable function. The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) gives $E(\alpha)\to E(0)=0$, so $C=0$. Evenness then extends the [logarithmic parameter integral with Cauchy weight](../../../../../logarithmic-parameter-integral-with-cauchy-weight.md) to its full stated domain:

$$
\boxed{E(\alpha)=\pi\ln(1+|\alpha|)\quad(\alpha\in\mathbb R).}
$$

For negative $\alpha$, the derivative is $-\pi/(1-\alpha)$. At zero the right and left [derivatives](../../../../../derivative.md) are $\pi$ and $-\pi$, so $E$ is not [differentiable](../../../../../differentiable-function.md) there. The pointwise derivative of the integrand at zero is zero, but interchanging it with the infinite [integral](../../../../../integral-split.md) at that parameter is invalid. Finally, substituting $\alpha=1$ gives the requested special value

$$
\boxed{\int_0^\infty\frac{\ln(1+x^2)}{1+x^2}\,dx=\pi\ln2.}
$$

## ↑ Ancestors (13)

1. [B](../b.md)
2. [20](../../20.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
