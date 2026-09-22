<h1 id="f/f1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The constraint set $S^1\times S^2$ is [compact](../../../../../compact-space.md), so the continuous objective attains a maximum and minimum. The two constraint [gradients](../../../../../gradient.md) are nonzero and supported on separate coordinates, so they are [linearly independent](../../../../../linear-independence.md) everywhere on it. The [Lagrange multiplier](../../../../../lagrange-multiplier.md) equations are

$$
y_2-y_3=2\lambda x_1,\quad0=2\lambda x_2,\quad0=2\mu y_1,\quad x_1=2\mu y_2,\quad-x_1=2\mu y_3.
$$

Both positive and negative values occur. At a maximizing or minimizing point the objective is therefore nonzero, so $x_1\ne0$, $y_2-y_3\ne0$, and both $\lambda,\mu$ are nonzero. The equations imply $x_2=0$, $y_1=0$, and $y_3=-y_2$. The constraints then give $x_1=\pm1$, $y_2=\pm1/\sqrt2$.

Consequently, writing $s=\pm1$, the complete list of extrema is

$$
\boxed{\max=\sqrt2:\ (x_1,x_2;y_1,y_2,y_3)=(s,0;0,s/\sqrt2,-s/\sqrt2)},
$$



$$
\boxed{\min=-\sqrt2:\ (x_1,x_2;y_1,y_2,y_3)=(s,0;0,-s/\sqrt2,s/\sqrt2)}.
$$

For an independent global check, [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $|x_1(y_2-y_3)|\leq|x_1|\sqrt{2(y_2^2+y_3^2)}\leq\sqrt2$, with equality exactly at the displayed points.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [F1](../../f1.md)
3. [F](../../../f.md)
4. [2006](../../../../2006-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
