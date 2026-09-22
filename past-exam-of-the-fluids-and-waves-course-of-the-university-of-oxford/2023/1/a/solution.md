<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [irrotational flow](../../../../irrotational-flow.md) has $\nabla\times\mathbf u=0$. Hence a [velocity potential](../../../../velocity-potential.md) $\phi$ exists locally, and globally on a [simply connected domain](../../../../simply-connected-domain.md), with $\mathbf u=\nabla\phi$. The exterior of a sphere in three dimensions has this property. Constant [mass density](../../../../density.md) reduces the [continuity equation](../../../../continuity-equation.md) to $\nabla\cdot\mathbf u=0$, so

$$
\boxed{\nabla^2\phi=0}.
$$

Thus the [velocity potential](../../../../velocity-potential.md) is a [harmonic function](../../../../harmonic-function.md). For the [Euler equations](../../../../euler-equations-for-an-inviscid-fluid-split.md), use the [vorticity cross-product identity](../../../../vorticity-cross-product-identity.md)

$$
(\mathbf u\cdot\nabla)\mathbf u
=\nabla\!\left(\frac12|\mathbf u|^2\right)
-\mathbf u\times(\nabla\times\mathbf u).
$$

The last term vanishes. Since $\partial_t\mathbf u=\nabla\phi_t$, the [Euler momentum equation](../../../../euler-equations-for-an-inviscid-fluid-split.md) becomes

$$
\nabla\!\left(\phi_t+\frac12|\nabla\phi|^2+\frac p\rho\right)=0.
$$

On each connected fluid region, a function with zero [gradient](../../../../gradient.md) is spatially constant. Therefore the [Unsteady Bernoulli equation](../../../../unsteady-bernoulli-equation.md) is

$$
\boxed{\frac p\rho+\phi_t+\frac12|\nabla\phi|^2=F(t)}.
$$

The freedom to add a function of time to the [velocity potential](../../../../velocity-potential.md) changes $F(t)$ but leaves the [velocity field](../../../../velocity-field.md) unchanged. On a multiply connected region, zero [vorticity](../../../../vorticity-split.md) alone guarantees only local potentials; a global single-valued [velocity potential](../../../../velocity-potential.md) additionally requires zero [circulation](../../../../circulation-physics.md) around every closed path.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the fluids and waves course of the University of Oxford](../../../split.md)
5. [Fluids and waves course of the University of Oxford](../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
