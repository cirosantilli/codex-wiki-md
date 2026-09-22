<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Analyze a local temperature perturbation at fixed radius and fixed [surface density of a disk](../../../../../../surface-density-of-a-disk.md) $\Sigma$. The [thermal timescale of an accretion disk](../../../../../../thermal-timescale-of-an-accretion-disk.md) is shorter than its [viscous timescale](../../../../../../viscous-timescale.md), so mass redistribution is negligible during the perturbation. Let $Q^+$ be viscous heating and $Q^-$ radiative cooling, measured consistently through one face or both faces, and define net cooling by $\dot Q=Q^--Q^+$. A temperature increase is unstable if it decreases net cooling.

With [gas pressure](../../../../../../gas-pressure.md) dominant, vertical [hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md) and the [ideal gas](../../../../../../ideal-gas.md) law give

$$
c_s^2\propto T_c,\qquad H\propto T_c^{1/2},\qquad
\rho_c\sim\frac{\Sigma}{2H}\propto T_c^{-1/2}.
$$

For the [alpha disk](../../../../../../alpha-disk.md) prescription with temperature-independent $\alpha$, $\nu=\alpha c_sH\propto T_c$, and the [Keplerian rotation](../../../../../../keplerian-disk.md) heating law is

$$
Q^+=\frac98\nu\Sigma\Omega_K^2\propto T_c.
$$

One must not hold the steady-state $\dot m$ fixed while perturbing the temperature: the stress and heating respond through $\nu$, even though $\Sigma$ is temporarily fixed.

At an equilibrium temperature $T_0$ where $Q^+=Q^-=Q_0$, if $Q^-\propto T_c^q$ and $Q^+\propto T_c$, then

$$
\left.\frac{d\dot Q}{dT_c}\right|_{T_0}
=(q-1)\frac{Q_0}{T_0}.
$$

The cooling exponent therefore decides the sign.

For hot, ionized, [optically thin](../../../../../../optically-thin-medium.md) gas, the usual intended cooling model is [thermal bremsstrahlung](../../../../../../thermal-bremsstrahlung.md), whose volume emissivity scales as $\rho^2T_c^{1/2}$. Integrated vertically,

$$
Q^-_{\rm ff}\propto H\rho_c^2T_c^{1/2}
\propto\frac{\Sigma^2}{H}T_c^{1/2}\propto T_c^0.
$$

Thus $q=0$, and

$$
\boxed{\frac{d\dot Q}{dT_c}=-\frac{Q_0}{T_0}<0:
\quad\text{the optically thin bremsstrahlung branch is unstable}.}
$$

A hotter annulus expands vertically, lowering its density enough to offset the direct increase in bremsstrahlung emission; viscous heating still rises.

For an [optically thick medium](../../../../../../optically-thick-medium.md) with the [Kramers' opacity law](../../../../../../kramers-opacity-law.md), $\kappa\propto\rho_cT_c^{-7/2}\propto T_c^{-4}$ at fixed $\Sigma$. Thermalized [radiative diffusion](../../../../../../radiative-diffusion.md) gives

$$
Q^-\propto\frac{T_c^4}{\kappa\Sigma}\propto T_c^8,
\qquad
\boxed{\frac{d\dot Q}{dT_c}=7\frac{Q_0}{T_0}>0:
\quad\text{the gas-pressure Kramers branch is stable}.}
$$

Its falling opacity lets a hotter annulus radiate much more efficiently.

For an [optically thick medium](../../../../../../optically-thick-medium.md) with dominant [electron-scattering opacity](../../../../../../electron-scattering-opacity.md), $\kappa$ is nearly independent of temperature. Provided enough true absorption is present to thermalize the radiation,

$$
Q^-\propto T_c^4,
\qquad
\boxed{\frac{d\dot Q}{dT_c}=3\frac{Q_0}{T_0}>0:
\quad\text{the gas-pressure electron-scattering branch is stable}.}
$$

This conclusion differs from the [thermal instability of a radiation-pressure-dominated alpha disk](../../../../../../thermal-instability-of-a-radiation-pressure-dominated-alpha-disk.md), where the heating has a different temperature dependence. The question explicitly excludes that pressure regime.

The first conclusion needs its cooling assumption stated. $T>10^4\,\mathrm K$ alone does not guarantee that [thermal bremsstrahlung](../../../../../../thermal-bremsstrahlung.md) dominates; atomic-line cooling, ionization changes, external illumination, or energy advection can change the answer. For a general optically thin emissivity $\rho^2\Lambda(T_c)$, the corresponding exponent is

$$
q=\frac{d\log\Lambda}{d\log T_c}-\frac12.
$$

Accordingly, under the same fixed-$\Sigma$ alpha prescription,

$$
\boxed{\text{optically thin thermal stability requires }
\frac{d\log\Lambda}{d\log T_c}>\frac32.}
$$

The unstable/stable/stable classification is the standard free-free/diffusion answer, rather than a universal result specified by temperature and optical depth alone.

## ↑ Ancestors (11)

1. [B](../b.md)
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
