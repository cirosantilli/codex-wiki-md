<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the attenuation coefficient read from the PDF,

$$
\lambda=\frac{\nu k^3}{2N\sin\theta},\qquad A(\xi)=U_0e^{-\lambda\xi},\qquad U=A(\xi)\cos\omega t,
$$

where here $k$ is the beam wave-number magnitude and the angle convention has $\sin\theta>0$ for the chosen forward attenuation coordinate. The omitted denominator in the TeX is essential both physically and dimensionally. Work in the prescribed along-beam kinematic model, with small parcel excursion compared with $\lambda^{-1}$.

The first-order along-beam [fluid displacement](../../../../../../lagrangian-displacement-fluid-mechanics.md), initially zero, is $\delta\xi=A\sin(\omega t)/\omega$. Therefore the leading displacement correction to the along-beam velocity is

$$
\boxed{u_s(\xi,t)=\delta\xi\,\partial_\xi U
=-\frac{\lambda U_0^2}{2\omega}e^{-2\lambda\xi}\sin(2\omega t)
=-\frac{\nu k^3U_0^2}{4N\omega\sin\theta}e^{-\nu k^3\xi/(N\sin\theta)}\sin(2\omega t).}
$$

This [oscillatory drift of an attenuated internal-wave beam](../../../../../../oscillatory-drift-of-an-attenuated-internal-wave-beam.md) is oscillatory, so

$$
\boxed{\int_0^{2\pi/\omega}u_s\,dt=0.}
$$

Indeed the scalar parcel equation $\dot\Xi=U_0e^{-\lambda\Xi}\cos\omega t$ can be integrated exactly:

$$
e^{\lambda\Xi(t)}=e^{\lambda\Xi(0)}+\frac{\lambda U_0}{\omega}\sin\omega t.
$$

For excursions small enough that the right side stays positive, the parcel returns to its initial along-beam coordinate after each period. This demonstrates the zero net drift in this supplied model. It is not a claim that all components of a viscous beam, or a separately generated Eulerian mean flow, vanish; the question specifies the along-beam component only.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
