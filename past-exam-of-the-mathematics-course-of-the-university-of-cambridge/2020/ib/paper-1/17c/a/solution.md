<h1 id="17c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [velocity potential](../../../../../../velocity-potential.md), $\mathbf u=\nabla\phi$. The [incompressible flow](../../../../../../incompressible-flow.md) condition $\nabla\cdot\mathbf u=0$ therefore becomes [Laplace equation](../../../../../../laplace-equation.md) $\nabla^2\phi=0$. The [Laplace equation in polar coordinates](../../../../../../laplace-equation-in-polar-coordinates.md) gives

$$
\nabla^2\phi
=A(\gamma^2-\lambda^2)r^{\gamma-2}\cos(\lambda\theta),
$$

so positivity of $\gamma$ and $\lambda$ requires

$$
\boxed{\gamma=\lambda}.
$$

The velocity components are

$$
u_r=\frac{\partial\phi}{\partial r}
=A\gamma r^{\gamma-1}\cos(\lambda\theta),
\qquad
u_\theta=\frac1r\frac{\partial\phi}{\partial\theta}
=-A\lambda r^{\gamma-1}\sin(\lambda\theta).
$$

The [no-penetration boundary condition](../../../../../../no-penetration-boundary-condition.md) on both walls says $u_\theta=0$ at $\theta=0$ and $\theta=\alpha$, hence $\lambda\alpha=n\pi$. If $n\ge2$, $\sin(n\pi\theta/\alpha)$ changes sign inside the wedge. The stated sign condition therefore selects $n=1$, and

$$
\boxed{\gamma=\lambda=\frac\pi\alpha}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17C](../../17c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
