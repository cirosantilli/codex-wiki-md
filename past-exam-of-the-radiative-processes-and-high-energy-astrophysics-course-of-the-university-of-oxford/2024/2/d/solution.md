<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a spherical [star](../../../../star.md) in Newtonian [hydrostatic equilibrium](../../../../hydrostatic-equilibrium.md), the total supporting [pressure](../../../../pressure-split.md) satisfies

$$
\frac{dP}{dr}=-\frac{Gm(r)\rho(r)}{r^2},\qquad P(R)=0,
$$

where zero external [pressure](../../../../pressure-split.md) is the idealized vacuum boundary condition. Substitute the enclosed [mass](../../../../mass.md) from [a](../a.md), set $x=ar$, and integrate inwards:

$$
P(r)=\frac{4\pi G\rho_c^2}{a^2}
\int_{ar}^{\pi}\frac{\sin x(\sin x-x\cos x)}{x^3}\,dx.
$$

The supplied [integral](../../../../integral-split.md) follows directly by differentiating $\tfrac12(\sin x/x)^2$. It yields

$$
\boxed{P(r)=\frac{2\pi G\rho_c^2}{a^2}
\left(\frac{\sin ar}{ar}\right)^2
=\frac{2GR^2}{\pi}\rho(r)^2.}
$$

Thus $P_c=\pi GM^2/(8R^4)$, about $4.42\times10^{14}\,\mathrm{Pa}$ for the [Sun](../../../../sun.md)'s parameters. This is precisely the [equation of state](../../../../equation-of-state.md) of a [polytrope of index one](../../../../polytrope-of-index-one.md).

For nonrelativistic fully ionized [hydrogen](../../../../hydrogen.md) with [electrons](../../../../electron.md) and [protons](../../../../proton.md) at a common [temperature](../../../../temperature-split.md), the [gas pressure](../../../../gas-pressure.md) is $P_g=(n_e+n_p)k_BT=2\rho k_BT/m_p$. If [gas pressure](../../../../gas-pressure.md) dominates, the resulting [temperature](../../../../temperature-split.md) profile is

$$
\boxed{T_g(r)=\frac{m_pP(r)}{2k_B\rho(r)}
=T_c\frac{\sin ar}{ar},\qquad
T_c=\frac{GMm_p}{4Rk_B}.}
$$

Numerically $T_c\simeq5.78\times10^6\,\mathrm K$ for the [Sun](../../../../sun.md)'s parameters, and $T_g$ tends to zero at the idealized outer edge.

If the [photons](../../../../photon.md) are additionally assumed to be in [local thermodynamic equilibrium](../../../../local-thermodynamic-equilibrium.md) with this gas, their [radiation pressure](../../../../radiation-pressure.md) is $a_{\rm rad}T^4/3$, with $a_{\rm rad}=4\sigma_{\rm SB}/c$. The consistent [temperature](../../../../temperature-split.md) is instead the unique nonnegative root of

$$
\boxed{\frac{2\rho(r)k_B}{m_p}T(r)+\frac{a_{\rm rad}}3T(r)^4=P(r).}
$$

The left side is strictly increasing in $T$ for $r<R$, so the root is unique. Evaluating the [radiation pressure](../../../../radiation-pressure.md) at $T_g$ gives at most $P_{\rm rad}/P\simeq6.4\times10^{-4}$ for the [Sun](../../../../sun.md)'s parameters, at the centre; the ratio decreases approximately as $(\sin ar/ar)^2$ outwards. The gas-only profile is consequently an excellent approximation _within this imposed stellar model_.

[Hydrostatic equilibrium](../../../../hydrostatic-equilibrium.md) by itself fixes total [pressure](../../../../pressure-split.md), not how it is divided between gas and radiation. [Thomson scattering](../../../../thomson-scattering.md) alone does not enforce a common gas–radiation [temperature](../../../../temperature-split.md) or a [Planck photon distribution](../../../../planck-photon-distribution.md). Without either neglecting [radiation pressure](../../../../radiation-pressure.md) or specifying the radiation field and its thermodynamic closure, a unique gas [temperature](../../../../temperature-split.md) cannot be inferred from the given [mass density](../../../../density.md) alone.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the radiative processes and high energy astrophysics course of the University of Oxford](../../../split.md)
5. [Radiative processes and high energy astrophysics course of the University of Oxford](../../../../radiative-processes-and-high-energy-astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
