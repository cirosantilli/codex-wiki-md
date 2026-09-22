<h1 id="8c/solution">Solution</h1>

↑ **Parent:** [8C](../8c.md)

Taking the curl of the [Euler equation](../../../../../euler-equations-for-an-inviscid-fluid.md) gives the [vorticity equation](../../../../../vorticity-equation.md) for an inviscid [incompressible flow](../../../../../incompressible-flow.md) without body forces:

$$
\boxed{\partial_t\boldsymbol\omega+(u\cdot\nabla)\boldsymbol\omega
=(\boldsymbol\omega\cdot\nabla)u,\qquad\boldsymbol\omega=\nabla\times u.}
$$

The given velocity has divergence $-1+0+1=0$ and curl $(0,0,\omega(t))$. Its vorticity is spatially uniform, so its advective derivative vanishes. The stretching term is $\omega\partial_zu=(0,0,\omega)$. Thus

$$
\omega'=\omega,\qquad\boxed{\omega(t)=\omega_0e^t.}
$$

The signed vertical component is $\omega_0e^t$; its magnitude is $|\omega_0|e^t$, with the source's magnitude convention taking $\omega_0\geq0$. As an additional consistency check, after imposing this equation the material acceleration is $(x,0,z-1)$, so a pressure $p=-\rho[x^2+(z-1)^2]/2+p_0(t)$ satisfies the full [Euler equation](../../../../../euler-equations-for-an-inviscid-fluid.md).

## ↑ Ancestors (10)

1. [8C](../8c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
