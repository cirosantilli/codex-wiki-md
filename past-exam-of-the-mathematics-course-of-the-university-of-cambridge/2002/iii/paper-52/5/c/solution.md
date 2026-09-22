<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\mathcal B_0>0$ be the source [buoyancy flux](../../../../../../buoyancy-flux.md) per unit length. The conversion from the heat-source strength depends on its units: if $F$ is a kinematic temperature-volume flux, $\mathcal B_0=g\beta F$; if it is a physical heat power per unit length, $\mathcal B_0=g\beta F/(\rho_0c_p)$, where $c_p$ is [specific heat capacity at constant pressure](../../../../../../specific-heat-capacity-at-constant-pressure.md). This explicit convention avoids treating heat power as a [buoyancy flux](../../../../../../buoyancy-flux.md) without conversion.

For uniform ambient $N^2=0$, so $\mathcal B=\mathcal B_0$. The ideal pure line-source limit has negligible initial volume and [momentum](../../../../../../momentum.md) transport. The flux equations admit $w=w_*$ constant, $q=2\alpha w_*z$ and $b=\alpha z$. Substituting into the [momentum](../../../../../../momentum.md) equation gives $2\alpha w_*^2=2bG$, and the conserved [buoyancy flux](../../../../../../buoyancy-flux.md) then fixes $2\alpha w_*^3=\mathcal B_0$. Thus

$$
\boxed{2b=2\alpha z,\qquad w=w_* =\left(\frac{\mathcal B_0}{2\alpha}\right)^{1/3},\qquad g'=G=\frac{w_*^2}{z}=\frac{\mathcal B_0^{2/3}}{(2\alpha)^{2/3}z}.}
$$

This verifies all three differential equations, not just their dimensional exponents. The plume grows in width while maintaining constant upward [velocity](../../../../../../velocity.md); its [temperature](../../../../../../temperature.md) anomaly decreases like $z^{-1}$. The zero-height singularity is the ideal point-source limit. A finite source or nonzero [momentum](../../../../../../momentum.md) input introduces a [plume virtual origin](../../../../../../plume-virtual-origin.md) or a forced near-source region; the heat strength alone cannot uniquely determine that finite-source region.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Section C](../../section-c.md)
4. [Paper 52](../../../paper-52-split.md)
5. [Iii](../../../split.md)
6. [2002](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
