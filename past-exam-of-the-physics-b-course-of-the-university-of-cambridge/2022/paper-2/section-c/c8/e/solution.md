<h1 id="section-c/c8/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

This is the [Brayton cycle](../../../../../../brayton-cycle.md). Assume fixed gas amount, constant [heat capacities](../../../../../../heat-capacity.md), and internally reversible [adiabatic processes](../../../../../../adiabatic-process.md), as intended by the ideal engine model. Put $r_p=p_h/p_l=p_2/p_1>1$ and

$$
a=\frac{\gamma-1}{\gamma},\qquad k=r_p^a.
$$

Combining $pV^\gamma=\text{constant}$ with the [ideal gas law](../../../../../../ideal-gas-law.md) gives $T\propto p^{(\gamma-1)/\gamma}$ along either [reversible ideal-gas adiabat](../../../../../../reversible-ideal-gas-adiabat.md). Therefore

$$
\frac{T_2}{T_1}=k,\qquad \frac{T_3}{T_4}=k,
\qquad T_3-T_2=k(T_4-T_1).
$$

During a constant-pressure process the [heat](../../../../../../heat-split.md) supplied equals the [enthalpy](../../../../../../enthalpy-split.md) increase. If $C_p$ is the molar [heat capacity at constant pressure](../../../../../../heat-capacity-at-constant-pressure.md), the positive [heat](../../../../../../heat-split.md) input and output are

$$
Q_{\rm in}=nC_p(T_3-T_2),\qquad
Q_{\rm out}=nC_p(T_4-T_1).
$$

The insulated branches exchange no [heat](../../../../../../heat-split.md), so the [first law of thermodynamics](../../../../../../first-law-of-thermodynamics-split.md) gives $W=Q_{\rm in}-Q_{\rm out}$. Hence

$$
\boxed{\eta=1-\frac{Q_{\rm out}}{Q_{\rm in}}=1-\frac1k=1-\left(\frac{p_2}{p_1}\right)^{(1-\gamma)/\gamma}.}
$$

An [adiabatic process](../../../../../../adiabatic-process.md) alone need not be an [isentropic process](../../../../../../isentropic-process.md); the relations used here also require internal reversibility. Dissipative compression or expansion would require extra information and would not, in general, obey this efficiency formula.

## ↑ Ancestors (15)

1. [E](../e.md)
2. [C8](../../c8.md)
3. [Section C](../../../section-c.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2022](../../../../split.md)
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
