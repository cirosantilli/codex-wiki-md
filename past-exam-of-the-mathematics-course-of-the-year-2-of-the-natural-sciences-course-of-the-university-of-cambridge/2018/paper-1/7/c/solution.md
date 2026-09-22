<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Expand the exponential in inverse powers of $z$:

$$
g(z)=\sum_{n=0}^\infty\frac{z^{-n}}{n!}-\sum_{n=0}^\infty\frac{z^{2-n}}{n!}
=-z^2-z+\frac12+\sum_{k=1}^\infty\left(\frac1{k!}-\frac1{(k+2)!}\right)z^{-k}.
$$

This is a [Laurent series](../../../../../laurent-series.md), not a [Taylor series](../../../../../taylor-series.md), and converges throughout $0<|z|<\infty$. Every displayed coefficient of a negative power is nonzero, so its principal part has infinitely many terms. Thus

$$
\boxed{z=0\ \text{is an essential singularity}}.
$$

The [residue](../../../../../residue.md) is the coefficient of $z^{-1}$:

$$
\boxed{\operatorname{Res}_{z=0}g=1-\frac1{3!}=\frac56}.
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [7](../../7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
