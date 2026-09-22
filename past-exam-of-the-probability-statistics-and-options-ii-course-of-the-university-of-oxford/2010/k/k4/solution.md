<h1 id="k/k4/solution">Solution</h1>

↑ **Parent:** [K4](../k4.md)

The [conformal map](../../../../conformal-map.md) $\zeta=z^3$ sends the wedge to the upper half-plane. A [fluid vortex](../../../../vortex-fluid-mechanics.md) at $c^3$ there has an opposite image at $\bar c^3$, so the pulled-back potential is

$$
w(z)=\frac{i\Gamma}{2\pi}\bigl(-\log(z^3-c^3)+\log(z^3-\bar c^3)\bigr).
$$

The two boundary rays map to the real axis, where the imaginary part is constant, giving the required impermeability. Factoring $z^3-c^3=(z-c)(z^2+cz+c^2)$ gives the printed form up to branch constants.

The [fluid vortex](../../../../vortex-fluid-mechanics.md) moves with the regular part of the [complex velocity](../../../../complex-velocity.md), excluding its own singular term. Since $w'=u-iv$, its motion is the conjugated [derivative](../../../../derivative.md). Differentiating the remaining terms and setting $z=c$ gives

$$
\boxed{\frac{d\bar c}{dt}=\frac{i\Gamma}{2\pi}\left(-\frac1c+\frac{3c^2}{c^3-\bar c^3}\right).}
$$

The overbar on the time [derivative](../../../../derivative.md) is essential.

Write $c=re^{i\theta}$. Using $c^3-\bar c^3=2ir^3\sin3\theta$ and multiplying the velocity equation by $e^{i\theta}$ gives

$$
\dot r-ir\dot\theta=\frac{\Gamma}{4\pi r}(3\cot3\theta+i).
$$

Thus $\dot r=3\Gamma\cot3\theta/(4\pi r)$ and $\dot\theta=-\Gamma/(4\pi r^2)$. Direct differentiation now yields

$$
\frac d{dt}(r\sin3\theta)=\dot r\sin3\theta+3r\dot\theta\cos3\theta=0.
$$

Hence $\boxed{r\sin(3\theta)=\text{constant}}$ along the trajectory while it stays inside the wedge.

## ↑ Ancestors (12)

1. [K4](../k4.md)
2. [K](../../k.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
