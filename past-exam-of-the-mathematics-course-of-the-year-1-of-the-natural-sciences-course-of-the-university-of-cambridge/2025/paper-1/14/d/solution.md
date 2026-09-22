<h1 id="14/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Keep $a$ general initially, since the final part does not explicitly fix it. For $-h\leq y\leq h$, where $h=\pi/6$, the [cumulative distribution function](../../../../../cumulative-distribution-function.md) is

$$
F_X(y)=\int_{-h}^y(ax+\cos x)\,dx=\frac a2(y^2-h^2)+\sin y+\frac12.
$$

The [normalization constant](../../../../../normalizing-constant.md) in the [probability density function](../../../../../probability-density-function.md) of $Y$ must be

$$
M=\int_{-h}^h F_X(y)\,dy=\frac a2\left(\frac{2h^3}{3}-2h^3\right)+h=\boxed{h-\frac{2ah^3}{3}=\frac\pi6-\frac{a\pi^3}{324}.}
$$

Equivalently, the [integrated cumulative distribution function on a bounded interval](../../../../../integrated-cumulative-distribution-function-on-a-bounded-interval.md) identity gives $M=h-\mathbb E[X]$. If the assumption $a=0$ from part (c) is retained, the requested special case is $\boxed{M=\pi/6}$. For the value $a=1$ in part (b), it is $M=\pi/6-\pi^3/324$.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [14](../../14.md)
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
