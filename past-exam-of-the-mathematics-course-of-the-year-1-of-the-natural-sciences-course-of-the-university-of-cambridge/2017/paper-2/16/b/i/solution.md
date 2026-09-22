<h1 id="16/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The PDF diagram specifies the prism as

$$
0\leq x\leq2,\qquad0\leq y\leq4-2x,\qquad0\leq z\leq1.
$$

Its triangular horizontal cross-section has area four. Calculate the outward [flux](../../../../../../flux.md) on each face using its outward [normal vector](../../../../../../normal-vector.md).

On $x=0$, the normal is $-\mathbf e_x$ and $F_x=0$, so the [flux](../../../../../../flux.md) is zero. On $y=0$, the normal is $-\mathbf e_y$, giving

$$
\Phi_{y=0}=-\int_0^1\int_0^2(2x-4)^2\,dx\,dz=-\frac{32}{3}.
$$

On the sloping vertical face $y+2x=4$, the outward normal is proportional to $(2,1,0)$. Both $F_x$ and $F_y$ vanish there, while $F_z$ is tangent to the face, so the [flux](../../../../../../flux.md) is zero.

On the bottom $z=0$, the normal is $-\mathbf e_z$ and $F_z=1$, so the [flux](../../../../../../flux.md) is minus the base area, namely $-4$. On the top $z=1$, $F_z=0$, so the [flux](../../../../../../flux.md) is zero. Thus all five face values and their sum are

$$
\boxed{\begin{array}{c|ccccc}
\text{face}&x=0&y=0&y+2x=4&z=0&z=1\\\hline
\text{outward flux}&0&-32/3&0&-4&0
\end{array}\qquad\Phi_{\mathrm{total}}=-\frac{44}{3}}.
$$

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [16](../../../16.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
