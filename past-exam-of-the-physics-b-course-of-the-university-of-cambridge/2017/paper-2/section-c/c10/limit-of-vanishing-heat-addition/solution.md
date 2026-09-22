<h1 id="section-c/c10/limit-of-vanishing-heat-addition/solution">Solution</h1>

↑ **Parent:** [Limit of vanishing heat addition](../limit-of-vanishing-heat-addition.md)

For $\rho\to1^+$, [Taylor expansion](../../../../../../taylor-expansion.md) gives $\rho^\gamma-1=\gamma(\rho-1)+O((\rho-1)^2)$. The [vanishing-cutoff limit of the Diesel cycle](../../../../../../vanishing-cutoff-limit-of-the-diesel-cycle.md) is

$$
\boxed{\eta\longrightarrow1-\frac1{r^{\gamma-1}}
=1-\left(\frac{V_2}{V_1}\right)^{0.4}.}
$$

The maximum [temperature](../../../../../../temperature-split.md) tends to $T_2=T_1r^{\gamma-1}$, while the minimum stays at $T_1$. A Carnot engine between those limiting extrema has

$$
\eta_C=1-\frac{T_1}{T_2}=1-r^{1-\gamma},
$$

so **the limiting efficiencies coincide**. At exactly $V_3=V_2$, however, both [heat](../../../../../../heat-split.md) input and net [work](../../../../../../work.md) vanish, and the cycle retraces its compression [adiabat](../../../../../../adiabat.md). The efficiency there is an undefined $0/0$; the boxed value is the continuous limit for neighbouring nonzero cycles, not finite [work](../../../../../../work.md) at zero [heat](../../../../../../heat-split.md) input.

For a finite cutoff ratio $\rho>1$, the Carnot comparison uses $T_{\max}=T_3=T_1r^{\gamma-1}\rho$, giving $\eta_C=1-1/(r^{\gamma-1}\rho)$. The [Diesel cycle](../../../../../../diesel-cycle.md) has smaller efficiency. For example,

$$
\frac{\rho^\gamma-1}{\gamma(\rho-1)}
=\frac1{\rho-1}\int_1^\rho x^{\gamma-1}\,dx>1>\frac1\rho,
$$

which makes its rejected/input [heat](../../../../../../heat-split.md) ratio larger than the Carnot ratio.

## ↑ Ancestors (15)

1. [Limit of vanishing heat addition](../limit-of-vanishing-heat-addition.md)
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
