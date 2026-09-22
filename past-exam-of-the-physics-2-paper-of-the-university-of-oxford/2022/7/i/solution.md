<h1 id="7/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take coordinate $y$ across the slit and observation angle $\theta$ from its [normal vector](../../../../normal-vector.md). Under [Fraunhofer diffraction](../../../../fraunhofer-diffraction.md), the relative [optical path difference](../../../../optical-path-difference.md) from $y$ is $y\sin\theta$. Uniform coherent illumination makes the [complex amplitude](../../../../complex-amplitude.md) proportional to the aperture [integral](../../../../integral-split.md):

$$
\mathcal E(\theta)=K\int_{-w/2}^{w/2}e^{-iky\sin\theta}\,dy
=Kw\frac{\sin\beta}{\beta},\qquad
\beta=\frac{\pi w\sin\theta}{\lambda},\quad k=\frac{2\pi}{\lambda}.
$$

The [light intensity](../../../../light-intensity.md) is proportional to $|\mathcal E|^2$, so

$$
\boxed{I(\theta)=I(0)\left[\frac{\sin(\pi w\sin\theta/\lambda)}{\pi w\sin\theta/\lambda}\right]^2.}
$$

The central value is the continuous limit of the [sinc function](../../../../sinc-function.md). The first minima satisfy $\sin\theta=\pm\lambda/w$, if $\lambda\leq w$. Infinite slit height removes spreading in the other transverse direction; this expression describes the slit-width direction.

Strictly, distance $D\gg w$ alone does not ensure [Fraunhofer diffraction](../../../../fraunhofer-diffraction.md): one also needs $w^2/(\lambda D)\ll1$, so that quadratic aperture-dependent [wave phase](../../../../phase-waves.md) is negligible, or observation in a suitable [focal plane](../../../../focal-plane.md). For example, $w=1\,\mathrm{mm}$, $\lambda=500\,\mathrm{nm}$ and $D=1\,\mathrm m$ have $D/w=1000$ but $w^2/(\lambda D)=2$; the [Fresnel diffraction](../../../../fresnel-diffraction.md) correction is then substantial. The displayed result uses the intended far-field regime of the question and the usual scalar aperture approximation.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [7](../../7.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
