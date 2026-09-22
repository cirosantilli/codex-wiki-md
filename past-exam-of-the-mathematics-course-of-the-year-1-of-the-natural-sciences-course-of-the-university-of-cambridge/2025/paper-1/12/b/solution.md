<h1 id="12/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $F(x)=\ln(e^{ax}-b)$. Direct [differentiation](../../../../../differentiation.md), using the [chain rule](../../../../../chain-rule.md), gives

$$
F'(x)=\frac{ae^{ax}}{e^{ax}-b},\qquad F''(x)=-\frac{a^2be^{ax}}{(e^{ax}-b)^2}.
$$

The stated parameter restrictions ensure that the [logarithm](../../../../../logarithm.md) is defined near $x=1$, and that $F'(1)>0$ and $F''(1)<0$. With $h=x-1$, the [Taylor series](../../../../../taylor-series.md) begins

$$
F(1+h)=\ln(e^a-b)+\frac{ae^a}{e^a-b}h-\frac{a^2be^a}{2(e^a-b)^2}h^2+O(h^3).
$$

If $e^a-b\ne1$, the constant term is nonzero, and the first two nonzero terms are

$$
\boxed{\ln(e^a-b)+\frac{ae^a}{e^a-b}(x-1)+O((x-1)^2).}
$$

This covers both $a>\ln(1+b)$ and $0<a<\ln(1+b)$; the constant term is respectively positive or negative.

If $a=\ln(1+b)$, which is possible precisely with $0<a<\ln2$ and $b=e^a-1$, the constant term vanishes. The first two nonzero terms are then

$$
\boxed{a(1+b)(x-1)-\frac{a^2b(1+b)}2(x-1)^2+O((x-1)^3).}
$$

No further case is needed, since the linear and quadratic coefficients cannot vanish under the given restrictions. All remainders use [Big O notation](../../../../../big-o-notation.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [12](../../12.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
