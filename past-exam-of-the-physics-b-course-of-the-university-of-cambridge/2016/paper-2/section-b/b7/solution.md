<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

An electrostatic field calculation begins by specifying the charge information, material response and boundary conditions. In [vacuum](../../../../../vacuum.md), prescribed volume and surface [electric charge](../../../../../electric-charge-split.md) densities can be superposed directly using [Coulomb's law](../../../../../coulomb-s-law.md). For a volume distribution,

$$
\phi(\mathbf r)=\frac1{4\pi\epsilon_0}\int\frac{\rho(\mathbf r')}{|\mathbf r-\mathbf r'|}\,d^3r',\qquad \mathbf E=-\nabla\phi.
$$

Differentiating this [electric potential](../../../../../electric-potential.md) gives the [electric field](../../../../../electric-field-split.md). This is useful for known source distributions, but in the presence of conductors the induced surface [electric charge](../../../../../electric-charge-split.md) is usually an unknown rather than an independently specified input.

[Gauss's law](../../../../../gauss-s-law.md) is especially effective when [symmetry](../../../../../symmetry-physics.md) fixes the direction and magnitude of the [electric field](../../../../../electric-field-split.md) on a suitable closed surface. A spherical charge distribution gives a radial field, an infinitely long uniform line gives a cylindrical field, and a uniform infinite sheet gives a planar field. In an arbitrary geometry, the flux law remains true but does not alone determine the pointwise [electric field](../../../../../electric-field-split.md). A [multipole expansion](../../../../../electric-multipole-expansion.md) is another useful approximation: far from a localized charge distribution, successive monopole, dipole and higher terms separate the effects of total charge and its spatial structure.

For a boundary-value formulation, use the electrostatic equations

$$
\nabla\times\mathbf E=0,\qquad\nabla\cdot\mathbf E=\rho/\epsilon_0.
$$

They imply [Poisson equation](../../../../../poisson-s-equation.md) $\nabla^2\phi=-\rho/\epsilon_0$, or [Laplace equation](../../../../../laplace-equation.md) where $\rho=0$. A conductor in electrostatic equilibrium is an equipotential with zero internal [electric field](../../../../../electric-field-split.md). Its exterior normal [electric field](../../../../../electric-field-split.md) fixes the surface [electric charge](../../../../../electric-charge-split.md) through $E_n=\sigma/\epsilon_0$. One must specify whether each conductor is grounded, maintained at a prescribed [voltage](../../../../../voltage.md), or isolated with prescribed total [electric charge](../../../../../electric-charge-split.md).

[Uniqueness of Poisson equation](../../../../../uniqueness-of-poisson-equation.md) justifies methods that construct a convenient candidate solution. With fixed boundary [electric potential](../../../../../electric-potential.md) and suitable behaviour at infinity, a solution satisfying the field equation is the solution. With normal-derivative boundary conditions, the source and flux must be compatible, and the [electric potential](../../../../../electric-potential.md) is determined only up to an additive constant.

For example, a point charge $q$ a distance $h$ above a grounded infinite plane has the same upper-half-space [electric potential](../../../../../electric-potential.md) as $q$ and a mirrored [image charge](../../../../../image-charge.md) $-q$ below it. Their potentials cancel on the plane. The image is a mathematical source in the excluded region, not a second physical charge. [Separation of variables](../../../../../separation-of-variables.md) similarly constructs solutions suited to rectangular, cylindrical or spherical boundaries; matching coefficients enforces the prescribed boundary data.

In dielectrics, the distinction between total and [free charge](../../../../../free-charge.md) is essential. In a linear isotropic material,

$$
\mathbf D=\epsilon(\mathbf r)\mathbf E,\qquad \boxed{\nabla\cdot[\epsilon(\mathbf r)\nabla\phi]=-\rho_f.}
$$

Only where [permittivity](../../../../../permittivity-split.md) is constant may this be reduced to $\nabla^2\phi=-\rho_f/\epsilon$. At an ordinary interface, $\phi$ and the tangential [electric field](../../../../../electric-field-split.md) are continuous, while the jump in normal [electric displacement field](../../../../../electric-displacement-field.md) is the free surface charge. Applying [Gauss's law](../../../../../gauss-s-law.md) to total charge with $\epsilon_0$, or its displacement-field form to [free charge](../../../../../free-charge.md), gives consistent descriptions; mixing their sources and permittivities does not.

A useful interface example is the [image charge at a dielectric interface](../../../../../image-charge-at-a-dielectric-interface.md). If $q$ lies in medium 1, the source-side potential is represented by

$$
\phi_1=\frac1{4\pi\epsilon_1}\left(\frac q{r_1}+\frac{q'}{r_2}\right),\qquad \boxed{q'=q\frac{\epsilon_1-\epsilon_2}{\epsilon_1+\epsilon_2}},
$$

where $r_1$ is distance to the real charge and $r_2$ to its mirrored position. The other-side potential can be written $\phi_2=q_t/(4\pi\epsilon_2r_1)$, where $q_t=2\epsilon_2q/(\epsilon_1+\epsilon_2)$. Continuity of $\phi$ and of normal $\mathbf D$ fixes both coefficients. The equal-[permittivity](../../../../../permittivity-split.md) limit gives no image; the conductor limit $\epsilon_2\to\infty$ gives $q'\to-q$.

For a sphere of radius $a$ and relative [permittivity](../../../../../permittivity-split.md) $\epsilon_r$ in a uniform external [electric field](../../../../../electric-field-split.md) $\mathbf E_0$, matching the spherical solutions gives a uniform internal [electric field](../../../../../electric-field-split.md) and an external induced [electric dipole moment](../../../../../electric-dipole-moment.md):

$$
\boxed{\mathbf E_{\rm in}=\frac3{\epsilon_r+2}\mathbf E_0,\qquad \mathbf p=4\pi\epsilon_0a^3\frac{\epsilon_r-1}{\epsilon_r+2}\mathbf E_0.}
$$

This illustrates how a material boundary modifies an otherwise simple applied [electric field](../../../../../electric-field-split.md).

For complex boundaries or spatially varying materials, [finite difference methods](../../../../../finite-difference-method.md) or the [finite element method](../../../../../finite-element-method-split.md) solve the same [boundary value problem](../../../../../boundary-value-problem-split.md) numerically. A sound calculation checks its boundary conditions, charge or flux balance and convergence with mesh refinement. The governing equations, source classification and uniqueness argument remain the organizing principles even when an analytic formula is unavailable.

## ↑ Ancestors (14)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2016](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
