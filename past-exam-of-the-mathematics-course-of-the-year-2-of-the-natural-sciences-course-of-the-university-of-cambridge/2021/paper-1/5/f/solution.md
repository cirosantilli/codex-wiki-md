<h1 id="5/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Applying the rightmost [rotation matrix](../../../../../rotation-matrix.md) first gives

$$
R_1\mathbf e_z=(\sin\theta\cos\phi,\sin\theta\sin\phi,\cos\theta)^T.
$$

Equality with $\mathbf e_y$ requires $\cos\theta=0$, so $\theta=\pi/2$ in the specified range. Then $\sin\phi=1$ and $\cos\phi=0$ give

$$
\boxed{\theta=\frac\pi2,\qquad\phi=\frac\pi2.}
$$

In the reverse order, $R_z$ first fixes $\mathbf e_z$, so $R_2\mathbf e_z=R_y(\pi/2)\mathbf e_z=\mathbf e_x$. Therefore $\boxed{R_2\mathbf v\ne\mathbf v'}$. This explicitly demonstrates that [rotations](../../../../../rotation-mathematics.md) about different axes do not generally commute.

## ↑ Ancestors (13)

1. [F](../f.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
