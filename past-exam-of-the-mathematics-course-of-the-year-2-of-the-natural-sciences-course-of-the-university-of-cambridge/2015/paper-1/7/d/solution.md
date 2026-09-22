<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

[Partial fraction decomposition](../../../../../partial-fraction-decomposition.md) give $h(z)=1/(z-i)+1/(z+i)$. Let $w=z-1$. Each fraction has a geometric expansion, so

$$
\boxed{h(z)=\sum_{j=0}^\infty(-1)^j\left[\frac1{(1-i)^{j+1}}+\frac1{(1+i)^{j+1}}\right](z-1)^j.}
$$

Equivalently, its coefficient is $(-1)^j2^{(1-j)/2}\cos((j+1)\pi/4)$. The first terms are

$$
h(z)=1-\frac12w^2+\frac12w^3-\frac14w^4+O(w^6).
$$

The linear and fifth-order coefficients vanish. Both [geometric series](../../../../../geometric-series.md) converge for $|w|<\sqrt2$, and $h$ has genuine simple poles at $z=\pm i$, each distance $\sqrt2$ from the centre. Thus the [Taylor series](../../../../../taylor-series.md) has

$$
\boxed{R=\sqrt2.}
$$

## ↑ Ancestors (13)

1. [D](../d.md)
2. [7](../../7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
