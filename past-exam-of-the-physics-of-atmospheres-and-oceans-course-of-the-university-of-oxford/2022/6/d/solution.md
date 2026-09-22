<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

[Coastal Kelvin-wave radiation of long Rossby waves](../../../../coastal-kelvin-wave-radiation-of-long-rossby-waves.md) requires a common [phase](../../../../phase-waves.md) convention to match the two [waves](../../../../wave-split.md). The supplied [Rossby wave](../../../../rossby-wave.md) formula conventionally multiplies $e^{i(k_Rx+\ell_Ry-\omega_Rt)}$, while the coastal expression uses $e^{i(\omega_Kt-\ell_Ky)}$. Since physical fields are real, matching may use the complex-conjugate representative; in either convention the boundary forcing fixes the absolute [frequency](../../../../frequency.md) and alongshore [wavenumber](../../../../wavenumber.md). Thus $|\omega_R|=|\omega_K|$ and $|\ell_R|=|\ell_K|$.

For $k_R^2+\ell_R^2\ll L_d^{-2}$, the [shallow-water Rossby-wave dispersion relation](../../../../shallow-water-rossby-wave-dispersion-relation.md) reduces to

$$
\omega_R\simeq-\beta L_d^2k_R,
\qquad
\boxed{|\omega_K|\simeq\beta|k_R|L_d^2
=\frac{\beta|k_R|g'h_0}{f_0^2}.}
$$

Choosing $k_R>0$ recovers the printed magnitude relation. Both the zonal [phase velocity](../../../../phase-velocity.md) and zonal [group velocity](../../../../group-velocity.md) are approximately $-\beta L_d^2$, so the long [Rossby waves](../../../../rossby-wave.md) carry the coastal signal westwards into the basin.

The coastal condition $|\ell_K|L_d\ll1$ alone does not guarantee a long zonal [wavelength](../../../../wavelength.md). Since $|\omega_K|=c|\ell_K|$, matching requires $|k_R|=c|\ell_K|/(\beta L_d^2)$ and hence the stronger consistency condition

$$
|\ell_K|\ll\frac{\beta L_d}{c},\qquad\text{equivalently}\qquad |\omega_K|\ll\beta L_d.
$$

For example, at $10^\circ$ a coastal [wavenumber](../../../../wavenumber.md) with $|\ell_K|L_d=0.05$ gives $|k_R|L_d\simeq0.56$, which is not asymptotically small even though the meridional [wavelength](../../../../wavelength.md) is long. Thus the source's proposed excitation is possible at sufficiently low [frequency](../../../../frequency.md); it is not an automatic consequence of its meridional long-wave assumption.

At $10^\circ$ N or S the [beta plane](../../../../beta-plane.md) parameter is

$$
\beta=\frac{2\Omega\cos10^\circ}{R_E}
=2.25\times10^{-11}\,\mathrm{m}^{-1}\mathrm{s}^{-1},\qquad
\beta L_d^2\simeq0.225\,\mathrm{m\,s}^{-1}.
$$

Taking a representative Pacific basin width $W\simeq1.5\times10^7$ m gives

$$
\boxed{t_{\rm cross}\simeq\frac W{\beta L_d^2}
=6.65\times10^7\,\mathrm s\simeq2.1\,\mathrm{yr}.}
$$

A width of $1.4$–$1.7\times10^7$ m gives roughly $2.0$–$2.4$ years. This is propagation near $10^\circ$ latitude, not an equatorial $f=0$ calculation. Slow [Rossby wave](../../../../rossby-wave.md) adjustment supplies a basin-scale delay relevant to [El Niño–Southern Oscillation](../../../../el-nino-southern-oscillation.md): changing [thermocline](../../../../thermocline.md) depth can affect later [sea surface temperature](../../../../sea-surface-temperature.md) and coupled wind forcing. Reflection and coupling may help produce interannual memory, but this travel-time estimate alone does not establish a climate oscillation or its period.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
