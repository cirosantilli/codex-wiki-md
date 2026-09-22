<h1 id="section-b/b8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An Euler strut is a slender elastic column under axial compression. Let its [bending stiffness](../../../../../../bending-stiffness.md) about the weaker section axis be $EI_A$ and its [length](../../../../../../length.md) be $L$. With small lateral deflection $y(x)$ and a dead compressive load $P$, the quadratic total [potential energy](../../../../../../potential-energy.md) is

$$
\Pi[y]=\frac12\int_0^L EI_A(y'')^2\,dx
-\frac P2\int_0^L(y')^2\,dx.
$$

The first term is bending [energy](../../../../../../energy-split.md); the negative term is [work](../../../../../../work.md) released by the load as bending shortens the end-to-end distance. Stationarity gives $EI_Ay''''+Py''=0$. For pinned ends, $y=y''=0$ at $0,L$, and $y\propto\sin(n\pi x/L)$ requires $P_n=n^2\pi^2EI_A/L^2$. The first instability is [Euler's critical load](../../../../../../euler-s-critical-load.md),

$$
\boxed{P_{\rm cr}=\frac{\pi^2EI_A}{L^2}.}
$$

Below this load, the straight state has positive quadratic [energy](../../../../../../energy-split.md) against these perturbations. At the threshold, the lowest bending mode has zero quadratic restoring [energy](../../../../../../energy-split.md); above it the straight state is unstable. For a rectangular section, $I_A=bh^3/12$ about the appropriate bending axis, so the smaller [second moment of area](../../../../../../second-moment-of-area.md) controls the first buckling direction.

Endpoint [constraints](../../../../../../constraint-mechanics.md) matter. Write $P_{\rm cr}=\pi^2EI_A/(KL)^2$: $K=1$ for pinned-pinned, $2$ for fixed-free and $1/2$ for fixed-fixed conditions. This elastic instability differs from compressive material failure. Imperfections cause bending before the ideal threshold, and a short column may yield before [Euler buckling](../../../../../../euler-s-critical-load.md) occurs.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [B8](../../b8.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2017](../../../../split.md)
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
