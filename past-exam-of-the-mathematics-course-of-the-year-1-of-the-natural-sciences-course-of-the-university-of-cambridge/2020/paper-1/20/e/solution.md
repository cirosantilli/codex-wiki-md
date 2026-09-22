<h1 id="20/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Take a piecewise linear [path](../../../../../continuous-path.md) along three coordinate directions, passing through the origin and then $(0,1,0)$:

$$
\mathbf x(t)=\begin{cases}(1-t,0,0),&0\le t\le1,\\(0,t-1,0),&1\le t\le2,\\(0,1,t-2),&2\le t\le3.\end{cases}
$$

On the first segment $G_x=y^2+z^2=0$, so its [line integral](../../../../../line-integral.md) is zero. On the second $G_y=x^2+z^2=0$, so its contribution is also zero. On the last segment $G_z=x^2+y^2=1$ and $z$ increases from zero to one. Therefore

$$
\boxed{\int\mathbf G\cdot d\mathbf x=0+0+\int_0^1 1\,dz=1\ne\frac23.}
$$

This gives the requested concrete path dependence with the same ordered endpoints.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [20](../../20.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
