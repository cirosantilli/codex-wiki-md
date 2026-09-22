<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Set $w=z-1$. [Partial fraction decomposition](../../../../../partial-fraction-decomposition.md) gives

$$
\frac{2z}{z^2+1}=\frac1{z-i}+\frac1{z+i}=\frac1{1-i+w}+\frac1{1+i+w}.
$$

Expand both terms as [geometric series](../../../../../geometric-series.md):

$$
f(z)=\sum_{n=0}^{\infty}(-1)^n\left[(1-i)^{-n-1}+(1+i)^{-n-1}\right]w^n.
$$

The two bracketed terms are complex conjugates. Using $1\pm i=\sqrt2e^{\pm i\pi/4}$ produces the required real coefficients:

$$
\boxed{f(z)=\sum_{n=0}^{\infty}(-1)^n2^{(1-n)/2}\cos\left(\frac{(n+1)\pi}{4}\right)(z-1)^n.}
$$

The initial terms are $1-\tfrac12w^2+\tfrac12w^3-\tfrac14w^4+\cdots$. The nearest singularities are the [simple poles](../../../../../simple-pole.md) $z=\pm i$, both at distance $\sqrt2$ from the center. Hence the [Taylor series](../../../../../taylor-series.md) has

$$
\boxed{R=\sqrt2,\qquad|z-1|<\sqrt2.}
$$

## ↑ Ancestors (13)

1. [D](../d.md)
2. [7](../../7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
