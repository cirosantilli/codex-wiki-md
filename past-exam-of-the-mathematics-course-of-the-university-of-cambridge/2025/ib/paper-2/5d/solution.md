<h1 id="5d/solution">Solution</h1>

↑ **Parent:** [5D](../5d.md)

For incompressible inviscid flow without body force,

$$
\nabla\cdot u=0,\qquad \partial_tu+(u\cdot\nabla)u=-\rho^{-1}\nabla p.
$$

Taking curl gives

$$
\partial_t\omega+(u\cdot\nabla)\omega=(\omega\cdot\nabla)u,\qquad \omega=\nabla\times u,
$$

equivalently $\partial_t\omega=\nabla\times(u\times\omega)$.

Direct [differentiation](../../../../../differentiation.md) of the stated field gives $\omega=u$. Hence $u\times\omega=0$, so the [vorticity equation](../../../../../vorticity-equation.md) gives $\partial_t\omega=0$ and the field is steady. Finally

$$
(u\cdot\nabla)u=\nabla(|u|^2/2)-u\times\omega=\nabla(|u|^2/2).
$$

Euler's equation therefore implies

$$
\nabla\left(p+\frac12\rho|u|^2\right)=0,
$$

so $H$ is spatially uniform.

## ↑ Ancestors (10)

1. [5D](../5d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
