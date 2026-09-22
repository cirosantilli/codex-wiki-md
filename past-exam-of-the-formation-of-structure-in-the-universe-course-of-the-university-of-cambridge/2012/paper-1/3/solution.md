<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The normalized [cycloid](../../../../cycloid.md) has

$$
\frac{R_s}{R_m}=\frac{1-\cos\eta}{2},\qquad
\frac{t}{t_m}=\frac{\eta-\sin\eta}{\pi}.
$$

The initially expanding perturbation reaches maximum radius at $\eta=\pi$, $t=t_m$, then formally collapses to zero radius at $\eta=2\pi$, $t=2t_m$. A finite virialized object is assigned the conventional formation epoch **$t_f=2t_m$**; random motions replace the pressureless point-collapse singularity. The [cycloid](../../../../cycloid.md) alone does not describe that relaxation.

<a id="3/image-spherical-collapse-history"></a>
![](../../../../past-exam-of-the-formation-of-structure-in-the-universe-course-of-the-university-of-cambridge/2012/paper-1-collapse-history.png)

**[Figure 2](#3/image-spherical-collapse-history). Spherical-collapse history**.

For the standard top-hat [virialization](../../../../virialization.md) estimate, write $U=-C_GGM^2/R$ and retain the same gravitational structure factor $C_G$ at turnaround and final equilibrium. The coherent [kinetic energy](../../../../kinetic-energy.md) vanishes at turnaround, whereas the [virial theorem](../../../../virial-theorem.md) gives $2K_v+U_v=0$ in the final isolated equilibrium. [conservation of energy](../../../../conservation-of-energy.md) gives

$$
U_m=K_v+U_v=\frac{U_v}{2},
\qquad\boxed{R_v=R_m/2}.
$$

The final [density](../../../../density.md) is eight times the turnaround [density](../../../../density.md). Meanwhile $\bar\rho\propto a^{-3}\propto t^{-2}$, so $\bar\rho(t_f)=\bar\rho(t_m)/4$. The [Einstein-de Sitter virial overdensity](../../../../einstein-de-sitter-virial-overdensity.md) follows by combining these factors with the supplied turnaround contrast:

$$
\boxed{\Delta_f=8\times4\left(\frac{3\pi}{4}\right)^2
=18\pi^2\simeq177.65\approx200,}
\qquad
\boxed{\rho_v=\Delta_f\rho_0(1+z_f)^3.}
$$

The value 200 is a convenient rounded overdensity convention, not exactly the Einstein-de Sitter result.

The [virial radius of a dark-matter halo](../../../../virial-radius-of-a-dark-matter-halo.md) follows from $M_v=4\pi R_v^3\rho_v/3$:

$$
\boxed{R_v=
\left(\frac{3M_v}{4\pi\Delta_f\rho_0}\right)^{1/3}
\frac1{1+z_f}.}
$$

The [hydrostatic temperature of an inverse-square halo](../../../../hydrostatic-temperature-of-an-inverse-square-halo.md) follows from [hydrostatic equilibrium](../../../../hydrostatic-equilibrium.md) and the [ideal gas law](../../../../ideal-gas-law.md):

$$
\frac{dP}{dr}=-\rho_g\frac{GM(r)}{r^2},\qquad
P=\frac{\rho_gk_BT_v}{\mu}.
$$

Since $\rho_g\propto r^{-2}$ and $M(r)=M_vr/R_v$, cancellation of $\rho_g/r$ gives $2k_BT_v/\mu=GM_v/R_v$. Therefore

$$
\boxed{T_v=\frac{GM_v\mu}{2k_BR_v}
=\frac{GM_v^{2/3}\mu}{2k_B}
\left(\frac{4\pi\Delta_f\rho_0}{3}\right)^{1/3}(1+z_f).}
$$

Here $\mu$ is a dimensionful [mean particle mass](../../../../mean-particle-mass.md), as specified in the paper; a [dimensionless](../../../../dimensionless-quantity.md) [mean molecular weight](../../../../mean-molecular-weight.md) would need multiplication by a particle-mass unit. The isothermal interior is a further halo idealization, not an exact continuation of the uniform top-hat profile used in the virial-overdensity estimate. Changing its gravitational structure factor in a literal [energy](../../../../energy-split.md) comparison would change the turnaround-radius relation.

The [formation redshift from halo mean density](../../../../formation-redshift-from-halo-mean-density.md) uses the cluster data, which imply $\rho_v=3M_v/(4\pi R_v^3)=5.37148\times10^{13}M_\odot\,\mathrm{Mpc}^{-3}$. Thus, using the requested rounded convention,

$$
\boxed{1+z_f=\left(\frac{3M_v}{4\pi R_v^3\Delta_f\rho_0}\right)^{1/3}
=1.91908,\qquad z_f\simeq0.92\quad(\Delta_f=200).}
$$

Using $18\pi^2$ instead gives $z_f\simeq1.00$. In the Einstein-de Sitter time scaling the rounded-convention result is $t_f/t_0=(1+z_f)^{-3/2}\simeq0.376$. Directly from the [mass](../../../../mass.md) and radius,

$$
\boxed{T_v=2.34478\times10^8
\left(\frac{\mu}{m_p}\right)\mathrm K.}
$$

For the estimate, take [mean particle mass](../../../../mean-particle-mass.md) $\mu=0.6m_p$, appropriate approximately to a [hydrogen](../../../../hydrogen.md)-[helium](../../../../helium.md) mixture with complete [ionization](../../../../ionization.md). This gives **$T_v\simeq1.41\times10^8\,\mathrm K$**, or $k_BT_v\simeq12.1\,\mathrm{keV}$. The composition choice is additional input, not a value supplied by the examination; the boxed expression retains the result for any $\mu$.

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2012](../../split.md)
4. [Past exam of the formation of Structure in the Universe course of the University of Cambridge](../../../split.md)
5. [Formation of Structure in the Universe course of the University of Cambridge](../../../../formation-of-structure-in-the-universe-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
