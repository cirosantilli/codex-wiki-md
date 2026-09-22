<h1 id="section-c/c10/heat-exchanges-and-efficiency/solution">Solution</h1>

↑ **Parent:** [Heat exchanges and efficiency](../heat-exchanges-and-efficiency.md)

Use [heat](../../../../../../heat-split.md) into the [gas](../../../../../../gas.md) as positive. The two adiabatic stages have $Q_{12}=Q_{34}=0$. During constant-pressure heating and constant-volume cooling,

$$
\boxed{Q_{23}=C_p(T_3-T_2)>0,\qquad Q_{41}=C_V(T_1-T_4)<0.}
$$

The first law over a complete cycle gives $W_{\rm out}=Q_{23}+Q_{41}$, since the [internal energy](../../../../../../internal-energy-split.md) returns to its initial value. Therefore

$$
\eta=1-\frac{C_V(T_4-T_1)}{C_p(T_3-T_2)}.
$$

Substitute the [temperatures](../../../../../../temperature-split.md):

$$
\frac{T_4-T_1}{T_3-T_2}
=\frac{(V_3/V_2)^\gamma-1}
{(V_1/V_2)^{\gamma-1}(V_3/V_2-1)}
=\frac{V_3^\gamma-V_2^\gamma}{V_1^{\gamma-1}(V_3-V_2)}.
$$

Hence

$$
\boxed{\eta=1-\frac1\gamma
\frac{(V_3/V_1)^\gamma-(V_2/V_1)^\gamma}
{V_3/V_1-V_2/V_1}.}
$$

Equivalently, define compression ratio $r=V_1/V_2$ and cutoff ratio $\rho=V_3/V_2$:

$$
\boxed{\eta=1-\frac{\rho^\gamma-1}{\gamma r^{\gamma-1}(\rho-1)}.}
$$

These formulas use the ideal constant-heat-capacity model and reversible adiabatic strokes. The heat-addition and heat-rejection strokes occur over changing [gas](../../../../../../gas.md) [temperatures](../../../../../../temperature-split.md), unlike the isothermal [heat](../../../../../../heat-split.md) exchanges of a Carnot engine.

## ↑ Ancestors (15)

1. [Heat exchanges and efficiency](../heat-exchanges-and-efficiency.md)
2. [C10](../../c10.md)
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
