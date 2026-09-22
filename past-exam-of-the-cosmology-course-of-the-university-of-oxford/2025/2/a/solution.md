<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Helmholtz decomposition](../../../../helmholtz-decomposition.md) separates the [peculiar velocity](../../../../peculiar-velocity.md) into a [gradient field](../../../../gradient-field.md) and a [transverse vector field](../../../../transverse-vector-field.md):

$$
\mathbf v=\nabla V+\mathbf v_\perp,\qquad \nabla\cdot\mathbf v_\perp=0.
$$

With decaying or periodic spatial boundary conditions this is equivalently the [Fourier transform](../../../../fourier-transform-split.md) projection, for $k\ne0$,

$$
v_{\perp i}(\mathbf k)=\left(\delta_{ij}-\frac{k_ik_j}{k^2}\right)v_j(\mathbf k).
$$

The [transverse projection operator](../../../../transverse-projection-operator.md) annihilates a [gradient](../../../../gradient.md), because $(\delta_{ij}-k_ik_j/k^2)k_j=0$. Both forces in the linear [cosmological Euler equation](../../../../cosmological-euler-equation.md) are [gradients](../../../../gradient.md), with spatially homogeneous coefficients. Applying the [transverse projection operator](../../../../transverse-projection-operator.md) therefore gives

$$
\dot{\mathbf v}_\perp+H\mathbf v_\perp=0.
$$

Since $H=\dot a/a$, this is $d(a\mathbf v_\perp)/dt=0$, and hence

$$
\boxed{\mathbf v_\perp(\mathbf x,t)=\frac{a(t_i)}{a(t)}\mathbf v_\perp(\mathbf x,t_i).}
$$

At this order the scalar pressure and gravitational forces cannot generate [vorticity](../../../../vorticity-split.md); an initially vanishing [transverse vector field](../../../../transverse-vector-field.md) remains zero. Its nonzero initial value is damped by [cosmic expansion](../../../../expansion-of-the-universe.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the cosmology course of the University of Oxford](../../../split.md)
5. [Cosmology course of the University of Oxford](../../../../cosmology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
