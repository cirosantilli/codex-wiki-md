<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

[Snell's law](../../../snell-s-law.md) is $n_a\sin\theta_a=n_b\sin\theta_b$, with both [angles](../../../angle.md) measured from the interface [normal vector](../../../normal-vector.md). Let $\psi$ be the [meridional ray](../../../meridional-ray.md)'s angle to the [optical axis](../../../optical-axis.md) inside the core and let $n_0$ be the incident medium's [refractive index](../../../refractive-index.md). At the entrance face,

$$
n_0\sin\theta=n_{\rm inner}\sin\psi.
$$

At the cylindrical wall the [angle of incidence](../../../angle-of-incidence.md) is $i=\pi/2-\psi$. For $n_{\rm inner}>n_{\rm outer}$, the [critical angle for total internal reflection](../../../critical-angle-for-total-internal-reflection.md) satisfies $\sin i_c=n_{\rm outer}/n_{\rm inner}$. At the limiting accepted ray,

$$
\sin\psi_{\max}=\cos i_c=\sqrt{1-\frac{n_{\rm outer}^2}{n_{\rm inner}^2}}.
$$

Consequently the [optical fiber acceptance angle](../../../optical-fiber-acceptance-angle.md) obeys

$$
\boxed{n_0\sin\theta_{\max}=\sqrt{n_{\rm inner}^2-n_{\rm outer}^2}.}
$$

The requested expression follows for incidence from air, $n_0\simeq1$, provided the right-hand side is at most one. Strict [total internal reflection](../../../total-internal-reflection.md) occurs inside this limiting cone. The derivation uses the standard [meridional ray](../../../meridional-ray.md) model; skew launches need additional geometry.

If $\sqrt{n_{\rm inner}^2-n_{\rm outer}^2}>n_0$, every forward entrance angle allowed by this ideal model meets the side-wall condition, and the limiting half-angle is $\pi/2$, rather than an undefined [inverse sine](../../../inverse-sine.md). For example, $n_{\rm inner}=1.6$, $n_{\rm outer}=1.1$, $n_0=1$ gives $\sqrt{1.35}>1$. Thus the unsaturated printed formula is not valid for every possible pair of [refractive indices](../../../refractive-index.md).

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2016](../../2016-split.md)
3. [Past exam of the electromagnetism and optics course of the University of Oxford](../../split.md)
4. [Electromagnetism and optics course of the University of Oxford](../../../electromagnetism-and-optics-course-of-the-university-of-oxford.md)
5. [Year 2 of the physics course of the University of Oxford](../../../year-2-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
