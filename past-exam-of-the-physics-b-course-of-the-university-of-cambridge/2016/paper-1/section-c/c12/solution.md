<h1 id="section-c/c12/solution">Solution</h1>

↑ **Parent:** [C12](../c12.md)

Take $\zeta$ as signed [distance](../../../../../distance.md) from the [neutral axis](../../../../../neutral-axis.md) within the beam cross-section. Bending into a large radius $R$ changes the [length](../../../../../length.md) of a fibre proportionally to $\zeta/R$, so [linear elasticity](../../../../../linear-elasticity.md) gives $\sigma=E\zeta/R$, up to the [curvature](../../../../../curvature.md) sign convention. The moment magnitude is

$$
B=\int_A\sigma\zeta\,dA=\frac ER\int_A\zeta^2\,dA=\boxed{\frac{EI}{R}},\qquad I=\int_A\zeta^2\,dA.
$$

Here $I$ is the [second moment of area](../../../../../second-moment-of-area.md) about the [neutral axis](../../../../../neutral-axis.md), with units of [length](../../../../../length.md) to the fourth [power](../../../../../power.md), not the [mass](../../../../../mass.md) [moment of inertia](../../../../../moment-of-inertia.md). A homogeneous cross-section has its [neutral axis](../../../../../neutral-axis.md) through the [centroid](../../../../../centroid.md) under pure bending.

For the straight pin-ended beam, the compressive dead load produces [bending moment](../../../../../bending-moment.md) $-Fy$ at transverse offset $y$. In the small-slope approximation, [curvature](../../../../../curvature.md) is $y''$ with the corresponding sign convention, giving

$$
\boxed{EIy''+Fy=0,\qquad y(0)=y(L)=0.}
$$

The stated endpoints fix positions rather than slopes: this interpretation is consistent with the illustrated end [forces](../../../../../force-split.md) and the later sinusoidal unstressed shape. Truly clamped endpoints would have a different threshold. A nonzero solution $y=A_n\sin(n\pi x/L)$ requires $F_n=n^2\pi^2EI/L^2$. Thus the first Euler load is **$F_c=\pi^2EI/L^2$**. Below it the perfect straight state is stable, at it the first mode is marginal in linear theory, and above it the straight state is unstable. The linear equation selects thresholds but cannot set the [amplitude](../../../../../wave-amplitude.md) or describe a finite postbuckled equilibrium.

For the [initially curved compressed beam](../../../../../initially-curved-compressed-beam.md), elastic [stress](../../../../../stress.md) responds to the change from its stress-free [curvature](../../../../../curvature.md). With $y=y_0+\eta$, the moment is $EI(y''-y_0'')=EI\eta''$, so [force](../../../../../force-split.md) balance gives

$$
\boxed{EI\eta''=-F(y_0+\eta),\qquad \eta(0)=\eta(L)=0.}
$$

Put $q=\pi/L$ and seek the branch continuously connected to the unloaded shape. Since $y_0=Y\sin qx$, substitute $\eta=C\sin qx$ to obtain $-EIq^2C=-F(Y+C)$, or

$$
\boxed{\eta(x)=\frac{F}{F_c-F}Y\sin\frac{\pi x}{L},\qquad y(x)=\frac{F_c}{F_c-F}Y\sin\frac{\pi x}{L}.}
$$

Away from [eigenvalues](../../../../../eigenvalue.md), the homogeneous solution $A\sin(\sqrt{F/(EI)}x)+B\cos(\sqrt{F/(EI)}x)$ vanishes under the two end conditions, so this particular solution is the unique linear equilibrium. For $0\le F<F_c$ and $Y>0$, the maximum additional displacement is $\eta_{\max}=YF/(F_c-F)$ and maximum total displacement is $y_{\max}=Y/(1-F/F_c)$, both at midspan.

<a id="section-c/c12/image-original-small-deflection-amplification-curves-for-a-sinusoidally-imperfect-pin-ended-beam"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-1-imperfect-beam.png)

**[Figure 5](#section-c/c12/image-original-small-deflection-amplification-curves-for-a-sinusoidally-imperfect-pin-ended-beam). Original small-deflection amplification curves for a sinusoidally imperfect pin-ended beam**.

This [sinusoidal imperfection amplification of a column](../../../../../sinusoidal-imperfection-amplification-of-a-column.md) produces deflection at every positive load and strong amplification near $F_c$. The apparent divergence signals loss of the small-slope model before infinite displacement; nonlinear geometry is needed there. The formal continuation above the first threshold is not a stable physical loading branch. Both total and additional displacement are distinguished in the graph.

## ↑ Ancestors (14)

1. [C12](../c12.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
