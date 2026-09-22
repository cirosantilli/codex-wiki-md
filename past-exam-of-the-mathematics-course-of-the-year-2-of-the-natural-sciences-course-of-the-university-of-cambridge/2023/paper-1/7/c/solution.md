<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Multiply the exponential [power series](../../../../../power-series.md) by the two prefactors:

$$
f(z)=\sum_{n=0}^{\infty}\frac{z^{1-n}}{n!}+\sum_{n=0}^{\infty}\frac{z^{-1-n}}{n!}.
$$

Collecting powers yields the [Laurent series](../../../../../laurent-series.md)

$$
\boxed{f(z)=z+1+\sum_{m=1}^{\infty}\left(\frac1{(m+1)!}+\frac1{(m-1)!}\right)z^{-m},\qquad0<|z|<\infty.}
$$

Its first terms are $z+1+3/(2z)+7/(6z^2)+13/(24z^3)+\cdots$. Infinitely many negative-power coefficients are nonzero, so $\boxed{z=0\text{ is an essential singularity}}$. The [residue](../../../../../residue.md) is the coefficient of $z^{-1}$:

$$
\boxed{\operatorname{Res}_{z=0}f=\frac1{2!}+\frac1{0!}=\frac32.}
$$

The phrase "power series" here refers to a [Laurent series](../../../../../laurent-series.md); no ordinary [Taylor series](../../../../../taylor-series.md) about an [essential singularity](../../../../../essential-singularity.md) exists.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [7](../../7.md)
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
