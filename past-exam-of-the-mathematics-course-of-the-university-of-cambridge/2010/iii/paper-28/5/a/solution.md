<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $f=u+iv$. The prescribed complex-linear differential is exactly the [Cauchy-Riemann equations](../../../../../../cauchy-riemann-equations.md)

$$
u_x=v_y,\qquad u_y=-v_x.
$$

A [holomorphic function](../../../../../../holomorphic-function.md) is smooth, as follows locally from its Cauchy integral formula, so its mixed second [partial derivatives](../../../../../../partial-derivative.md) commute. Differentiating the two equations gives

$$
\Delta u=u_{xx}+u_{yy}=v_{yx}-v_{xy}=0,
$$

and, rewriting them as $v_x=-u_y$, $v_y=u_x$,

$$
\Delta v=v_{xx}+v_{yy}=-u_{yx}+u_{xy}=0.
$$

Thus $\boxed{\Delta\Re f=\Delta\Im f=0}$: both components are [harmonic functions](../../../../../../harmonic-function.md). Here $\Delta=\partial_x^2+\partial_y^2$, the sign convention used for the Brownian generator $\Delta/2$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
