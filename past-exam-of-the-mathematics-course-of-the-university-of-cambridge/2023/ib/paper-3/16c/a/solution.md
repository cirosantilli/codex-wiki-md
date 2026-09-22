<h1 id="16c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an inviscid fluid of constant [mass density](../../../../../../density.md) $\rho$ with no body force, the [Euler equations for an inviscid fluid](../../../../../../euler-equations-for-an-inviscid-fluid.md) are

$$
\partial_tu+(u\cdot\nabla)u=-\frac1\rho\nabla p.
$$

The vector identity

$$
(u\cdot\nabla)u=\nabla\!\left(\frac12|u|^2\right)-u\times(\nabla\times u)
$$

and [irrotational flow](../../../../../../irrotational-flow.md) give $(u\cdot\nabla)u=\nabla(|u|^2/2)$. Writing $u=\nabla\phi$ in terms of a [velocity potential](../../../../../../velocity-potential.md), we obtain

$$
\nabla\!\left(\partial_t\phi+\frac12|\nabla\phi|^2+\frac p\rho\right)=0.
$$

Thus the bracket depends only on time:

$$
\boxed{\partial_t\phi+\frac12|\nabla\phi|^2+\frac p\rho=C(t)}.
$$

Since adding a function of time to $\phi$ leaves $u=\nabla\phi$ unchanged, that function may be chosen to absorb $C(t)$. This is the [Unsteady Bernoulli equation](../../../../../../unsteady-bernoulli-equation.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [16C](../../16c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
