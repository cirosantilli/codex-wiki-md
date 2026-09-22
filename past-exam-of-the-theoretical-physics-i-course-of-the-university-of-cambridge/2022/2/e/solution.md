<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [dispersion relation](../../../../dispersion-relation-split.md) shows that an infinite rod has unstable long-wave modes. A finite rod excludes sufficiently long wavelengths, so stability depends on its length and the precise end conditions. The fourth spatial [derivative](../../../../derivative.md) requires two conditions at each end; fixing transverse positions alone does not specify whether slopes are constrained.

First take displacement-fixed ends with free rotation. Setting $\phi(0)=\phi(l)=0$ leaves slope variations free; the bending boundary term in the [first variation](../../../../first-variation.md) then gives the corresponding [natural boundary conditions on the slope](../../../../natural-boundary-condition-on-the-slope.md), $\phi_{xx}(0)=\phi_{xx}(l)=0$. The spatial [normal modes](../../../../normal-mode.md) are $\sin(n\pi x/l)$, and

$$
\boxed{\omega_n^2=\frac\beta\rho\left(\frac{n\pi}{l}\right)^4-\frac\alpha\rho\left(\frac{n\pi}{l}\right)^2.}
$$

The first mode destabilizes first. Consequently

$$
\boxed{l<\pi\sqrt{\frac\beta\alpha}:\ \text{stable oscillatory modes};\qquad l>\pi\sqrt{\frac\beta\alpha}:\ \text{unstable straight rod}.}
$$

At equality, the first mode has zero restoring force and is marginal, with a static component and a possible linear-in-time component in the linear theory. Every integer $n<l\sqrt{\alpha/\beta}/\pi$ gives an exponentially growing mode.

If "fixed" instead means clamped, the [clamped boundary condition](../../../../clamped-boundary-condition.md) is $\phi=\phi_x=0$ at both ends. The critical compression is then

$$
\boxed{\alpha_c=\frac{4\pi^2\beta}{l^2},\qquad l_c=2\pi\sqrt{\frac\beta\alpha}.}
$$

For example, the static critical shape $1-\cos(2\pi x/l)$ obeys the four clamp conditions and the zero-frequency equation at this load. To establish that it is the first threshold, write $v=\phi_x$: it has zero endpoints and zero mean, and periodic extension gives $\int_0^lv_x^2dx\geq(2\pi/l)^2\int_0^lv^2dx$ by the zero-mean periodic [Poincaré inequality](../../../../poincare-inequality.md), with equality at $v\propto\sin(2\pi x/l)$. This proves the critical [Rayleigh quotient](../../../../rayleigh-quotient.md). Both cases are instances of the [compressed Euler-Bernoulli beam and its endpoint-dependent buckling threshold](../../../../compressed-euler-bernoulli-beam-and-its-endpoint-dependent-buckling-threshold.md). The source does not specify the endpoint rotation, so both interpretations are stated explicitly.

## ↑ Ancestors (14)

1. [E](../e.md)
2. [2](../../2.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the theoretical physics I course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics I course of the University of Cambridge](../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
