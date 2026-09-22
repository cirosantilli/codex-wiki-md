<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The usual [Pressure-opacity zones of a Shakura--Sunyaev thin disk](../../../../../../pressure-opacity-zones-of-a-shakura-sunyaev-thin-disk.md), in order of increasing cylindrical radius, are an inner region dominated by [radiation pressure](../../../../../../radiation-pressure.md) and [electron-scattering opacity](../../../../../../electron-scattering-opacity.md), a middle region dominated by [gas pressure](../../../../../../gas-pressure.md) and [electron-scattering opacity](../../../../../../electron-scattering-opacity.md), and an outer region dominated by [gas pressure](../../../../../../gas-pressure.md) and the [Kramers' opacity law](../../../../../../kramers-opacity-law.md), often approximated by [free-free opacity](../../../../../../free-free-opacity.md). The boundaries depend on mass, [mass accretion rate](../../../../../../mass-accretion-rate.md), and the [alpha disk](../../../../../../alpha-disk.md) viscosity parameter. At sufficiently large radius, [accretion-disk self-gravity](../../../../../../accretion-disk-self-gravity.md) or changes in ionization can invalidate this three-zone model.

For the inner region write

$$
\Omega_K^2=\frac{GM_{\rm BH}}{R^3},\qquad
f(R)=1-\sqrt{\frac{R_*}{R}},\qquad
F(R)=\frac{3GM_{\rm BH}\dot m}{8\pi R^3}f(R).
$$

Here $F$ is the [standard thin-disk dissipation flux](../../../../../../standard-thin-disk-dissipation-flux.md) through one face, and $R_*$ is the [innermost stable circular orbit](../../../../../../innermost-stable-circular-orbit.md) treated as a zero-torque inner boundary. The given factor $1/2$ in the dissipation rate is appropriate to one face. For [Keplerian rotation](../../../../../../keplerian-disk.md), it is $(9/8)\nu\Sigma\Omega_K^2$.

Let $H$ denote the [disk scale height](../../../../../../disk-scale-height.md) or vertical half-thickness, not the full thickness. In vertical [hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md), the leading vertical acceleration is $\Omega_K^2z$, so a one-zone estimate gives

$$
P_c\simeq\rho_c\Omega_K^2H^2
\simeq\frac12\Sigma\Omega_K^2H.
$$

In the inner zone, $P_c\simeq P_{\rm rad,c}=a_{\rm rad}T_c^4/3$. For an [optically thick medium](../../../../../../optically-thick-medium.md) with constant [electron-scattering opacity](../../../../../../electron-scattering-opacity.md), [radiative diffusion](../../../../../../radiative-diffusion.md) gives the emergent one-face flux

$$
F\simeq\frac{2ca_{\rm rad}T_c^4}{3\kappa_{\rm es}\Sigma}
=\frac{2cP_c}{\kappa_{\rm es}\Sigma}
\simeq\frac{c\Omega_K^2H}{\kappa_{\rm es}}.
$$

Equivalently, combine $F=-c(\kappa_{\rm es}\rho)^{-1}dP_{\rm rad}/dz$ with vertical pressure balance. Equating the radiative flux to the dissipated flux yields the [radiation-supported inner-disk height](../../../../../../radiation-supported-inner-disk-height.md):

$$
\boxed{H(R)\simeq\frac{3\kappa_{\rm es}\dot m}{8\pi c}
\left(1-\sqrt{\frac{R_*}{R}}\right).}
$$

Order-unity vertical-profile factors depend on the precise height convention. The central mass cancels at fixed physical [mass accretion rate](../../../../../../mass-accretion-rate.md), because both vertical gravity and local dissipation are proportional to $GM_{\rm BH}/R^3$.

If $\dot m_{\rm Edd}=L_{\rm Edd,es}/(\eta_0c^2)$ and $r_g=GM_{\rm BH}/c^2$, this can also be written

$$
\boxed{H(R)\simeq\frac{3}{2\eta_0}
\frac{\dot m}{\dot m_{\rm Edd}}r_g f(R).}
$$

The radiation-supported height rises from the formal zero at $R_*$ toward the approximately constant value $H_0=3\kappa_{\rm es}\dot m/(8\pi c)$. That zero is not a reliable description of the physical plunging region: the radiation-dominated approximation and the Newtonian zero-torque formula fail very close to the inner edge.

Beyond the inner zone, the height grows slowly with radius rather than staying on that plateau forever. Far from the inner boundary, the standard gas-pressure scalings give $H\propto R^{21/20}$ in the electron-scattering zone and $H\propto R^{9/8}$ in the Kramers zone. These follow from $H\propto T_c^{1/2}R^{3/2}$ with $T_c\propto R^{-9/10}$ and $R^{-3/4}$, respectively. A schematic profile is

```
vertical half-thickness H
  ^
  |                                               / outer gas/Kramers
  |                                          ____/
  |                                     ____/ middle gas/scattering
  |              ______________________/
  |          ___/ inner radiation/scattering plateau
  |       __/
  |     _/
  +----|----------------------------------------------> radius R
      R_*              zone boundaries are schematic
```

The height formula also tests the [thin disk](../../../../../../thin-disk.md) assumption. For a nonrotating hole with $R_*=6r_g$, the largest $H/R$ in this inner approximation occurs at $R=(9/4)R_*$. At $\dot m=\dot m_{\rm Edd}$ and $\eta_0=0.1$, it is about $0.37$, so a disc this close to the conventional [Eddington accretion rate](../../../../../../eddington-accretion-rate.md) is only marginally thin. [Slim accretion disk](../../../../../../slim-accretion-disk.md) effects and advected heat can then matter.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 347](../../../paper-347-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
