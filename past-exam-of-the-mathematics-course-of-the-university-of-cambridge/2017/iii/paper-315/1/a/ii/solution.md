<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume a homogeneous [ideal gas](../../../../../../../ideal-gas.md), constant [specific-heat ratio](../../../../../../../heat-capacity-ratio.md) $\gamma>1$, and an upward displacement that is an [adiabatic process](../../../../../../../adiabatic-process.md) and maintains pressure balance with its surroundings. If the ambient [temperature](../../../../../../../temperature.md) falls faster with decreasing [pressure](../../../../../../../pressure.md) than the parcel's [adiabatic temperature gradient](../../../../../../../adiabatic-temperature-gradient.md), the parcel becomes hotter and less dense than its surroundings; [buoyancy](../../../../../../../buoyancy.md) amplifies the displacement. This is the [Schwarzschild criterion](../../../../../../../schwarzschild-criterion.md):

$$
\nabla\equiv\frac{d\log T}{d\log P}>\nabla_{\rm ad}
=\frac{\gamma-1}{\gamma}\equiv A.
$$

The [square-root exponential atmospheric profile](../../../../../../../square-root-exponential-atmospheric-profile.md) has

$$
\boxed{\nabla=\frac{2\sqrt{T-T_0}}{\alpha T};\qquad
\text{instability requires }\frac{2\sqrt{T-T_0}}{\alpha T}>A.}
$$

An [atmospheric thermal inversion](../../../../../../../inversion-meteorology.md) with $\alpha<0$ has $\nabla<0$ and is stable to these ordinary adiabatic displacements. For $\alpha>0$, put $s=\sqrt{T-T_0}$. The condition becomes the [quadratic inequality](../../../../../../../quadratic-inequality.md)

$$
A\alpha s^2-2s+A\alpha T_0<0,
$$

intersected with $s\ge0$ and $T_0+s^2>0$. In the usual case $T_0>0$, the maximum gradient occurs at $s=\sqrt{T_0}$, namely $T=2T_0$, and is $1/(\alpha\sqrt{T_0})$. Hence a convectively unstable interval exists precisely when

$$
\boxed{A\alpha\sqrt{T_0}<1,\qquad
s_-<\sqrt{T-T_0}<s_+,\quad
s_\pm=\frac{1\pm\sqrt{1-(A\alpha)^2T_0}}{A\alpha}.}
$$

Equality in the existence condition gives a single neutrally stable point. A molecular-hydrogen-dominated [hot Jupiter](../../../../../../../hot-jupiter.md) with rotational modes active but vibrational excitation and dissociation negligible has approximately $\gamma=7/5$, so $A=2/7$. The existence condition is then $\alpha\sqrt{T_0}<7/2$. For $T_0\le0$ the general inequality above remains valid, but its roots must be intersected with the positive-[temperature](../../../../../../../temperature.md) domain; the positive-$T_0$ maximum formula must not be reused. Composition gradients require the [Ledoux criterion](../../../../../../../ledoux-criterion.md), and dissociation or variable heat capacities change $A$. Sustained [convection](../../../../../../../convection.md) normally adjusts a superadiabatic profile toward an [adiabatic temperature gradient](../../../../../../../adiabatic-temperature-gradient.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 315](../../../../paper-315-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
