<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Rotation about the vertical axis gives the inner surface the azimuthal speed $\Omega a\sin\theta$. The leading [Couette flow](../../../../../../couette-flow.md) shear traction is opposing and has magnitude

$$
\frac{\mu\Omega a\sin\theta}{h(\theta)}.
$$

Its moment arm about the vertical axis is $a\sin\theta$, and $dS=2\pi a^2\sin\theta\,d\theta$. Consequently

$$
G_z=-\frac{2\pi\mu\Omega a^4}{\Delta}
\int_0^\pi\frac{\sin^3\theta}{1-\lambda\cos\theta}\,d\theta.
$$

Putting $t=\lambda\cos\theta$ and using the supplied integral gives

$$
\boxed{
G_z=-\frac{2\pi\mu\Omega a^4}{\lambda^3\Delta}
\left[
2\lambda+(1-\lambda^2)
\log\left(\frac{1-\lambda}{1+\lambda}\right)
\right]}.
$$

This [viscous shear torque](../../../../../../viscous-shear-torque.md) opposes the rotation. Its concentric limit is $-8\pi\mu\Omega a^4/(3\Delta)$, agreeing with the thin-gap limit of [Torque in rotational Stokes flow between concentric spheres](../../../../../../torque-in-rotational-stokes-flow-between-concentric-spheres.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
