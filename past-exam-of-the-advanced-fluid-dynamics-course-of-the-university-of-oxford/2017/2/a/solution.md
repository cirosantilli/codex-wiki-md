<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $\mathbf R=\mathbf r_2-\mathbf r_1$ and label each [dumbbell](../../../../hookean-dumbbell-model.md) once. Locally assume its [probability density](../../../../probability-density.md) and [number density](../../../../number-density.md) vary negligibly over a connector length. The [oriented connector crossing count](../../../../oriented-connector-crossing-count.md) follows geometrically: a connector crosses a small [plane](../../../../plane.md) element precisely when its midpoint lies within a slab of normal thickness $|\mathbf R\cdot\mathbf n|$. For configurations in $d^3R$, the **unsigned** crossing number per unit area is therefore

$$
\boxed{n|\mathbf R\cdot\mathbf n|\psi(\mathbf x,\mathbf R,t)\,d^3R.}
$$

The expression without the [absolute value](../../../../absolute-value.md) is an oriented crossing count, or an unsigned count restricted to $\mathbf R\cdot\mathbf n\ge0$. It cannot be an unrestricted nonnegative number: a connector $\mathbf R=-R\mathbf n$ gives a negative printed expression despite physically intersecting the [plane](../../../../plane.md).

To obtain [traction](../../../../traction.md), keep the [force](../../../../force-split.md) orientation as well. For $\mathbf R\cdot\mathbf n>0$, the [spring force](../../../../hooke-s-law.md) on the bead below the [plane](../../../../plane.md) exerted by the bead above it is $H\mathbf R$. For the opposite orientation it is $-H\mathbf R$. Multiplying that [force](../../../../force-split.md) by the unsigned crossing count in either case gives

$$
d\mathbf t=nH\mathbf R(\mathbf R\cdot\mathbf n)\psi\,d^3R.
$$

Integrating over all labelled configurations yields

$$
\mathbf t=\left[nH\int\mathbf R\mathbf R^T\psi\,d^3R\right]\mathbf n,
\qquad
\boxed{\boldsymbol\sigma_{\rm spring}=nH\langle\mathbf R\mathbf R^T\rangle.}
$$

There is no extra factor of two: each [dumbbell](../../../../hookean-dumbbell-model.md) was labelled and counted once, and the orientation-dependent [force](../../../../force-split.md) has already supplied the sign. This is the local [continuum](../../../../continuum-mechanics-split.md) [stress approximation](../../../../cauchy-stress-tensor.md); resolving appreciable spatial [variation](../../../../calculus-of-variations-split.md) across a finite connector would require a nonlocal [stress](../../../../stress.md) construction.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
