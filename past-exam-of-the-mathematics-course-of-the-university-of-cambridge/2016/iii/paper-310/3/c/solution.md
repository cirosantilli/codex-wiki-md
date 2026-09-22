<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The instantaneous-decay approximation keeps the [scale factor](../../../../../../scale-factor-cosmology.md) and physical volume fixed across the decay. Energy conservation and rapid thermalization give

$$
\rho_{r,+}=\rho_{r,-}+\rho_{\phi,-}\simeq\frac{3M_{\rm Pl}^2}{t_d^2},
\qquad
s_+=c_1g_\star\left(\frac{3M_{\rm Pl}^2}{c_2g_\star t_d^2}\right)^{3/4}.
$$

Meanwhile the abundance relation gives $s_-=\rho_{\phi,-}/(Ym)\simeq3M_{\rm Pl}^2/(Ym\,t_d^2)$. Dividing yields the **entropy-injection factor**

$$
\boxed{\frac{s_+}{s_-}\simeq
\frac{c_1}{3}\left(\frac3{c_2}\right)^{3/4}g_\star^{1/4}
\frac{Ym\sqrt{t_d}}{\sqrt{M_{\rm Pl}}}.}
$$

There is a numerical error in the printed coefficient: part (c) omits the factor $1/3$. The denominator $s_-=3M_{\rm Pl}^2/(Ym\,t_d^2)$ supplies that factor, while the radiation energy contributes $3^{3/4}$ to the numerator. Thus the consistent coefficient is $c_1 3^{-1/4}c_2^{-3/4}$, rather than $c_1 3^{3/4}c_2^{-3/4}$. Both cannot follow from the stated part (b) using the same decay-time approximation.

Its increase is especially transparent without dropping the original radiation. Let $R=\rho_{\phi,-}/\rho_{r,-}$. At unchanged $g_\star$, $T_+^4/T_-^4=1+R$, so

$$
\boxed{\frac{s_+}{s_-}=\left(\frac{T_+}{T_-}\right)^3
=(1+R)^{3/4}>1.}
$$

Relic domination means $R\gg1$, so the leading estimate is much larger than one. This is [entropy production by decay of a dominant relic](../../../../../../entropy-production-by-decay-of-a-dominant-relic.md).

There is no conflict with part (a). The equilibrium gas before the decay was a separately conserved, reversibly expanding system. During decay it receives energy from the nonthermal relic, and the decay products thermalize irreversibly. Its [cosmological perfect-fluid continuity equation](../../../../../../cosmological-perfect-fluid-continuity-equation.md) now has an energy-injection source, so $d(\rho_rV)+P_r\,dV$ does not vanish. The assumptions behind [cosmological entropy conservation](../../../../../../cosmological-entropy-conservation.md) therefore fail during the event. Moreover the zero-chemical-potential equilibrium expression in part (a) cannot be imposed on the decoupled relic as though it were already part of that same equilibrium radiation bath. The [Second law of thermodynamics](../../../../../../second-law-of-thermodynamics.md) permits, and here requires, the resulting entropy increase.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 310](../../../paper-310-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
