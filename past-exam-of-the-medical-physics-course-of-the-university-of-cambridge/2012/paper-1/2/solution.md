<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

TODO: Biology deferred at the user's request: clinical contrast interpretation, applications, and the head-injury MRI-versus-CT comparison.

The generic physics of [magnetic resonance imaging](../../../../magnetic-resonance-imaging.md) combines a main static magnet, radiofrequency transmit and receive coils, controlled [magnetic field gradients](../../../../magnetic-field-gradient.md), signal electronics and reconstruction. A transverse radiofrequency pulse excites [nuclear spins](../../../../nuclear-spin.md) near their Larmor [frequency](../../../../frequency.md), $\omega_0=\gamma B_0$. The evolving transverse magnetization induces a received signal; [phase](../../../../phase-waves.md) coherence and relaxation determine its time dependence.

Gradients encode [position](../../../../position.md) into [phase](../../../../phase-waves.md). In a simplified homogeneous receive-sensitivity model,

$$
s(t)=\int\rho(\mathbf r)e^{-2\pi i\mathbf k(t)\cdot\mathbf r}\,d^3\mathbf r,
\qquad \mathbf k(t)=\frac{\gamma}{2\pi}\int^t\mathbf G(t')\,dt'.
$$

Here $\mathbf k$ is in cycles per unit length and $\gamma$ is in radians per second per tesla. Echo sign changes, pulse sequence timing and receive sensitivity belong in a more complete signal model. Sampling this [MRI k-space](../../../../magnetic-resonance-k-space.md) and reconstructing its data produces an image; the measured samples are not already real-space pixel values.

The physical signal depends on [spin](../../../../spin.md) density, longitudinal recovery and transverse dephasing. Timing changes their weighting. Static field inhomogeneity adds reversible dephasing beyond intrinsic [transverse relaxation](../../../../transverse-relaxation.md), motivating echo techniques and distinguishing $T_2^*$ from $T_2$. Those are physical signal mechanisms; their biological interpretation remains deferred.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2012](../../split.md)
4. [Past exam of the medical physics course of the University of Cambridge](../../../split.md)
5. [Medical Physics course of the University of Cambridge](../../../../medical-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
