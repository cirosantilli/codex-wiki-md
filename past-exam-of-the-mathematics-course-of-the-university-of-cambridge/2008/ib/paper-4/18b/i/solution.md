<h1 id="18b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For constant density $\rho$, the inviscid [Euler equations](../../../../../../euler-equations-for-an-inviscid-fluid.md) with conservative [body force](../../../../../../body-force.md) are

$$
\partial_t\mathbf u+(\mathbf u\cdot\nabla)\mathbf u=-\nabla(p/\rho+V).
$$

The vector identity $(\mathbf u\cdot\nabla)\mathbf u=\nabla(|\mathbf u|^2/2)-\mathbf u\times(\nabla\times\mathbf u)$ simplifies for [potential flow](../../../../../../potential-flow.md) $\mathbf u=\nabla\phi$, since its [vorticity](../../../../../../vorticity.md) vanishes. Also $\partial_t\mathbf u=\nabla\phi_t$. Therefore

$$
\nabla\left(\phi_t+\frac12|\mathbf u|^2+\frac p\rho+V\right)=0.
$$

On each connected fluid region the expression is spatially constant but may depend on time, giving the [Unsteady Bernoulli equation](../../../../../../unsteady-bernoulli-equation.md)

$$
\boxed{\frac{\partial\phi}{\partial t}+\frac12u^2+\chi=f(t),\qquad \chi=p/\rho+V.}
$$

The arbitrariness of $f$ corresponds to the freedom to add a function of time to the [velocity potential](../../../../../../velocity-potential.md) without changing $\mathbf u$. Replacing $\phi$ by $\phi-\int^t f(s)\,ds$ sets the right-hand side to zero.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [18B](../../18b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
