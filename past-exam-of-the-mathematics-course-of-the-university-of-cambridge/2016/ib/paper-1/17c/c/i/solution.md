<h1 id="17c/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write the conservative body force per unit mass as $-\nabla\Phi$. For a fluid of constant density $\rho$, the [Euler equations for an inviscid fluid](../../../../../../../euler-equations-for-an-inviscid-fluid.md) and the [incompressible flow](../../../../../../../incompressible-flow.md) condition are

$$
\partial_t\mathbf u+(\mathbf u\cdot\nabla)\mathbf u=-\nabla\left(\frac p\rho+\Phi\right),\qquad \nabla\cdot\mathbf u=0.
$$

Using part (a), these become

$$
\partial_t\mathbf u-\mathbf u\times\boldsymbol\omega=-\nabla H,\qquad H=\tfrac12|\mathbf u|^2+\frac p\rho+\Phi.
$$

For [irrotational flow](../../../../../../../irrotational-flow.md), locally choose a [velocity potential](../../../../../../../velocity-potential.md) with $\mathbf u=\nabla\phi$. Then $\nabla(\partial_t\phi+H)=0$, so **the unsteady Bernoulli integral** is

$$
\boxed{\partial_t\phi+\tfrac12|\mathbf u|^2+\frac p\rho+\Phi=C(t).}
$$

The constant is spatially uniform on a connected region where the [velocity potential](../../../../../../../velocity-potential.md) is defined; its time dependence can be absorbed into the additive time-dependent gauge of $\phi$. A global single-valued [velocity potential](../../../../../../../velocity-potential.md) requires an appropriate topological condition, such as a [simply connected](../../../../../../../simply-connected-space.md) domain; without it, the integral is locally valid. In a connected steady irrotational region, $\nabla H=0$ directly gives one spatial Bernoulli constant even without choosing a global potential.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [17C](../../../17c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ib](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
