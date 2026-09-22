<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

In a spherical self-gravitating equilibrium with positive [mass density](../../../../density.md), $d\psi/dr=GM(r)/r^2>0$ away from the center. Thus $r$ can locally be replaced by $\psi$, so both $p(r)$ and $\rho(r)$ can be expressed as functions of $\psi$. [Hydrostatic equilibrium](../../../../hydrostatic-equilibrium.md) further gives

$$
\frac{dp}{d\psi}=-\rho.
$$

Since $p$ decreases outward wherever $\rho>0$, eliminating $\psi$ gives a [barotropic equation of state](../../../../barotropic-equation-of-state.md) along this equilibrium. This is a relation describing its structure; it does not require all thermodynamic perturbations of an arbitrary material to be barotropic.

For $p=K\rho^{1+1/n}$, integrate the [polytropic enthalpy](../../../../polytropic-enthalpy.md) balance $dp/\rho=-d\psi$:

$$
(n+1)K\rho^{1/n}+\psi=\psi_T,\qquad
\boxed{\rho=\left[\frac{\psi_T-\psi}{(n+1)K}\right]^n.}
$$

For a finite-radius zero-pressure boundary with $K>0$ and $n>0$, $\rho(R)=0$ and therefore $\psi_T=\psi(R)$. With the gravitational potential zero at infinity, an isolated sphere has $\psi_T=-GM/R$. It is an integration constant tied to that boundary, not necessarily a zero of the [gravitational potential](../../../../newtonian-potential-of-a-point-mass.md).

Put $\theta=(\rho/\rho_c)^{1/n}$ and $\xi=\alpha r$, with $\alpha^2=4\pi G\rho_c^{1-1/n}/[(n+1)K]$. The preceding relation gives $\psi=\psi_T-(n+1)K\rho_c^{1/n}\theta$. Substitution into the spherical gravitational [Poisson equation](../../../../poisson-s-equation.md) yields the [Lane-Emden equation](../../../../lane-emden-equation.md)

$$
\boxed{\frac1{\xi^2}\frac d{d\xi}\left(\xi^2\frac{d\theta}{d\xi}\right)=-\theta^n,\qquad
\theta(0)=1,\quad\theta'(0)=0.}
$$

Let $\xi_1$ be the first zero of the regular [Lane-Emden function](../../../../lane-emden-function.md) and $Y_n=-\xi_1^2\theta'(\xi_1)>0$. Then the [Lane-Emden mass formula](../../../../lane-emden-mass-formula.md) and radius are

$$
R=\frac{\xi_1}{\alpha},\qquad
M=\frac{4\pi\rho_c}{\alpha^3}Y_n.
$$

For a common fixed [polytropic index](../../../../polytropic-index.md) with a finite first zero, their scalings are

$$
\boxed{M\propto K^{3/2}\rho_c^{3/(2n)-1/2},\qquad
R\propto K^{1/2}\rho_c^{1/(2n)-1/2}.}
$$

The usual regular zero-pressure models have a finite first zero for $0<n<5$; the $n=5$ model has infinite radius, so a finite-radius formula cannot simply be applied to it.

For an [ideal gas](../../../../ideal-gas-split.md) of fixed composition, $T_c\propto K\rho_c^{1/n}$. Consequently [homologous polytropes at fixed central temperature](../../../../homologous-polytropes-at-fixed-central-temperature.md) have $K\propto\rho_c^{-1/n}$ and both $M,R\propto\rho_c^{-1/2}$, recovering $M\propto R$. The common central [temperature](../../../../temperature-split.md), composition and dimensionless structure are the relevant assumptions. Keeping $K$ fixed instead gives the different [polytropic mass-radius relation](../../../../polytropic-mass-radius-relation.md), and no finite index makes its generic fixed-$K$ exponent exactly one.

For adiabatic monatomic [hydrogen](../../../../hydrogen.md), $\gamma=5/3$ and $n=3/2$. At a common fixed [specific entropy](../../../../specific-entropy.md), hence common $K$, the same relations give

$$
\boxed{R\propto KM^{-1/3},\qquad M\propto R^{-3},\qquad\bar\rho\propto M^2\quad(K\text{ fixed}).}
$$

Here $\bar\rho=3M/(4\pi R^3)$, and the omitted constant in the last relation depends on $K$. A population with different cloud entropies need not follow that [mass](../../../../mass.md) sequence.

Efficient [radiative cooling](../../../../radiative-cooling.md) in [molecular clouds](../../../../molecular-cloud.md) prevents compression from forcing the [temperature](../../../../temperature-split.md) upward as steeply as in an adiabatic monatomic gas. Rotational transitions of molecules and radiation by dust provide low-temperature cooling channels; which dominates depends on composition, opacity and [temperature](../../../../temperature-split.md). It is therefore possible to assemble dense massive cold clouds while disposing of compressional [heat](../../../../heat-split.md). This explains the direction of the idealized comparison, rather than proving a universal cloud-mass cutoff.

For a common [isothermal sound speed](../../../../isothermal-sound-speed.md) $c_T$, a spherical isothermal equilibrium has $GM/R$ equal to $c_T^2$ times a dimensionless structural factor. Holding that factor fixed gives the [homologous isothermal mass-radius relation](../../../../homologous-isothermal-mass-radius-relation.md)

$$
\boxed{M\propto R\quad(T\text{ and dimensionless structure fixed}).}
$$

For example, the [singular isothermal sphere](../../../../singular-isothermal-sphere.md) has $M(R)=2c_T^2R/G$. A regular finite cloud requires a [pressure-confined isothermal sphere](../../../../pressure-confined-isothermal-sphere.md) or another outer boundary: an unconfined [isothermal sphere](../../../../isothermal-sphere.md) does not end at a finite vacuum radius. Equal [temperature](../../../../temperature-split.md) alone, while allowing arbitrary truncation or density contrast, does not make the coefficient universal.

## ↑ Ancestors (13)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [2013](../../split.md)
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
