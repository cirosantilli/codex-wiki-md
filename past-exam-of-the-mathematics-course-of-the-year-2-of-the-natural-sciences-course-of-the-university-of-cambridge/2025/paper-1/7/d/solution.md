<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $w=z-1$ and $a=1-i$. [Partial fraction decomposition](../../../../../partial-fraction-decomposition.md) gives

$$
\frac1{(z-i)(z+3)}=\frac1{3+i}\left(\frac1{w+a}-\frac1{w+4}\right).
$$

Both terms admit a [geometric series](../../../../../geometric-series.md) at $w=0$. The local [Laurent series](../../../../../laurent-series.md) is actually a [Taylor series](../../../../../taylor-series.md), since the center is regular:

$$
\boxed{\frac1{(z-i)(z+3)}=\frac1{3+i}\sum_{m=0}^{\infty}(-1)^m\left[\frac1{(1-i)^{m+1}}-\frac1{4^{m+1}}\right](z-1)^m,\quad |z-1|<\sqrt2.}
$$

The nearest [pole](../../../../../pole.md) is $z=i$, a distance $|1-i|=\sqrt2$ from the center; the other [pole](../../../../../pole.md) is at distance $4$. Thus the requested local [radius of convergence](../../../../../radius-of-convergence.md) is $\boxed{R=\sqrt2}$.

For completeness, specifying a [Laurent series](../../../../../laurent-series.md) without a region can also mean either of the other maximal annuli. Expanding the first fraction in inverse powers and the second in positive powers gives

$$
\frac1{3+i}\left[\sum_{m=0}^{\infty}\frac{(-a)^m}{w^{m+1}}-\sum_{m=0}^{\infty}\frac{(-1)^mw^m}{4^{m+1}}\right],\qquad \sqrt2<|w|<4.
$$

Expanding both fractions in inverse powers instead gives

$$
\frac1{3+i}\sum_{m=0}^{\infty}\frac{(-a)^m-(-4)^m}{w^{m+1}},\qquad |w|>4.
$$

These are different [Laurent series](../../../../../laurent-series.md) on different annuli, rather than extensions of the local [Taylor series](../../../../../taylor-series.md) beyond its [radius of convergence](../../../../../radius-of-convergence.md).

## ↑ Ancestors (13)

1. [D](../d.md)
2. [7](../../7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
