<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\delta_T$ be the thickness of the [thermal boundary layer](../../../../../../thermal-boundary-layer.md) immediately below $z=h$, let $\nu$ be the [kinematic viscosity](../../../../../../kinematic-viscosity.md), let $\kappa$ be the [thermal diffusivity](../../../../../../thermal-diffusivity.md), and let $\operatorname{Ra}_c$ be the critical local [Rayleigh number](../../../../../../rayleigh-number.md). The density contrast driving the boundary layer follows from the [density anomaly of water](../../../../../../density-anomaly-of-water.md):

$$
\Delta\rho
=\rho(T_h)-\rho(T_w)
=\rho_m\alpha
\left[(T_w-T_m)^2-(T_h-T_m)^2\right].
$$

A [Local Rayleigh-number closure](../../../../../../local-rayleigh-number-closure.md) sets

$$
\frac{g\Delta\rho\,\delta_T^3}
{\rho_m\nu\kappa}
=\operatorname{Ra}_c,
$$

and therefore

$$
\delta_T=
\left[
\frac{\operatorname{Ra}_c\nu\kappa}
{g\alpha\{(T_w-T_m)^2-(T_h-T_m)^2\}}
\right]^{1/3}.
$$

By [Fourier's law](../../../../../../fourier-s-law.md), the upward [heat flux](../../../../../../heat-flux-density.md) through this layer is

$$
\boxed{
F_c=k(T_w-T_h)
\left[
\frac{g\alpha\{(T_w-T_m)^2-(T_h-T_m)^2\}}
{\operatorname{Ra}_c\nu\kappa}
\right]^{1/3}},
$$

where $k$ is the water's [thermal conductivity](../../../../../../thermal-conductivity.md). This expression applies while the quantity inside braces is positive.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
