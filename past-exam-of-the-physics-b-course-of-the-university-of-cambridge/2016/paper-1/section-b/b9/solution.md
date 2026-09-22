<h1 id="section-b/b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

For a linear nondispersive medium with real absolute [permittivity](../../../../../permittivity-split.md) $\epsilon_a=\epsilon\epsilon_0$ and permeability $\mu_0$, instantaneous field [energy density](../../../../../energy-density.md) and [energy](../../../../../energy-split.md) flux are

$$
u=\frac12\epsilon_aE^2+\frac{B^2}{2\mu_0},\qquad \mathbf N=\mathbf E\times\mathbf H,
$$

with local balance $\partial_tu+\nabla\cdot\mathbf N=-\mathbf J\cdot\mathbf E$. [energy](../../../../../energy-split.md) stored locally and [energy](../../../../../energy-split.md) passing through a surface are distinct: integrating the balance relates their rates and the [power](../../../../../power.md) given to charges.

Between the coaxial conductors, cylindrical Gauss and Ampère laws give

$$
\boxed{\mathbf E=\frac{V}{r\ln(b/a)}\widehat{\mathbf r},\qquad \mathbf B=\frac{\mu_0I}{2\pi r}\widehat{\boldsymbol\phi},\qquad a<r<b.}
$$

The inner line charge is $\lambda=2\pi\epsilon_a V/\ln(b/a)$, so the [capacitance](../../../../../capacitance.md) per [length](../../../../../length.md) is $C=2\pi\epsilon_a/\ln(b/a)$. Integrating magnetic [energy](../../../../../energy-split.md) over the annulus gives $\int B^2(2\pi r\,dr)/(2\mu_0)=\mu_0I^2\ln(b/a)/(4\pi)=LI^2/2$, hence $L=\mu_0\ln(b/a)/(2\pi)$. Thus

$$
\boxed{Z_0=\sqrt{\frac LC}=\frac{\ln(b/a)}{2\pi}\sqrt{\frac{\mu_0}{\epsilon\epsilon_0}}.}
$$

These are per-length parameters for ideal conductors, excluding internal magnetic penetration.

Now let the [voltage](../../../../../voltage.md) and current [amplitudes](../../../../../wave-amplitude.md) be $V_0,I_0$ and multiply both transverse fields by $e^{i(kz-\omega t)}$. Their divergences vanish in the annular [dielectric](../../../../../dielectric.md). The two nontrivial curl equations reduce to

$$
k\widetilde E_r=\omega\widetilde B_\phi,\qquad k\widetilde B_\phi=\omega\mu_0\epsilon_a\widetilde E_r.
$$

Consequently **both $k^2=\omega^2\mu_0\epsilon_a$ and $V_0=Z_0I_0$ are required for a forward [wave](../../../../../wave-split.md)**. Arbitrary independent static $V$ and $I$ cannot acquire the same forward-wave factor and still satisfy [Maxwell's equations](../../../../../maxwell-equations-split.md). This [TEM travelling-wave voltage-current relation](../../../../../tem-travelling-wave-voltage-current-relation.md) and the dispersion constraint identify the [transverse electromagnetic mode](../../../../../transverse-electromagnetic-mode.md) and its [speed](../../../../../speed.md) $v_p=1/\sqrt{LC}$.

For the travelling [wave](../../../../../wave-split.md), $\langle N_z\rangle=\operatorname{Re}(V_0I_0^*)/[4\pi r^2\ln(b/a)]$. Integrating over the [dielectric](../../../../../dielectric.md) annulus yields

$$
\boxed{\langle P\rangle=\frac12\operatorname{Re}(V_0I_0^*)=\frac{|V_0|^2}{2Z_0}=\frac{Z_0|I_0|^2}{2}.}
$$

This is the familiar circuit [power](../../../../../power.md), carried here through the [dielectric](../../../../../dielectric.md) rather than through the ideal metal. In [root mean square](../../../../../root-mean-square.md) notation it is $V_{\rm rms}I_{\rm rms}$ for the forward lossless [wave](../../../../../wave-split.md); the corresponding static fields give $VI$ without a time-average factor. The average line [energy](../../../../../energy-split.md) is $(C|V_0|^2+L|I_0|^2)/4=C|V_0|^2/2$, whose product with [wave](../../../../../wave-split.md) [speed](../../../../../speed.md) agrees with the [power](../../../../../power.md).

Finite conductor resistance requires a small longitudinal electric field to drive current. Its [cross product](../../../../../cross-product.md) with the azimuthal [magnetic field](../../../../../magnetic-field-split.md) produces a radial Poynting component into each conductor: inward radially at the inner conductor and outward radially into the outer conductor. This [Poynting flux into lossy coaxial conductors](../../../../../poynting-flux-into-lossy-coaxial-conductors.md) explains why forward [power](../../../../../power.md) decreases along the cable as [energy](../../../../../energy-split.md) becomes [heat](../../../../../heat-split.md) in the metal. The mode is then only approximately TEM; strictly zero longitudinal electric field would be inconsistent with resistive current.

## ↑ Ancestors (14)

1. [B9](../b9.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
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
