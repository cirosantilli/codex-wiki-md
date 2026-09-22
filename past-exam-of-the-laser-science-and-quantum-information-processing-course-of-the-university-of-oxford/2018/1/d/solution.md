<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A time delay $d$ multiplies the spectral field by $e^{i\omega d}$. The bright-port [transfer function](../../../../transfer-function.md) is therefore

$$
H(\omega)=\frac{1+e^{i\omega d}}2=e^{i\omega d/2}\cos\frac{\omega d}{2},\qquad
|H(\omega)|^2=\cos^2\frac{\omega d}{2}.
$$

The spectral transmission maxima have [angular frequency](../../../../angular-frequency.md) spacing $\Delta\omega=2\pi/|d|$. For a strongly chirped pulse the local frequency-time mapping is $\omega(t)=\omega_0+2bt$. Thus the filter's adjacent transmitted [frequency](../../../../frequency.md) bands emerge at times separated by

$$
\boxed{\Delta t=\frac{\Delta\omega}{d\omega/dt}=\frac{\pi}{b|d|},}
$$

as obtained directly from the temporal fields. The spectral [transfer function](../../../../transfer-function.md) itself is exact; mapping its features directly onto time requires a sufficiently strong chirp and overlapping envelopes.

As $|d|$ approaches the pulse duration, the two envelopes overlap only partly and the small-delay formula fails. For $|d|\gg\tau$, the selected port contains two separate replicas of field [amplitude](../../../../wave-amplitude.md) $E_0/2$, each with one quarter of the input pulse [energy](../../../../energy-split.md). Their combined [energy](../../../../energy-split.md) is half the input; the other output port carries the remainder. There is no temporal overlap or corresponding time-resolved [interference](../../../../interference-wave-propagation.md). A sufficiently resolving spectrometer can still reveal fine spectral fringes, whose spacing decreases as $1/|d|$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
