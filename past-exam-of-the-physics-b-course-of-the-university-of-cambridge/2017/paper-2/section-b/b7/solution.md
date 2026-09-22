<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

**Distributed circuit model.** A [transmission line](../../../../../transmission-line.md) must be treated as a distributed system when its propagation [time](../../../../../time-in-physics.md) is appreciable compared with the [signal](../../../../../signal.md) timescale. Divide a uniform two-conductor line into elements of [length](../../../../../length.md) $dx$. Each has series resistance $R'dx$ and [inductance](../../../../../inductance.md) $L'dx$, and shunt [electrical conductance](../../../../../electrical-conductance.md) $G'dx$ and [capacitance](../../../../../capacitance.md) $C'dx$. The primes denote quantities per unit [length](../../../../../length.md), with units $\mathrm{\Omega\,m^{-1}}$, $\mathrm{H\,m^{-1}}$, $\mathrm{S\,m^{-1}}$ and $\mathrm{F\,m^{-1}}$, respectively.

Kirchhoff's [voltage](../../../../../voltage.md) and current laws give the [Telegrapher's equations](../../../../../telegrapher-s-equations.md):

$$
\boxed{\frac{\partial V}{\partial x}=-R'I-L'\frac{\partial I}{\partial t},
\qquad \frac{\partial I}{\partial x}=-G'V-C'\frac{\partial V}{\partial t}.}
$$

For a lossless line, $R'=G'=0$, differentiation gives $V_{xx}=L'C'V_{tt}$ and the same [wave equation](../../../../../wave-equation-split.md) for $I$. The propagation [speed](../../../../../speed.md) and [characteristic impedance](../../../../../characteristic-impedance.md) are

$$
\boxed{u=\frac1{\sqrt{L'C'}},\qquad Z_0=\sqrt{\frac{L'}{C'}}.}
$$

A general lossless [signal](../../../../../signal.md) has $V=V^+(t-x/u)+V^-(t+x/u)$ and $I=[V^+(t-x/u)-V^-(t+x/u)]/Z_0$. Thus [characteristic impedance](../../../../../characteristic-impedance.md) is the [voltage](../../../../../voltage.md)/current ratio of one travelling wave, not simply the resistance of the wires. It can be real even when the line dissipates no [energy](../../../../../energy-split.md), because [energy](../../../../../energy-split.md) is carried away by propagation.

For sinusoidal quantities with convention $e^{i\omega t}$, the general lossy-line formulas are

$$
\gamma_{\rm prop}=\sqrt{(R'+i\omega L')(G'+i\omega C')},
\qquad Z_0=\sqrt{\frac{R'+i\omega L'}{G'+i\omega C'}}.
$$

Choose the square-root branches for forward attenuation and positive forward [power](../../../../../power.md). The [real part](../../../../../real-part.md) of $\gamma_{\rm prop}$ is attenuation per unit [length](../../../../../length.md); its [imaginary part](../../../../../imaginary-part.md) is the phase [wavenumber](../../../../../wavenumber.md). For small losses, attenuation is approximately $R'/(2Z_0)+G'Z_0/2$, using the lossless real $Z_0$ in this estimate.

**Fields and geometry.** Two separated conductors support a [transverse electromagnetic mode](../../../../../transverse-electromagnetic-mode.md), with electric and [magnetic fields](../../../../../magnetic-field-split.md) transverse to the propagation axis. For a homogeneous [dielectric](../../../../../dielectric.md) and negligible conductor penetration, both examples below have $L'C'=\mu\epsilon$ and hence $u=1/\sqrt{\mu\epsilon}$. The distributed circuit model follows from the field [energy](../../../../../energy-split.md) and charges in each slice.

For a [coaxial cable](../../../../../coaxial-cable.md) with inner radius $a$ and inner surface of the outer conductor at $b$, [Gauss's law](../../../../../gauss-s-law.md) and [Ampère's law](../../../../../ampere-s-circuital-law.md) give

$$
E_\rho=\frac{V}{\rho\ln(b/a)},\qquad H_\phi=\frac{I}{2\pi\rho},\quad a<\rho<b.
$$

The [electric field](../../../../../electric-field-split.md) is radial and the [magnetic field](../../../../../magnetic-field-split.md) circles the axis. Integration of [voltage](../../../../../voltage.md) and field [energy](../../../../../energy-split.md) gives

$$
C'=\frac{2\pi\epsilon}{\ln(b/a)},\qquad
L'=\frac{\mu}{2\pi}\ln(b/a),\qquad
\boxed{Z_0=\frac1{2\pi}\sqrt{\frac\mu\epsilon}\ln\frac ba.}
$$

The equal and opposite return current on the outer conductor confines the ideal external field to the annulus.

For wide parallel plates of width $w$ separated by $d\ll w$, neglect fringing. The [electric field](../../../../../electric-field-split.md) crosses the gap, $E\simeq V/d$, while the [magnetic field](../../../../../magnetic-field-split.md) lies in the gap parallel to the plates and perpendicular to propagation, $H\simeq I/w$. Therefore

$$
C'=\frac{\epsilon w}{d},\qquad L'=\frac{\mu d}{w},\qquad
\boxed{Z_0=\frac d w\sqrt{\frac\mu\epsilon}.}
$$

For a forward wave, $\mathbf E\times\mathbf H$ points along the line. Integrating this [Poynting vector](../../../../../poynting-vector.md) over either cross-section gives instantaneous [power](../../../../../power.md) $VI$. For complex peak amplitudes, average [power](../../../../../power.md) is $\operatorname{Re}(VI^*)/2$, or $|V^+|^2/(2Z_0)$ for a single forward wave on a lossless line. The conductors guide an [energy flux](../../../../../energy-flux.md) predominantly in the [dielectric](../../../../../dielectric.md) between them.

<a id="section-b/b7/image-electric-and-magnetic-fields-in-coaxial-and-parallel-plate-transmission-lines"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2-2017-line-fields.png)

**[Figure 2](#section-b/b7/image-electric-and-magnetic-fields-in-coaxial-and-parallel-plate-transmission-lines). Electric and magnetic fields in coaxial and parallel-plate transmission lines**. Original transverse cross-sections for a forward TEM wave. Blue arrows show the electric field and orange arrows the magnetic field strength. Dots denote current out of the page and crosses current into it. Parallel-plate edge fields and coaxial conductor penetration are neglected.

**Terminations and reflection.** At a load $Z_L$, require $V_L=Z_LI_L$. If $V^+$ and $V^-$ are the incident and reflected [voltage](../../../../../voltage.md) amplitudes there, the total current is $(V^+-V^-)/Z_0$. Thus

$$
\boxed{\Gamma_V=\frac{V^-}{V^+}=\frac{Z_L-Z_0}{Z_L+Z_0},\qquad \Gamma_I=-\Gamma_V.}
$$

A matched load, $Z_L=Z_0$, absorbs the incident [power](../../../../../power.md) with no reflection. An [open circuit](../../../../../open-circuit.md) has $\Gamma_V=+1$, a current node and a doubled [voltage](../../../../../voltage.md) at the end. A [short circuit](../../../../../short-circuit.md) has $\Gamma_V=-1$, a [voltage](../../../../../voltage.md) node and a doubled current there. A purely reactive load on a lossless line has $|\Gamma_V|=1$ and accepts no average [power](../../../../../power.md). For real $Z_0$, the reflected [power](../../../../../power.md) fraction is $|\Gamma_V|^2$ and the accepted fraction is $1-|\Gamma_V|^2$.

Incident and reflected waves produce a standing-wave pattern with [voltage](../../../../../voltage.md) [standing wave ratio](../../../../../standing-wave-ratio.md) $(1+|\Gamma_V|)/(1-|\Gamma_V|)$. The [input impedance](../../../../../input-impedance.md) of a lossless [length](../../../../../length.md) $\ell$ is

$$
Z_{\rm in}=Z_0\frac{Z_L+iZ_0\tan(k\ell)}{Z_0+iZ_L\tan(k\ell)}.
$$

This gives $iZ_0\tan(k\ell)$ for a short and $-iZ_0\cot(k\ell)$ for an open. A quarter-wave section gives $Z_{\rm in}=Z_0^2/Z_L$, enabling impedance transformation. After a source launches a pulse, a distant termination affects it only after the reflected pulse returns; the return [time](../../../../../time-in-physics.md) is $2\ell/u$. Real conductor resistance, [dielectric loss](../../../../../dielectric-loss.md) and departures from a TEM field profile limit the ideal model at high [frequency](../../../../../frequency.md).

## ↑ Ancestors (14)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2017](../../../split.md)
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
