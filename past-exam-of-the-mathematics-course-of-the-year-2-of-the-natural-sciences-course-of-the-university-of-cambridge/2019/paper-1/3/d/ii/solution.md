<h1 id="3/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The original PDF shows $x^2$ in the nonzero source branch. Inserting that source into $G_0$ gives, for $x<1/2$,

$$
y_p(x)=\frac x2\int_{1/2}^1(z^2-1)\,dz=-\frac{5x}{48}.
$$

For $x\geq1/2$, split the integral at $z=x$:

$$
\begin{aligned}
y_p(x)&=\frac{x^3-x}{2}\int_{1/2}^x1\,dz+\frac x2\int_x^1(z^2-1)\,dz\\
&=\frac{x^4}{3}-\frac{x^3}{4}-\frac{x}{12}.
\end{aligned}
$$

Because of the homogeneous freedom established in part (i), the full answer to the stated endpoint problem is

$$
\boxed{y(x)=\begin{cases}-5x/48,&0\leq x<1/2,\\x^4/3-x^3/4-x/12,&1/2\leq x\leq1,\end{cases}+C(x^3-x),\qquad C\in\mathbb R.}
$$

At the interface, both branches have value $-5/96$ and [derivative](../../../../../../derivative.md) $-5/48$, so no extra delta or delta [derivative](../../../../../../derivative.md) occurs there. Direct substitution gives zero source on the left and $x^2$ on the right; the endpoint values are zero for every $C$. If the extra condition $y/x\to0$ is imposed, it selects $C=-5/48$, but that is additional information absent from the printed question.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
