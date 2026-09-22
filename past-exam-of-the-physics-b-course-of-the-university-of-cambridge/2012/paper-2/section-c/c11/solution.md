<h1 id="section-c/c11/solution">Solution</h1>

↑ **Parent:** [C11](../c11.md)

**Capacity convention.** The printed equation requires $c$ to be [volumetric heat capacity](../../../../../volumetric-heat-capacity.md), in $\mathrm{J\,m^{-3}\,K^{-1}}$. If “[specific heat capacity](../../../../../specific-heat-capacity.md)” means per unit [mass](../../../../../mass.md) instead, the storage term is $\rho_m c\,\partial_tT$ and both denominators in the printed equation must contain $\rho_m c$. This distinction is fixed by dimensions.

For a fixed material region $V$, conservation of thermal [energy](../../../../../energy-split.md) gives the [heat balance with volumetric heat generation](../../../../../heat-balance-with-volumetric-heat-generation.md),

$$
\frac d{dt}\int_VcT\,dV
=-\oint_{\partial V}\mathbf J\cdot\mathbf n\,dS+\int_VH\,dV.
$$

Use the [divergence theorem](../../../../../divergence-theorem.md), $\mathbf J=-\kappa\nabla T$ and constant coefficients. Since the region is arbitrary,

$$
\boxed{c\partial_tT=\kappa\nabla^2T+H,\qquad
\partial_tT=\frac\kappa c\nabla^2T+\frac Hc.}
$$

The [heat](../../../../../heat-split.md) source is power per volume, while $\kappa$ is [thermal conductivity](../../../../../thermal-conductivity.md) rather than [thermal diffusivity](../../../../../thermal-diffusivity.md).

For uniform [electrical conductivity](../../../../../electrical-conductivity.md) and imposed current, current [density](../../../../../density.md) is $j=I/(\pi a^2)$ and [Joule heating](../../../../../joule-heating.md) is $H=j^2/\sigma$. A long, steady, cylindrically symmetric wire therefore satisfies

$$
\frac1s\frac d{ds}\left(s\frac{dT}{ds}\right)=-\frac H\kappa.
$$

Integration gives $T'=-Hs/(2\kappa)+C/s$. Regularity at $s=0$ makes $C=0$, and the surface condition fixes the remaining constant. Thus the [Joule-heated cylindrical wire](../../../../../joule-heated-cylindrical-wire.md) has

$$
\boxed{T(s)=T_0+\frac{I^2}{4\pi^2a^4\kappa\sigma}(a^2-s^2).}
$$

Here $s$ denotes the printed radial coordinate $\rho$ and avoids confusing it with [mass](../../../../../mass.md) [density](../../../../../density.md). The centre is hotter by $I^2/(4\pi^2a^2\kappa\sigma)$.

For the air boundary, the internal flux at $s=a$ is $-\kappa T'(a)=Ha/2$. Equate this to $\alpha[T(a)-T_{\rm air}]$. The [Newton cooling of a Joule-heated wire](../../../../../newton-cooling-of-a-joule-heated-wire.md) gives

$$
\boxed{T(a)=T_{\rm air}+\frac{Ha}{2\alpha}
=T_{\rm air}+\frac{I^2}{2\pi^2a^3\sigma\alpha}.}
$$

Multiplication by circumference $2\pi a$ verifies that surface loss per length equals $I^2/(\pi a^2\sigma)$, the electrical power per length. The full air-cooled profile uses this surface [temperature](../../../../../temperature-split.md) plus the same parabolic interior excess, assuming constant material properties and negligible end losses.

## ↑ Ancestors (14)

1. [C11](../c11.md)
2. [Section C](../../section-c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2012](../../../split.md)
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
