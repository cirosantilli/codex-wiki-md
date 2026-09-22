<h1 id="section-a/a1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First solve the [equation of state](../../../../../equation-of-state.md) for the [volume](../../../../../volume-thermodynamics.md):

$$
V(T,p,N)=\frac{Nk_BT}{p}-NA(T).
$$

The [Gibbs free energy](../../../../../gibbs-free-energy.md) has differential $dG=-S\,dT+V\,dp+\mu\,dN$. At fixed [temperature](../../../../../temperature-split.md) and [particle number](../../../../../particle-number.md), integrate $dG=V\,dp$ between the two pressures:

$$
\Delta G=\int_{p_0}^{p_1}\left[\frac{Nk_BT}{p}-NA(T)\right]dp.
$$

Consequently

$$
\boxed{\Delta G=Nk_BT\ln\frac{p_1}{p_0}-NA(T)(p_1-p_0).}
$$

Use $S=-(\partial G/\partial T)_{p,N}$, keeping both endpoint pressures fixed while differentiating the difference:

$$
\boxed{\Delta S=-Nk_B\ln\frac{p_1}{p_0}+NA'(T)(p_1-p_0).}
$$

Equivalently, the [Maxwell relation](../../../../../maxwell-relations.md) $(\partial S/\partial p)_{T,N}=-(\partial V/\partial T)_{p,N}$ gives $-Nk_B/p+NA'(T)$, whose [pressure](../../../../../pressure-split.md) [integral](../../../../../integral-split.md) is the same result. These are the [Gibbs free-energy change for a pressure-linear gas correction](../../../../../gibbs-free-energy-change-for-a-pressure-linear-gas-correction.md) identities. The physical path requires $p_0,p_1>0$ and positive [volume](../../../../../volume-thermodynamics.md) throughout. The correction $A(T)$ has units of [volume](../../../../../volume-thermodynamics.md) per particle, so each term in $\Delta G$ is an [energy](../../../../../energy-split.md) and each term in $\Delta S$ has units of [energy](../../../../../energy-split.md) per kelvin.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [A1](../../a1.md)
3. [Section A](../../../section-a.md)
4. [2018](../../../../2018-split.md)
5. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../../split.md)
6. [Thermal and Statistical Physics course of the University of Cambridge](../../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
