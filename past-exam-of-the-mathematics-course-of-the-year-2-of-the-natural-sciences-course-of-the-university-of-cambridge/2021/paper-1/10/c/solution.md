<h1 id="10/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Move the differential terms to the left in the sign convention of part (a). Then $\widetilde a=1+x$, $\widetilde c=0$, and $\widetilde b=(3+2x)-\widetilde a'=2(1+x)$. The [integrating factor](../../../../../integrating-factor.md) is therefore $w=e^{2x}$, up to a positive constant. The [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md) is

$$
\boxed{-\frac d{dx}\left[(1+x)e^{2x}y'\right]=\lambda e^{2x}y,\qquad y(0)=0,\quad y'(1)=0.}
$$

The trial $y=xe^{-x}$ is admissible because $y(0)=0$ and $y'=e^{-x}(1-x)$ vanishes at one. Its [Rayleigh quotient](../../../../../rayleigh-quotient.md) has numerator

$$
F[y]=\int_0^1(1+x)(1-x)^2dx=\int_0^1(1-x-x^2+x^3)dx=\frac5{12}
$$

and denominator

$$
G[y]=\int_0^1x^2dx=\frac13.
$$

Consequently the [Rayleigh-Ritz variational principle](../../../../../rayleigh-ritz-variational-principle.md) gives

$$
\boxed{\lambda_{\min}\leq\frac54.}
$$

The numerator is positive for every nonzero admissible function, so the lowest [eigenvalue](../../../../../eigenvalue.md) is positive. The trial is not an exact [eigenfunction](../../../../../eigenfunction.md): substituting it would require $x^2+2x-1=\lambda x$ for every $x$. Thus the upper inequality is actually strict. This example underlies the [exponential-polynomial trial space for a mixed Sturm-Liouville problem](../../../../../exponential-polynomial-trial-space-for-a-mixed-sturm-liouville-problem.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
