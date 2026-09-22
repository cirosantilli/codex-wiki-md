<h1 id="k/k4/solution">Solution</h1>

↑ **Parent:** [K4](../k4.md)

The [conformal map](../../../../conformal-map.md) $\zeta=z^3$ sends the wedge $0<\arg z<\pi/3$ to the upper half-plane. The physical [vortex](../../../../phase-vortex.md) maps to $\zeta=c^3$; an opposite image [vortex](../../../../phase-vortex.md) at $\overline c^{,3}$ makes the real axis a streamline. Pulling this potential back gives

$$
w(z)=-\frac{i\Gamma}{2\pi}\log(z^3-c^3)
+\frac{i\Gamma}{2\pi}\log(z^3-\overline c^{,3}).
$$

Since $z^3-c^3=(z-c)(z^2+cz+c^2)$, splitting the first logarithm, up to an additive constant, gives exactly the required form. The image construction enforces zero normal velocity on both rays.

To find the [vortex](../../../../phase-vortex.md) motion, hold $c$ fixed while differentiating with respect to $z$, remove the self-induced singular term $-i\Gamma/(2\pi(z-c))$, and then evaluate at $z=c$. The remaining [complex velocity](../../../../complex-velocity.md) is

$$
\frac{i\Gamma}{2\pi}\left[-\frac{2c+c}{c^2+c^2+c^2}
+\frac{3c^2}{c^3-\overline c^{,3}}\right].
$$

A [complex velocity](../../../../complex-velocity.md) $u-iv$ equals $d\overline c/dt$, rather than $dc/dt$. Thus

$$
\boxed{\frac{d\overline c}{dt}=\frac{i\Gamma}{2\pi}
\left(-\frac1c+\frac{3c^2}{c^3-\overline c^{,3}}\right).}
$$

The overbar on the source derivative is essential to the trajectory calculation.

Write $c=re^{i\theta}$. Since $c^3-\overline c^{,3}=2ir^3\sin(3\theta)$, multiply the equation by $e^{i\theta}$ to obtain

$$
\dot r-ir\dot\theta
=\frac{3\Gamma}{4\pi r}\cot(3\theta)+\frac{i\Gamma}{4\pi r}.
$$

Taking real and imaginary parts gives

$$
\dot r=\frac{3\Gamma}{4\pi r}\cot(3\theta),\qquad
\dot\theta=-\frac{\Gamma}{4\pi r^2}.
$$

Therefore

$$
\frac d{dt}\big(r\sin(3\theta)\big)
=\dot r\sin(3\theta)+3r\cos(3\theta)\dot\theta=0,
$$

proving the trajectory invariant

$$
\boxed{r\sin(3\theta)=\text{constant}.}
$$

The calculation also covers $\Gamma=0$, when the [vortex](../../../../phase-vortex.md) position is stationary.

This is the sixty-degree case of a [point vortex in a wedge](../../../../point-vortex-in-a-wedge.md).

## ↑ Ancestors (12)

1. [K4](../k4.md)
2. [K](../../k.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
