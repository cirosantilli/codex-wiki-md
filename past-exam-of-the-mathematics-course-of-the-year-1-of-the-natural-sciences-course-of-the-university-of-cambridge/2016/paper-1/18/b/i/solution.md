<h1 id="18/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $m=2$, evaluate the [improper integral](../../../../../../improper-integral.md) directly:

$$
I_{2,n}=\int_0^\infty(1+x)^{-n}dx
=\left[\frac{(1+x)^{1-n}}{1-n}\right]_0^\infty
=\boxed{\frac1{n-1}}.
$$

For $m\geq3$, use [integration by parts](../../../../../../integration-by-parts.md) with $u=x^{m-2}$ and $dv=(1+x)^{-(m+n-2)}dx$. Then $v=-(1+x)^{-(m+n-3)}/(m+n-3)$ and

$$
\begin{aligned}
I_{m,n}
&=\left[-\frac{x^{m-2}}{(m+n-3)(1+x)^{m+n-3}}\right]_0^\infty\\
&\quad+\frac{m-2}{m+n-3}\int_0^\infty\frac{x^{m-3}}{(1+x)^{m+n-3}}dx\\
&=\boxed{\frac{m-2}{m+n-3}I_{m-1,n}}.
\end{aligned}
$$

The boundary term vanishes: at zero $m-2>0$, while at infinity its power is $1-n<0$. The restriction $m\geq3$ belongs to this recurrence step; the separate $m=2$ base case must not be replaced by a formal zero times a divergent $I_{1,n}$.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [18](../../../18.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
