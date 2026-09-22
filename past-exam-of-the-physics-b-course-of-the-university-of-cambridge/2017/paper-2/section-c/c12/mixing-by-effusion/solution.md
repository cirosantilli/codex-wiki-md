<h1 id="section-c/c12/mixing-by-effusion/solution">Solution</h1>

↑ **Parent:** [Mixing by effusion](../mixing-by-effusion.md)

Let L be the vessel initially containing [argon](../../../../../../argon.md) and R the vessel initially containing [helium](../../../../../../helium.md). Both have [volume](../../../../../../volume-thermodynamics.md) $V$ and fixed [temperature](../../../../../../temperature-split.md) $T_0$, and the aperture has [area](../../../../../../surface-area.md) $A_h$. The incoming and outgoing rates of each species must be considered separately. For species $s$,

$$
\frac{dn_{s,L}}{dt}=-\frac{A_h\overline v_s}{4V}(n_{s,L}-n_{s,R}),
\qquad n_{s,L}+n_{s,R}=n_0.
$$

Thus its density difference relaxes exponentially with [time](../../../../../../time-in-physics.md) constant

$$
\tau_s=\frac{2V}{A_h\overline v_s},\qquad
\overline v_s=\sqrt{\frac{8k_BT_0}{\pi m_s}}.
$$

The [two-vessel effusive mixing](../../../../../../two-vessel-effusive-mixing.md) solution for the four densities is

$$
\boxed{\begin{aligned}
n_{{\rm Ar},L}&=\tfrac12n_0(1+e^{-t/\tau_{\rm Ar}}),&
n_{{\rm Ar},R}&=\tfrac12n_0(1-e^{-t/\tau_{\rm Ar}}),\\
n_{{\rm He},L}&=\tfrac12n_0(1-e^{-t/\tau_{\rm He}}),&
n_{{\rm He},R}&=\tfrac12n_0(1+e^{-t/\tau_{\rm He}}).
\end{aligned}}
$$

Using atomic masses of approximately $40$ and $4$ atomic [mass](../../../../../../mass.md) units gives $\tau_{\rm He}/\tau_{\rm Ar}\simeq1/\sqrt{10}\simeq0.32$. [Helium](../../../../../../helium.md) therefore transfers faster. Each species eventually reaches $n_0/2$ in each vessel, but its transient is different. In particular, the total density temporarily rises in the initially [argon](../../../../../../argon.md) vessel and falls in the initially [helium](../../../../../../helium.md) vessel, before both return to $n_0$.

<a id="section-c/c12/mixing-by-effusion/image-species-densities-during-effusive-mixing-of-initially-separated-argon-and-helium"></a>
![](../../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2-2017-effusive-mixing.png)

**[Figure 5](#section-c/c12/mixing-by-effusion/image-species-densities-during-effusive-mixing-of-initially-separated-argon-and-helium). Species densities during effusive mixing of initially separated argon and helium**. Original solutions of the equal-volume, equal-temperature rate equations, with the helium rate faster by sqrt(10). The dashed total densities show the temporary pressure imbalance even though both temperatures are equal. Each species ultimately has density n0/2 in each vessel.

For unequal maintained [temperatures](../../../../../../temperature-split.md) $T_L,T_R$, replace the rate equation by

$$
\dot n_{s,L}=-\frac{A_h}{4V}\left[\overline v_s(T_L)n_{s,L}-\overline v_s(T_R)n_{s,R}\right].
$$

With each species' total density sum still $n_0$, its final densities and relaxation [time](../../../../../../time-in-physics.md) are

$$
\boxed{n_{s,L}^{\infty}=\frac{n_0\sqrt{T_R}}{\sqrt{T_L}+\sqrt{T_R}},\qquad
n_{s,R}^{\infty}=\frac{n_0\sqrt{T_L}}{\sqrt{T_L}+\sqrt{T_R}},\qquad
\tau_s=\frac{4V}{A_h[\overline v_s(T_L)+\overline v_s(T_R)]}.}
$$

Every species has the same final density ratio $\sqrt{T_R/T_L}$ and partial-pressure ratio $\sqrt{T_L/T_R}$. Thus there is no permanent composition separation in this ideal steady state, although the rates remain [mass](../../../../../../mass.md) dependent. A maintained hot side has lower density and higher [pressure](../../../../../../pressure-split.md). Equal [particle](../../../../../../particle-physics.md) rates do not imply [thermal equilibrium](../../../../../../thermal-equilibrium-split.md): atoms arriving from the hotter side carry more [energy](../../../../../../energy-split.md), so external heating and cooling are required to hold different [temperatures](../../../../../../temperature-split.md). The model assumes thin-hole [effusion](../../../../../../effusion.md), local equilibrium within each vessel and negligible aperture [volume](../../../../../../volume-thermodynamics.md).

## ↑ Ancestors (15)

1. [Mixing by effusion](../mixing-by-effusion.md)
2. [C12](../../c12.md)
3. [Section C](../../../section-c.md)
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
