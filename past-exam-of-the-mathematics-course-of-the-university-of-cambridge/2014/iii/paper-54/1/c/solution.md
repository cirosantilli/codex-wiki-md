<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The axial [angular momentum](../../../../../../angular-momentum.md) density is $\rho Ru_\phi$. The second equation in part (b) writes its conservation law with [magnetic axial angular momentum flux](../../../../../../magnetic-axial-angular-momentum-flux.md)

$$
\mathbf F_{J,p}=-\frac{RB_\phi\mathbf B_p}{\mu_0}.
$$

The nonmagnetic part of the energy flux is azimuthal. Using $(\mathbf u\times\mathbf B)\times\mathbf B=\mathbf B(\mathbf u\cdot\mathbf B)-\mathbf u B^2$, its poloidal part is

$$
\boxed{\mathbf F_{E,p}=-\frac{u_\phi B_\phi\mathbf B_p}{\mu_0}=\Omega\mathbf F_{J,p}.}
$$

The ratio is therefore $\Omega$ wherever the compared component of the angular-momentum flux is nonzero; the proportionality remains meaningful at zero flux.

A fully steady magnetic configuration requires $\partial_tB_\phi=0$, hence $\mathbf B_p\cdot\nabla\Omega_0=0$: [angular velocity](../../../../../../angular-velocity.md) is constant along poloidal field lines. This is [Ferraro's law of isorotation](../../../../../../ferraro-s-law-of-isorotation.md). The steady azimuthal force additionally requires $\mathbf B_p\cdot\nabla(RB_\phi)=0$, which holds, for example, if $B_\phi=0$. The remaining meridional force balance is a separate equilibrium condition.

Since $\rho$ and $\mathbf B_p$ are time independent, differentiate the angular-momentum equation once more and substitute the induction equation:

$$
\boxed{\rho R^2\mu_0\partial_t^2\Omega=\mathbf B_p\cdot\nabla\!\left(R^2\mathbf B_p\cdot\nabla\Omega\right).}
$$

This is the variable-coefficient wave equation for the [torsional Alfvén wave](../../../../../../torsional-alfven-wave.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 54](../../../paper-54-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
