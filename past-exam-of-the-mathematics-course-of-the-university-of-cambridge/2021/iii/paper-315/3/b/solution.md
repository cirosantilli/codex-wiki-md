<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let the atmosphere occupy a thin annulus from $R_p$ to $R_a=R_p+\Delta R$. With mass extinction coefficient $k_\nu$, constant density $\rho$, and the assumed common chord length $l$, its [optical depth](../../../../../../optical-depth.md) is

$$
\tau_\nu=k_\nu\rho l.
$$

The opaque solid planet removes area $\pi R_p^2$, while the annulus removes the fraction $1-e^{-\tau_\nu}$ of the incident [specific intensity](../../../../../../specific-intensity.md). Neglecting limb darkening, the [exoplanet transmission spectrum](../../../../../../exoplanet-transmission-spectrum.md) is therefore

$$
\boxed{D_\nu\equiv1-\frac{F_\nu^{\rm in}}{F_\nu^{\rm out}}
=\frac{R_p^2+(R_a^2-R_p^2)(1-e^{-k_\nu\rho l})}{R_s^2}}.
$$

For a thin annulus,

$$
D_\nu\simeq\left(\frac{R_p}{R_s}\right)^2
+\frac{2R_p\Delta R}{R_s^2}(1-e^{-k_\nu\rho l}).
$$

If the geometrical thickness is estimated as $\Delta R=N_HH$, then the [atmospheric scale height](../../../../../../atmospheric-scale-height.md) is $H=k_BT_p/(\mu m_HGM_p/R_p^2)$. A wavelength-independent $k_\nu$ makes this idealized spectrum flat; real molecular opacities create its features.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 315](../../../paper-315-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
