<h1 id="s25/1/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the optical-depth weighting stipulated in the paper. A jump in the [Planck function](../../../../../planck-function.md) at $\tau_1$ gives $dB/d\tau=(B_1-B_0)\delta(\tau-\tau_1)$, so

$$
\boxed{I_0=\pi\left[B_0+(B_1-B_0)e^{-\tau_1}\right]
=\pi B_0(1-e^{-\tau_1})+\pi B_1e^{-\tau_1}.}
$$

The upper isothermal layer emits $\pi B_0(1-e^{-\tau_1})$ and transmits the lower region's blackbody [spectral irradiance](../../../../../spectral-irradiance.md) with factor $e^{-\tau_1}$. The lower layer and black surface have the same $B_1$, so their combined radiation entering the upper layer is $\pi B_1$, independent of how its emission is divided between the lower gas and surface.

More generally, integration by parts rewrites the supplied expression as

$$
I_0=\pi B(\tau_s)e^{-\tau_s}+\pi\int_0^{\tau_s}B(\tau)e^{-\tau}\,d\tau.
$$

The terms are attenuated surface emission and the atmosphere's own emission. In the original boundary-plus-gradient form, $\pi B_0$ is the isothermal reference flux and the integral corrects for temperature variation below the top. Optical depths of order unity contribute most strongly. These formulas follow the paper's specified exponential weighting; a full angular [radiative transfer](../../../../../radiative-transfer.md) calculation uses ray-angle-dependent optical paths rather than identifying every ray with a vertical path.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [1](../../1.md)
3. [S25](../../../s25.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
