<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let the two returning monochromatic fields at the chosen detector port be

$$
E_1=a\cos(\omega t),\qquad E_2=a\cos(\omega t+\varphi),\qquad
\varphi=2\pi\nu\Delta d.
$$

Here $\nu$ is [wavenumber](../../../../wavenumber.md), rather than temporal [frequency](../../../../frequency.md). An optical-cycle average uses $\langle\cos^2\omega t\rangle=1/2$ and $\langle\cos\omega t\cos(\omega t+\varphi)\rangle=\cos\varphi/2$. In units absorbing the detector's field-to-power conversion,

$$
\boxed{P=\langle(E_1+E_2)^2\rangle=a^2[1+\cos(2\pi\nu\Delta d)].}
$$

The choice of output port can reverse the cosine sign. For mutually incoherent components of the [radiation spectrum](../../../../radiation-spectrum.md), add powers rather than instantaneous fields, giving

$$
P(\Delta d)=\int_0^\infty Q(\nu)[1+\cos(2\pi\nu\Delta d)]\,d\nu.
$$

Subtracting the constant term leaves the [Fourier cosine transform](../../../../fourier-cosine-transform.md) of the detected spectral weighting $Q(\nu)$, including throughput and detector response.

The printed prefactor requires a normalization convention. In the derivation, $a$ is the amplitude of each returning field at the detector, not an entrance amplitude with input power $a^2$. For a lossless balanced [beam splitter](../../../../beam-splitter.md) and literal input power $P_{\rm in}$, [conservation of energy](../../../../conservation-of-energy.md) instead gives $P_{\rm out}=P_{\rm in}[1+\cos\varphi]/2$, so the source formula identifies $a^2=P_{\rm in}/2$. Taking both $P_{\rm in}=a^2$ and the printed formula literally would give $P_{\rm out}=2P_{\rm in}$ at zero [optical path difference](../../../../optical-path-difference.md), a concrete normalization contradiction.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
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
