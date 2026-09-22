<h1 id="s02/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For spherical [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md), the [stellar structure equations](../../../../../stellar-structure-equations.md) include

$$
\frac{dP}{dr}=-\frac{Gm(r)\rho(r)}{r^2},\qquad \frac{dm}{dr}=4\pi r^2\rho(r).
$$

Eliminate $\rho$ to obtain $dP/dm=-Gm/(4\pi r^4)$. Since $r(m)<R_\odot$ through the interior, integration gives

$$
P_c-P_s=\int_0^{M_\odot}\frac{Gm}{4\pi r(m)^4}\,dm>\frac{G}{4\pi R_\odot^4}\int_0^{M_\odot}m\,dm.
$$

With negligible surface [pressure](../../../../../pressure-split.md), this proves

$$
\boxed{P_{c,\odot}>\frac{GM_\odot^2}{8\pi R_\odot^4}\simeq4.48\times10^{13}\,\mathrm{Pa}.}
$$

This is a conservative lower bound; concentrating [mass](../../../../../mass.md) near the centre increases the required [pressure](../../../../../pressure-split.md).

For the [temperature](../../../../../temperature-split.md) inference assume predominantly [ideal gas](../../../../../ideal-gas-split.md) support, a nearly fully ionized hydrogen–helium mixture with [mean molecular weight](../../../../../mean-molecular-weight.md) $\mu\simeq0.61$, and the hottest region at the centre. A rigorous scale estimate follows from the [stellar virial theorem](../../../../../stellar-virial-theorem.md), rather than substituting the mean [mass density](../../../../../density.md) for the unknown central [mass density](../../../../../density.md). With negligible surface [pressure](../../../../../pressure-split.md),

$$
3\int P\,dV=-W,\qquad -W=\int_0^{M_\odot}\frac{Gm}{r(m)}\,dm>\frac{GM_\odot^2}{2R_\odot}.
$$

The [ideal gas law](../../../../../ideal-gas-law.md) gives $\int P\,dV=k_B\int T\,dm/(\mu m_p)$. The mass-weighted mean [temperature](../../../../../temperature-split.md) consequently obeys

$$
\boxed{T_c\ge\langle T\rangle_M>\frac{\mu m_pGM_\odot}{6k_BR_\odot}\simeq2.35\times10^6\,\mathrm K.}
$$

This establishes several million [kelvin](../../../../../kelvin.md) under the stated physical assumptions. The central [pressure](../../../../../pressure-split.md) inequality alone does not give a central [temperature](../../../../../temperature-split.md) bound without an [equation of state](../../../../../equation-of-state.md) and information about [mass density](../../../../../density.md) or an integrated argument.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [S02](../../../s02.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the short options paper of the physics Prelims of the University of Oxford](../../../../split.md)
6. [Short options paper of the physics Prelims of the University of Oxford](../../../../../short-options-paper-of-the-physics-prelims-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
