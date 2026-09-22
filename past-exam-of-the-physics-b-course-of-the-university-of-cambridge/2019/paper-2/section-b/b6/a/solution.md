<h1 id="section-b/b6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In a homogeneous linear medium, write $\mathbf D=\epsilon\mathbf E$ and $\mathbf B=\mu\mathbf H$. Without free charge or current, [Maxwell's equations](../../../../../../maxwell-equations-split.md) become

$$
\nabla\cdot\mathbf E=0,\quad\nabla\cdot\mathbf B=0,\quad
\nabla\times\mathbf E=-\frac{\partial\mathbf B}{\partial t},\quad
\nabla\times\mathbf B=\mu\epsilon\frac{\partial\mathbf E}{\partial t}.
$$

Taking the [curl](../../../../../../curl.md) of [Faraday's law](../../../../../../faraday-s-law-of-induction.md), using $\nabla\times(\nabla\times\mathbf E)=\nabla(\nabla\cdot\mathbf E)-\nabla^2\mathbf E$, gives

$$
\boxed{\nabla^2\mathbf E-\mu\epsilon\,\partial_t^2\mathbf E=0,
\qquad\nabla^2\mathbf B-\mu\epsilon\,\partial_t^2\mathbf B=0.}
$$

Their plane-wave solutions have $\omega^2=k^2/(\mu\epsilon)$ and speed $v=1/\sqrt{\mu\epsilon}$; in vacuum this is $c=1/\sqrt{\mu_0\epsilon_0}$. For a wave $\operatorname{Re}[\mathbf E_0e^{i(\mathbf k\cdot\mathbf r-\omega t)}]$, the [divergence](../../../../../../divergence.md) equations give $\mathbf k\cdot\mathbf E_0=\mathbf k\cdot\mathbf B_0=0$, while [Faraday's law](../../../../../../faraday-s-law-of-induction.md) gives $\mathbf B_0=\mathbf k\times\mathbf E_0/\omega$. Thus the fields and propagation direction form an [orthogonal](../../../../../../orthogonal-vectors.md) triad, with $B_0=E_0/v$.

The two independent transverse electric components allow linear, circular and elliptical [polarization of an electromagnetic wave](../../../../../../polarization-of-an-electromagnetic-wave.md). Their relative amplitudes and phase determine the polarization state. In a lossless nondispersive medium the [energy density](../../../../../../energy-density.md) and [energy](../../../../../../energy-split.md) flux are

$$
u=\frac12\epsilon E^2+\frac{B^2}{2\mu},\qquad
\mathbf S=\mathbf E\times\mathbf H.
$$

A travelling [plane wave](../../../../../../plane-wave.md) has equal electric and [magnetic energy](../../../../../../magnetic-energy.md) contributions and time-averaged intensity $\langle S\rangle=E_0^2/(2Z)$, where $Z=\sqrt{\mu/\epsilon}$ is its [wave impedance](../../../../../../wave-impedance.md) and $E_0$ denotes peak electric-field amplitude. Reflection and refraction follow by imposing the electromagnetic [boundary conditions](../../../../../../boundary-condition.md). Frequency-dependent constitutive response introduces dispersion; conductivity introduces attenuation, so the simple real constant-speed result has a specified domain of validity.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [B6](../../b6.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
