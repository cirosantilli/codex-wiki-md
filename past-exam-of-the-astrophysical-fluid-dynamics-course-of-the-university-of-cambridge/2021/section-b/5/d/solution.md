<h1 id="section-b/5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Along a family of equilibria at fixed temperature, $K$ and the dimensionless function $\Psi$ are fixed. The boundary [mass density](../../../../../density.md) changes through both $\rho_c$ and the boundary coordinate $\xi$:

$$
\boxed{\delta\rho=e^{-\Psi}\delta\rho_c-\rho_ce^{-\Psi}\Psi'\delta\xi
=\rho\left(\frac{\delta\rho_c}{\rho_c}-\Psi'\delta\xi\right).}
$$

From part (c), $N=C\rho_c^{-1/2}f(\xi)$, where $C$ is constant at fixed temperature and $f=\xi^2\Psi'$. Set its logarithmic variation to zero:

$$
0=\frac{\delta N}{N}=-\frac12\frac{\delta\rho_c}{\rho_c}
+\frac{f'}f\delta\xi.
$$

The [isothermal Lane-Emden equation](../../../../../isothermal-lane-emden-equation.md) gives $f'=\xi^2e^{-\Psi}$, so the fixed-$N$ relation is

$$
\boxed{\frac{\delta\rho_c}{\rho_c}=\frac{2e^{-\Psi}}{\Psi'}\delta\xi.}
$$

Substitute back into the boundary-density variation:

$$
\delta\rho\big|_N
=\rho\left(\frac{2e^{-\Psi}}{\Psi'}-\Psi'\right)\delta\xi.
$$

For a nontrivial variation at a finite positive radius, its vanishing gives the [fixed-mass turning point of an isothermal sphere](../../../../../fixed-mass-turning-point-of-an-isothermal-sphere.md):

$$
\boxed{[\Psi'(\xi)]^2=2e^{-\Psi(\xi)}.}
$$

This derivative follows a fixed-mass sequence of equilibria; it is not merely the spatial derivative of density inside one sphere. The corresponding radial variation is

$$
\frac{\delta r}{r}=\left(\frac1\xi-\frac{e^{-\Psi}}{\Psi'}\right)\delta\xi.
$$

At small $\xi$, $\Psi'\simeq\xi/3$: the boundary density increases while the radius decreases along increasing $\xi$, giving the stated negative $(\partial p/\partial V)_{N,T}$ of the stable branch. The first density turning point marks its first loss of radial [stability](../../../../../stability-of-a-numerical-method.md); it need not be confused with a turning point of radius itself.

## ↑ Ancestors (14)

1. [D](../d.md)
2. [5](../../5.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../../split.md)
6. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
