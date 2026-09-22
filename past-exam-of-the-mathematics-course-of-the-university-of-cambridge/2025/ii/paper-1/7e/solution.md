<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

The [Cauchy principal value](../../../../../cauchy-principal-value.md) deletes symmetric intervals around the real poles $-1$ and $1$ and takes a symmetric [limit](../../../../../limit-of-a-function.md) at infinity:

$$
\operatorname{PV}\int_{-\infty}^{\infty}f(x)dx
=\lim_{R\to\infty,\ \varepsilon\downarrow0}
\left(\int_{-R}^{-1-\varepsilon}+\int_{-1+\varepsilon}^{1-\varepsilon}+\int_{1+\varepsilon}^{R}\right)f(x)dx.
$$

The integrand is even. The standard [principal-value beta integral](../../../../../principal-value-beta-integral.md) gives

$$
\operatorname{PV}\int_0^\infty\frac{x^{s-1}}{1-x^a}dx=\frac\pi a\cot\frac{\pi s}{a}.
$$

Taking $s=1$, $a=6$, and reversing the denominator,

$$
\operatorname{PV}\int_{-\infty}^{\infty}\frac{dx}{x^6-1}
=-\frac{2\pi}{6}\cot\frac\pi6=-\frac\pi{\sqrt3}.
$$

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
