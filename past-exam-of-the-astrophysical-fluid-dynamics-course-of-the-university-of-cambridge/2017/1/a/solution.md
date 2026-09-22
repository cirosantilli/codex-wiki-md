<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume a constant downward [gravitational acceleration](../../../../gravitational-acceleration.md) $g$, constant composition, and an [ideal gas law](../../../../ideal-gas-law.md) $p=\rho\mathcal R T$, where $\mathcal R=k_B/(\mu m_u)$ is the gas constant per unit mass. Here $m_u$ is the [unified atomic mass unit](../../../../dalton-unit.md); this convention makes the specified [mean molecular weight](../../../../mean-molecular-weight.md) dimensionless. [Hydrostatic equilibrium](../../../../hydrostatic-equilibrium.md) gives

$$
\frac{dp}{dz}=-\rho g=-\frac{pg}{\mathcal R(T_0-\alpha z)},\qquad
\frac{d\ln p}{dz}=-\frac{g}{\mathcal R(T_0-\alpha z)}.
$$

Integrating from sea level yields

$$
\frac{p(z)}{p(0)}=\left(\frac{T_0-\alpha z}{T_0}\right)^{g/(\mathcal R\alpha)}.
$$

Dividing by the [temperature](../../../../temperature-split.md) ratio gives the [hydrostatic atmosphere with a constant temperature lapse rate](../../../../hydrostatic-atmosphere-with-a-constant-temperature-lapse-rate.md):

$$
\boxed{\rho(z)=\rho(0)\left(1-\frac{\alpha z}{T_0}\right)^{\mu m_ug/(k_B\alpha)-1}.}
$$

The model requires $T_0-\alpha z>0$ and is used here only within the troposphere.

Convert the [atmospheric lapse rate](../../../../lapse-rate-atmosphere.md) to $\alpha=6.5\times10^{-3}\ \mathrm{K\,m^{-1}}$. At $11\ \mathrm{km}$, $T=228.5\ \mathrm K$. With $g=9.81\ \mathrm{m\,s^{-2}}$, $k_B=1.380649\times10^{-23}\ \mathrm{J\,K^{-1}}$, $m_u\simeq1.66054\times10^{-27}\ \mathrm{kg}$ and $\mu=28$, the density exponent is $4.0825$. Hence

$$
\boxed{\frac{\rho(11\ \mathrm{km})}{\rho(0)}
=\left(\frac{228.5}{300}\right)^{4.0825}\simeq0.329.}
$$

The [mass density](../../../../density.md) is therefore approximately one third of its sea-level value in this model.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
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
