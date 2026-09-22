<h1 id="9c/solution">Solution</h1>

↑ **Parent:** [9C](../9c.md)

The general [continuity equation](../../../../../continuity-equation.md) is $\rho_t+\nabla\cdot(\rho u)=0$, or $D\rho/Dt+\rho\nabla\cdot u=0$. An [incompressible flow](../../../../../incompressible-flow.md) has $D\rho/Dt=0$, so for positive density **$\boxed{\nabla\cdot u=0}$**.

For the displayed velocity field, on $x^2+y^2>0$,

$$
\partial_x\frac{y}{x^2+y^2}=-\frac{2xy}{(x^2+y^2)^2},\qquad
\partial_y\frac{-x}{x^2+y^2}=\frac{2xy}{(x^2+y^2)^2}.
$$

The sum is zero. A [stream function](../../../../../stream-function.md) with the required sign convention is

$$
\boxed{\psi(x,y)=\frac12\log(x^2+y^2)+C.}
$$

Its derivatives give exactly $u=(\psi_y,-\psi_x)$. The origin is excluded because the prescribed velocity is singular there.

## ↑ Ancestors (10)

1. [9C](../9c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
