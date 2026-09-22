<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Expand both sides through second order as $\epsilon\to0$, holding $X,Y$ fixed. The product is

$$
e^{\epsilon X}e^{\epsilon Y}=I+\epsilon(X+Y)+\epsilon^2\left(\frac{X^2}{2}+XY+\frac{Y^2}{2}\right)+O(\epsilon^3).
$$

Put $Z=\epsilon(X+Y)+\epsilon^2[X,Y]/2$. Its exponential is

$$
\begin{aligned}
e^Z&=I+\epsilon(X+Y)+\frac{\epsilon^2}{2}\{[X,Y]+(X+Y)^2\}+O(\epsilon^3)\\
&=I+\epsilon(X+Y)+\epsilon^2\left(\frac{X^2}{2}+XY+\frac{Y^2}{2}\right)+O(\epsilon^3).
\end{aligned}
$$

Thus

$$
\boxed{e^{\epsilon X}e^{\epsilon Y}=e^{\epsilon X+\epsilon Y+\epsilon^2[X,Y]/2}+O(\epsilon^3).}
$$

This is the quadratic part of the [Baker--Campbell--Hausdorff formula](../../../../../baker-campbell-hausdorff-formula.md). The remainder estimate is in any fixed finite-dimensional [matrix](../../../../../matrix.md) [norm](../../../../../norm.md), and is an asymptotic statement rather than an exact formula for arbitrary finite $\epsilon$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
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
