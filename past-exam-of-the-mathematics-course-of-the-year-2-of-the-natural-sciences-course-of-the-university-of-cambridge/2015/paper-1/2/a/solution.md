<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Remove the first spatial [derivative](../../../../../derivative.md) by the [Dirichlet gauge transform for constant drift](../../../../../dirichlet-gauge-transform-for-constant-drift.md):

$$
u(x,y,t)=e^{-\beta x/2}v(x,y,t),\qquad v_t=v_{xx}+v_{yy}-\frac{\beta^2}{4}v.
$$

The nonzero exponential factor preserves the zero side and top values; it also preserves $v_y=0$ on the bottom. A separated product $v=X(x)Y(y)T(t)$ has the spatial [eigenvalue problems](../../../../../eigenvalue-problem.md)

$$
X''+k_x^2X=0,\quad X(0)=X(1)=0;\qquad Y''+k_y^2Y=0,\quad Y'(0)=Y(1)=0.
$$

The nontrivial solutions are $X_m=\sin(m\pi x)$ for $m\geq1$ and $Y_n=\cos((n-1/2)\pi y)$ for $n\geq1$. There is no zero spatial mode in either direction. The temporal equation gives $T=e^{-\lambda_{mn}t}$, where

$$
\lambda_{mn}=m^2\pi^2+(n-1/2)^2\pi^2+\beta^2/4.
$$

Therefore the [mixed-boundary drift-diffusion eigenmodes on a rectangle](../../../../../mixed-boundary-drift-diffusion-eigenmodes-on-a-rectangle.md) give

$$
\boxed{u(x,y,t)=e^{-\beta x/2}\sum_{m=1}^\infty\sum_{n=1}^\infty A_{mn}\sin(m\pi x)\cos((n-1/2)\pi y)e^{-\lambda_{mn}t}.}
$$

At $t=0$ the temporal factors are one, giving the required expansion. The sine and mixed-end cosine bases are complete and orthogonal for $v$. In particular,

$$
A_{mn}=4\int_0^1\int_0^1 e^{\beta x/2}u(x,y,0)\sin(m\pi x)\cos((n-1/2)\pi y)\,dy\,dx.
$$

The factor four comes from the product of the two squared basis norms, each $1/2$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
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
