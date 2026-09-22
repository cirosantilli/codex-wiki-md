<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Choose the [oriented surface](../../../../oriented-surface.md) parametrization $\mathbf r(x,y)=(x,y,1-x)$, with $0\leq x,y\leq1$. Then $\mathbf r_x\times\mathbf r_y=(1,0,1)$ and $\nabla\times\mathbf A=(-3z,x^2,y)$. The [surface integral](../../../../surface-integral.md) is

$$
\iint_S(\nabla\times\mathbf A)\cdot d\mathbf S=\int_0^1\int_0^1[-3(1-x)+y]\,dx\,dy=-1.
$$

For the compatible boundary direction, use successive vertices $(0,0,1)$, $(1,0,0)$, $(1,1,0)$, $(0,1,1)$ and back. The four [line integrals](../../../../line-integral.md) are respectively

$$
\int_0^1x^2(1-x)\,dx=\frac1{12},\qquad \int_0^1y\,dy=\frac12,\qquad \int_1^0[x^2(1-x)+3(1-x)]\,dx=-\frac{19}{12},\qquad0.
$$

Their sum is **$-1$, agreeing with the surface integral**. Choosing the opposite normal and reversing the boundary direction gives $+1$ on both sides. Stating an orientation is necessary because the question does not prescribe one.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
