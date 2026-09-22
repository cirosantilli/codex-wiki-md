<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a Gaussian smoothed density contrast, the Press-Schechter factor of two gives the collapsed mass fraction

$$
F(>M)=2\int_{\delta_c}^{\infty}
\frac{d\delta}{\sqrt{2\pi}\sigma}
e^{-\delta^2/(2\sigma^2)}
=\operatorname{erfc}\left(\frac\nu{\sqrt2}\right),
\qquad
\nu=\frac{\delta_c}{\sigma(M)}.
$$

The fraction in the interval $[M,M+dM]$ is $-(dF/dM)dM=(M/\bar\rho)(dn/dM)dM$. Since $d\nu/dM=-\nu\,d\log\sigma/dM$,

$$
\boxed{
\frac{dn}{dM}
=-\sqrt{\frac2\pi}\frac{\bar\rho}{M^2}
\nu e^{-\nu^2/2}\frac{d\log\sigma}{d\log M}}
$$

or, equivalently, the same expression with $|d\log\sigma/d\log M|$. The minus sign is needed because $\sigma(M)$ decreases with $M$; this is the positive [Press-Schechter halo mass function](../../../../../../press-schechter-halo-mass-function.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
