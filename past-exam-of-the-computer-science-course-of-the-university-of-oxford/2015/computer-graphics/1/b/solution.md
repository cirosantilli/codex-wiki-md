<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

By exchanging axes, reversing endpoint order and reflecting coordinate signs where necessary, reduce a general [line segment](../../../../../line-segment.md) to the first octant:

$$
\Delta x=x_1-x_0>0,\qquad 0\leq\Delta y=y_1-y_0\leq\Delta x,\qquad m=\frac{\Delta y}{\Delta x}\in[0,1].
$$

The vertical case is handled by exchanging axes. In this octant, increasing $x$ by one requires increasing $y$ by either zero or one. Thus, from the currently plotted [pixel](../../../../../pixel.md) $(x,y)$ the candidates are $E=(x+1,y)$ and $NE=(x+1,y+1)$.

Use the [implicit equation](../../../../../implicit-equation.md) of the [line](../../../../../straight-line.md)

$$
f(X,Y)=\Delta y(X-x_0)-\Delta x(Y-y_0).
$$

At a fixed $X$, $f(X,Y)>0$ means that $(X,Y)$ lies below the exact [line](../../../../../straight-line.md). The [midpoint line decision](../../../../../midpoint-line-decision.md) evaluates $M=(x+1,y+1/2)$, halfway between the two candidate [pixel](../../../../../pixel.md) centres. If $f(M)<0$, the exact [line](../../../../../straight-line.md) lies below $M$, so choose $E$; if $f(M)>0$, choose $NE$. At equality either candidate is equally near, but a fixed tie rule is essential. We choose $NE$ on a tie throughout these solutions:

$$
\boxed{f(x+1,y+1/2)<0\Rightarrow E;\qquad f(x+1,y+1/2)\geq0\Rightarrow NE.}
$$

This chooses the closest vertical-grid [pixel](../../../../../pixel.md) centre in each column, with ties rounded upward. Since $0\leq m\leq1$, the result has one [pixel](../../../../../pixel.md) per column and consecutive [pixels](../../../../../pixel.md) share an edge or a corner.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Computer graphics](../../../computer-graphics-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
