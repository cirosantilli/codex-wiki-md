<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**[antenna](../../../../antenna-radio.md) quantities.** [radiation resistance](../../../../radiation-resistance.md) represents emitted [power](../../../../power.md) by $P_{\rm rad}=I_{\rm rms}^2R_{\rm rad}$ at the feed. It is not [Joule heating](../../../../joule-heating.md) in the [antenna](../../../../antenna-radio.md); a separate loss resistance accounts for that. [antenna gain](../../../../antenna-gain.md) is the directional far-field intensity relative to an isotropic radiator supplied with the same input [power](../../../../power.md):

$$
G(\theta,\phi)=\frac{4\pi r^2S_r(\theta,\phi)}{P_{\rm in}}.
$$

It includes [radiation efficiency](../../../../radiation-efficiency.md) and equals [antenna directivity](../../../../antenna-directivity.md) only for a lossless [antenna](../../../../antenna-radio.md). [antenna effective area](../../../../antenna-effective-area.md) is defined by the [power](../../../../power.md) available to a matched load, $P_{\rm av}=A_{\rm eff}S_{\rm inc}$, for incidence from a specified direction and matched polarization. It need not equal a literal geometric collecting area.

**Gain–area relation.** To derive the [antenna gain-effective-area relation](../../../../antenna-gain-effective-area-relation.md), take a passive reciprocal [antenna](../../../../antenna-radio.md). Its [electromagnetic reciprocity](../../../../reciprocity-electromagnetism.md) makes the receive pattern proportional to the transmit pattern; write $A_{\rm eff}(\Omega)=K G(\Omega)$. The normalization follows from [thermal equilibrium](../../../../thermal-equilibrium-split.md). In the [Rayleigh-Jeans law](../../../../rayleigh-jeans-law.md) limit, [blackbody radiation](../../../../black-body-radiation.md) radiance per unit [frequency](../../../../frequency.md) per unit [solid angle](../../../../solid-angle.md) is $2k_BT/\lambda^2$ for two polarizations. A single [antenna](../../../../antenna-radio.md) polarization couples to one half, so the available incident noise [power](../../../../power.md) is

$$
dP_{\rm inc}=\frac{k_BT}{\lambda^2}\int A_{\rm eff}(\Omega)\,d\Omega\,d\nu.
$$

The open-circuit Johnson voltage spectrum of the [antenna](../../../../antenna-radio.md) resistance is $4k_BTR_{\rm rad}\,d\nu$. A [matched load](../../../../matched-load.md) receives half the open-circuit voltage, giving available [power](../../../../power.md) $k_BT\,d\nu$. In a lossless [antenna](../../../../antenna-radio.md) at [thermal equilibrium](../../../../thermal-equilibrium-split.md) these [powers](../../../../power.md) agree; hence $\int A_{\rm eff}\,d\Omega=\lambda^2$. Since $\int G\,d\Omega=4\pi$,

$$
\boxed{A_{\rm eff}(\theta,\phi)=\frac{\lambda^2}{4\pi}G(\theta,\phi)}.
$$

The same efficiency factor multiplies receiving area and gain if reciprocal dissipative losses are included consistently. Impedance mismatch or polarization mismatch reduces delivered [power](../../../../power.md) further. The factor of two for thermal polarization modes and the factor of four between open-circuit voltage variance and matched-load [power](../../../../power.md) are separate effects.

**Normalize the [radar](../../../../radar.md) beam.** Interpret the azimuth as signed about the beam centre at $\phi=0$, so both sides of the narrow lobe are included. Put $u=\theta-\pi/2$. To leading order in the small angular width, $\sin\theta\simeq1$ and the angular integrals can be extended over the real line:

$$
P=\int N\,d\Omega\simeq C\int e^{-u^2/(2\alpha^2)}du
\int e^{-\phi^2/(2\alpha^2)}d\phi=2\pi\alpha^2C.
$$

The [Gaussian antenna beam solid angle](../../../../gaussian-antenna-beam-solid-angle.md) gives the peak on the positive $x$-axis consequently has

$$
C\simeq\frac{P}{2\pi\alpha^2},\qquad
G_0\simeq\frac2{\alpha^2},\qquad
A_0\simeq\frac{\lambda^2}{2\pi\alpha^2},\qquad \lambda=\frac c\nu.
$$

Here $N$ is [power](../../../../power.md) per [solid angle](../../../../solid-angle.md), equal to $r^2S_r$ in the far field. The leading neglected solid-angle correction is relative order $\alpha^2$.

**Return using the supplied electric-dipole response.** The [electric-dipole radar cross section of a small conducting sphere](../../../../electric-dipole-radar-cross-section-of-a-small-conducting-sphere.md) determines this return. At target range $D$, the incident intensity is $S_t=C/D^2$. Write its [root mean square](../../../../root-mean-square.md) [electric field](../../../../electric-field-split.md) as $E_t$, with $S_t=\epsilon_0cE_t^2$. The induced [electric dipole](../../../../electric-dipole.md) is $p_{\rm rms}=4\pi\epsilon_0a^3E_t$. A dipole's angular radiation pattern, normalized by $\int\sin^2\chi\,d\Omega=8\pi/3$, gives $dP_{\rm sc}/d\Omega=(3P_{\rm sc}/8\pi)\sin^2\chi$. The backward direction is perpendicular to the induced dipole, so the supplied total dipole [power](../../../../power.md) gives

$$
\left.\frac{dP_{\rm sc}}{d\Omega}\right|_{\rm back}
=\frac{3}{8\pi}\frac{8\pi^3\nu^4p_{\rm rms}^2}{3\epsilon_0c^3}
=k^4a^6S_t,\qquad k=\frac{2\pi\nu}{c}.
$$

The received intensity is this angular [power](../../../../power.md) divided by $D^2$. Using the [monostatic radar equation](../../../../monostatic-radar-equation.md), or directly multiplying by the receive area, gives

$$
P_R=\frac{A_0}{D^2}k^4a^6\frac{C}{D^2}
=\frac{4\pi^2Pa^6}{\lambda^2\alpha^4D^4}.
$$

The receiver threshold is a voltage across the [matched load](../../../../matched-load.md), so the detectable [power](../../../../power.md) is $V_m^2/R$, without another matching factor:

$$
\boxed{D_{\rm electric}=
\left(\frac{4\pi^2PR\nu^2a^6}{c^2\alpha^4V_m^2}\right)^{1/4}}.
$$

This is the electric-dipole result following from the response data provided. It assumes $ka\ll1$, far-field propagation on each leg, alignment at the beam maximum and no attenuation or additional receiver losses.

**Perfect-conductor qualification.** [perfect-conductor sphere dipole interference](../../../../perfect-conductor-sphere-dipole-interference.md) arises because the sphere also excludes the oscillating [magnetic field](../../../../magnetic-field-split.md). Solving the magnetic boundary problem gives $\mathbf m=-2\pi a^3\mathbf H_t$ in addition to the [electric dipole](../../../../electric-dipole.md). The [magnetic polarizability of a perfectly conducting sphere](../../../../magnetic-polarizability-of-a-perfectly-conducting-sphere.md) follows from its induced surface currents.[section 8.4, Example 8.4.3: magnetic dipole induced in a perfectly conducting sphere](../../../../electromagnetic-fields-and-energy-by-hermann-a-haus-and-james-r-melcher.md) In the backward direction the magnetic contribution has half the electric scattering [amplitude](../../../../wave-amplitude.md) and the same sign, so the returned intensity is $9/4$ of the electric-only value. Equivalently, the monostatic [radar cross section](../../../../radar-cross-section.md) is $\sigma_{\rm back}=9\pi k^4a^6$, rather than $4\pi k^4a^6$. Including both leading dipoles therefore gives

$$
\boxed{D_{\rm PEC}=
\left(\frac{9\pi^2PR\nu^2a^6}{c^2\alpha^4V_m^2}\right)^{1/4}
=\sqrt{\frac32}\,D_{\rm electric}}.
$$

Both results have been distinguished because the supplied auxiliary data describe only the [electric dipole](../../../../electric-dipole.md), while the literal perfect-conductor boundary conditions also generate the magnetic one. The backward interference is a leading-order effect, not a higher-order correction in $ka$.[section Scattering by a Small Perfectly Conducting Sphere: electric and magnetic dipoles and backward interference](../../../../scattering-of-em-waves-by-michael-fowler.md)

<a id="3/image-original-electric-only-and-electric-plus-magnetic-small-sphere-scattering-comparison"></a>
![](../../../../past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2015/paper-1-radar-scattering.png)

**[Figure 2](#3/image-original-electric-only-and-electric-plus-magnetic-small-sphere-scattering-comparison). Original electric-only and electric-plus-magnetic small-sphere scattering comparison**.

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2015](../../split.md)
4. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../split.md)
5. [Optics and Electrodynamics course of the University of Cambridge](../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
