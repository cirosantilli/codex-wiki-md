<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

**Detector noise and graphical reading.** [Noise-equivalent power](../../../noise-equivalent-power.md) specifies the incident optical power producing signal-to-noise ratio one, with the electrical bandwidth and averaging convention stated. A spectral NEP has units $\mathrm{W\,Hz^{-1/2}}$; a band-integrated NEP has units W. [Specific detectivity](../../../specific-detectivity.md) normalizes the latter by detector area and noise bandwidth:

$$
\boxed{D_* =\frac{\sqrt{A_d\Delta f}}{\mathrm{NEP}_{\Delta f}}=\frac{\sqrt{A_d}}{\mathrm{NEP}_{\rm spectral}}}.
$$

Its usual unit, the Jones, is $\mathrm{cm\,Hz^{1/2}\,W^{-1}}$. Removing the expected square-root area and bandwidth dependence helps compare different detector sizes and readout bandwidths, provided noise conditions and spectral response are comparable. This does not normalize away every background, temperature or implementation difference.

Reading the native embedded voltage plot gives approximate means $V_C\simeq0.331\ \mathrm V$, $V_S\simeq0.406\ \mathrm V$ and $V_H\simeq0.493\ \mathrm V$. The one-second [root mean square](../../../root-mean-square.md) scatter is about $0.006\ \mathrm V$; the plotted peak-to-peak excursions are larger and must not be substituted for an [root mean square](../../../root-mean-square.md) noise. Independent graphical digitization of the blue trace gives means near $0.331,0.406,0.493$ V and scatters about $0.006$–$0.007$ V, consistent with this estimate. These are readings from a drawing, not exact original data.

The supplied Planck approximation gives $B_C\simeq0.08590$ and $B_H\simeq0.12836$ in $\mathrm{W\,m^{-2}\,sr^{-1}\,(cm^{-1})^{-1}}$. Thus the [noise-equivalent radiance](../../../noise-equivalent-radiance.md) of one one-second sample is

$$
\boxed{\mathrm{NER}\simeq\frac{B_H-B_C}{V_H-V_C}\sigma_V\simeq1.6\times10^{-3}\ \mathrm{W\,m^{-2}\,sr^{-1}\,(cm^{-1})^{-1}}}.
$$

Here the calibrating means are used to determine the response slope; their own uncertainty is included explicitly in the final scene estimate below.

**Optical throughput and detectivity.** A paraxial $f/F$ cone has half-angle approximately $1/(2F)$ and projected [solid angle](../../../solid-angle.md) approximately $\pi/(4F^2)$. With $F=2$ and $A_d=10^{-6}\ \mathrm{m^2}$,

$$
\boxed{A_d\Omega\simeq\frac{\pi A_d}{16}=1.96\times10^{-7}\ \mathrm{m^2\,sr}\simeq1.9\times10^{-7}\ \mathrm{m^2\,sr}}.
$$

Using the exact cone angle $\tan\theta=1/(2F)$ gives projected etendue $A_d\pi\sin^2\theta=1.85\times10^{-7}\ \mathrm{m^2\,sr}$, within the intended approximation. The [radiance](../../../radiance.md) noise corresponds to detector power noise

$$
\sigma_P\simeq\eta\,A_d\Omega\,\Delta\widetilde\nu\,\mathrm{NER}
\simeq0.6(1.9\times10^{-7})(1)(1.6\times10^{-3})\simeq1.8\times10^{-10}\ \mathrm W.
$$

The [wavenumber](../../../wavenumber.md) bandwidth is $1\ \mathrm{cm^{-1}}$ and must match the [radiance](../../../radiance.md)'s per-wavenumber unit; it is not an electrical noise bandwidth. For the common order-of-magnitude assignment $\Delta f\sim1\ \mathrm{Hz}$ to a one-second sample,

$$
\boxed{\mathrm{NEP}\sim1.8\times10^{-10}\ \mathrm{W\,Hz^{-1/2}},\qquad D_*\sim5.6\times10^8\ \mathrm{Jones}}.
$$

Area in the last expression is $1\ \mathrm{mm^2}=0.01\ \mathrm{cm^2}$. For a specified one-second boxcar with [white noise](../../../white-noise.md), the one-sided equivalent noise bandwidth is instead $1/(2t)=0.5\ \mathrm{Hz}$. That convention gives spectral NEP $\simeq2.5\times10^{-10}\ \mathrm{W\,Hz^{-1/2}}$ and $D_*\simeq3.9\times10^8$ Jones. The source does not specify the electrical filter, so the two conventions should not be mixed or assigned spurious precision.

**Two-point retrieval and its uncertainty.** Assume linear, stable response for the three views. The [radiometer two-point calibration](../../../radiometer-two-point-calibration.md) is

$$
B_S=B_C+(B_H-B_C)\frac{V_S-V_C}{V_H-V_C}.
$$

With target [radiances](../../../radiance.md) treated as known, differentiating gives

$$
\boxed{\delta B_S=a\,\delta V_S+b\,\delta V_H-(a+b)\,\delta V_C},\qquad
\boxed{a=\frac{B_H-B_C}{V_H-V_C},\quad b=-\frac{(B_H-B_C)(V_S-V_C)}{(V_H-V_C)^2}}.
$$

Notice $b<0$ for an intermediate scene: raising the hot voltage while keeping the scene voltage fixed reduces the inferred scene [radiance](../../../radiance.md). Numerically $a\simeq0.2621$, $b\simeq-0.1214$ in [radiance](../../../radiance.md) units per volt.

The scene interpolation fraction is about $0.463$, giving $B_S\simeq0.1056$ and

$$
\boxed{T_{b,S}=\frac{1200}{\ln(1+6.88/B_S)}\simeq286.2\ \mathrm K}.
$$

For independent [white noise](../../../white-noise.md) in each view, each hundred-sample mean has [standard error](../../../standard-error.md) $\sigma_{\bar V}=0.006/10=0.0006\ \mathrm V$. The [radiance](../../../radiance.md) error is

$$
\sigma_{B_S}=\sigma_{\bar V}\sqrt{a^2+b^2+(a+b)^2}\simeq1.93\times10^{-4}\ \mathrm{W\,m^{-2}\,sr^{-1}\,(cm^{-1})^{-1}}.
$$

Using the given temperature sensitivity,

$$
\boxed{\sigma_{T_b}\simeq630\sigma_{B_S}\simeq0.12\ \mathrm K}.
$$

A scatter estimate closer to $0.007$ V changes this to roughly $0.14$ K. These are random [standard errors](../../../standard-error.md) under the averaging assumptions. Target-temperature/emissivity uncertainty, response drift and atmospheric or surface-emissivity corrections are separate: the retrieved quantity is a [brightness temperature](../../../brightness-temperature.md), not automatically the true sea-surface temperature.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2016](../../2016-split.md)
3. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../split.md)
4. [Physics of atmospheres and oceans course of the University of Oxford](../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
5. [Year 4 of the physics course of the University of Oxford](../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
