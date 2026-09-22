<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [stellar polytrope](../../../../stellar-polytrope.md) approximates a spherical self-gravitating star by the structural relation

$$
p=K\rho^{1+1/n},
$$

where $K$ is constant and $n$ is the [polytropic index](../../../../polytropic-index.md). Combining [hydrostatic equilibrium](../../../../hydrostatic-equilibrium.md) with [mass conservation](../../../../mass-conservation.md) gives

$$
\frac{dp}{dr}=-\frac{Gm(r)\rho}{r^2},\qquad
\frac{dm}{dr}=4\pi r^2\rho.
$$

The [Lane-Emden variables for a stellar polytrope](../../../../lane-emden-variables-for-a-stellar-polytrope.md) separate the dimensional scales from the profile:

$$
\rho=\rho_c\theta^n,\quad r=a\xi,\qquad
 a^2=\frac{(n+1)K}{4\pi G}\rho_c^{1/n-1}.
$$

For $n>0$ these substitutions give the [Lane-Emden equation](../../../../lane-emden-equation.md)

$$
\boxed{\frac1{\xi^2}\frac d{d\xi}\left(\xi^2\frac{d\theta}{d\xi}\right)=-\theta^n,\qquad
\theta(0)=1,\quad\theta'(0)=0.}
$$

The central conditions express finite central [mass density](../../../../density.md) and spherical symmetry. If $\xi_1$ is the first zero, a zero-pressure surface has

$$
R=a\xi_1,\qquad
M=4\pi a^3\rho_c[-\xi_1^2\theta'(\xi_1)],
$$

the [Lane-Emden mass formula](../../../../lane-emden-mass-formula.md). For $0<n<5$ this surface is at finite radius. For example, the [polytrope of index one](../../../../polytrope-of-index-one.md) has $\theta=\sin\xi/\xi$ and $\xi_1=\pi$, giving the density profile shown in the overview figure.

An isentropic ideal monatomic gas has $p\propto\rho^{5/3}$ and hence $n=3/2$, a useful approximation for a fully convective ideal-gas star. Nonrelativistic [electron degeneracy pressure](../../../../electron-degeneracy-pressure.md) has the same density exponent. The exponent $4/3$, giving $n=3$, occurs for ultrarelativistic electron degeneracy and in appropriate radiation-dominated stellar models. The structural index should not be confused with the [adiabatic index](../../../../heat-capacity-ratio.md) controlling a perturbation unless the model is actually isentropic.

Polytropes give useful mass-radius scalings and central concentration with very few parameters. They do not by themselves specify [nuclear fusion](../../../../nuclear-fusion.md), energy transport, or the star's thermal evolution. Nor does a structural profile alone establish dynamical stability; that requires the response of [pressure](../../../../pressure-split.md) to the perturbation.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../split.md)
5. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
