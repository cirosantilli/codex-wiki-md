<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [etendue](../../../../etendue.md) is the area–solid-angle acceptance of a ray bundle, more generally $\mathcal G=n_{
m opt}^2\int\cos\theta\,dA\,d\Omega$. In an ideal lossless optical system it is conserved. Increasing pupil [area](../../../../surface-area.md) increases accepted power only together with the appropriate field and detector cone; passive optics cannot arbitrarily increase [radiance](../../../../radiance.md). For a small nadir pixel here, $A\Omega$ denotes entrance-pupil area times the solid angle of its surface footprint.

Choose $1.00$–$1.03\,\mu\mathrm m$ within the surface-sensitive window. A representative band-mean total [radiance](../../../../radiance.md) read from the original blue curve is $\bar L_\lambda\simeq4\,\mu\mathrm W\,\mathrm{cm^{-2}\,sr^{-1}\,\mu m^{-1}}$, uncertain at roughly the tens-of-per-cent level. Its band integral is

$$
\mathcal L\equiv\int L_\lambda\,d\lambda\simeq4(0.03)\times10^{-2}=1.2\times10^{-3}\,\mathrm{W\,m^{-2}\,sr^{-1}}.
$$

The provided SNR formula depends on $L\Delta\nu$ only through this band integral. If $\nu$ is wavenumber, the selected band spans about $291\,\mathrm{cm^{-1}}$ and $L_\nu\,d\nu=L_\lambda|d\lambda|$; numerical radiance densities in the two coordinates must not be mixed. Convert the [specific detectivity](../../../../specific-detectivity.md) to SI: $D^*=5\times10^9\,\mathrm{m\,Hz^{1/2}\,W^{-1}}$ and $\sqrt a=2\times10^{-4}\,\mathrm m$. Using the footprint dwell time from part (c),

$$
(A\Omega)_{\min}=\frac{50\sqrt a}{\mathcal L\tau D^*\sqrt{\Delta t}}=1.40\times10^{-8}\,\mathrm{m^2\,sr}.
$$

A square $200\,\mathrm m$ footprint at altitude $259\,\mathrm{km}$ subtends $\Omega\simeq(200/259000)^2=5.96\times10^{-7}\,\mathrm{sr}$. Thus the collecting [area](../../../../surface-area.md) and circular aperture diameter are

$$
\boxed{A\gtrsim0.0234\,\mathrm{m^2},\qquad D_{\rm tel}\gtrsim\sqrt{4A/\pi}\simeq0.17\,\mathrm m.}
$$

The [Rayleigh criterion](../../../../rayleigh-criterion.md) independently requires only $D\gtrsim1.22\lambda/(200/h)\simeq1.6\,\mathrm{mm}$ at $1.015\,\mu\mathrm m$, so the noise requirement dominates diffraction. The $200\,\mu\mathrm m$ detector size corresponds to focal length about $0.259\,\mathrm m$ for this pixel field. This assumes one detector footprint per stated feature size; stricter spatial sampling would need smaller footprints and a revised photon budget.

The estimate assumes a clear, non-scattering atmosphere as in the graph, a night-side or otherwise isolated thermal signal, negligible extra stray-light and read-noise penalties beyond the supplied detectivity, and transmission $0.7$ for the instrument alone. Atmospheric attenuation is already included in the plotted incoming radiance. The selected band has little atmospheric-only signal, but actual hot-spot detection concerns contrast relative to the background: SNR $50$ on total radiance is not a guarantee for an arbitrarily small temperature anomaly. An illustrative radiance range $3$–$5$ in the plotted units would give diameters about $0.20$–$0.15\,\mathrm m$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
