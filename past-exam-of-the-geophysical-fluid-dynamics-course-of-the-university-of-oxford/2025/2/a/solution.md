<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Define the [salinity](../../../../salinity.md) contrast $\Delta S=S_1-S_2$, positive when the warm box is saltier. The linear [equation of state](../../../../equation-of-state.md) gives the cold-minus-warm [density](../../../../density.md) contrast and signed [volume flux](../../../../volumetric-flow-rate.md)

$$
\frac{\rho_2-\rho_1}{\rho_0}=\alpha\Delta T-\beta\Delta S,\qquad
q=k(\alpha\Delta T-\beta\Delta S).
$$

Here $q>0$ represents warm upper water travelling poleward and cold deep water returning equatorward. The $\beta$ in this question is the haline [density](../../../../density.md) coefficient, unrelated to the planetary [vorticity](../../../../vorticity-split.md) gradient in Question 1. The imposed heating and cooling are taken to maintain $\Delta T$.

For the positive circulation shown in the source diagram, the exact stationary [salt budget](../../../../salt-budget.md) of the cold box is

$$
qS_1-(q+E)S_2=0,
\qquad q\Delta S=ES_2.
$$

The precipitation adds no salt. Replacing the salinity multiplying the small compensating [volume flux](../../../../volumetric-flow-rate.md) by a reference $S_0$ gives $q\Delta S\simeq ES_0$. When circulation reverses, the upstream box for the exchange reverses too: the homogenizing exchange is $|q|$, not $q$. In the same reference-salinity approximation the two stationary [salt budgets](../../../../salt-budget.md) reduce to

$$
\boxed{|q|\Delta S=ES_0.}
$$

For example, when $q=-r<0$ and $r>E$, the exact cold-box balance is $(r-E)S_1-rS_2=0$, giving $r\Delta S=ES_1$ and the same leading approximation.

Substitute $\Delta S=ES_0/|q|$ into the [density](../../../../density.md)-driven [volume flux](../../../../volumetric-flow-rate.md) and multiply by $|q|$:

$$
\boxed{q|q|-A|q|+BE=0,\qquad
A=k\alpha\Delta T,\qquad B=k\beta S_0.}
$$

Both $A$ and $B$ have the units of [volume flux](../../../../volumetric-flow-rate.md), so every term has units of squared [volume flux](../../../../volumetric-flow-rate.md). The absolute value expresses the fact that transport in either direction reduces the [salinity](../../../../salinity.md) contrast, while the [density](../../../../density.md) contrast sets its direction.

The requested equation is thus the reference-salinity, or [virtual salt flux](../../../../virtual-salt-flux.md), version of the [two-box overturning model](../../../../two-box-overturning-model.md). If the finite compensating flow is retained exactly with unequal $S_1,S_2$, one has the appropriate upstream salinity on the right-hand side instead of exactly $S_0$. The approximation assumes $|\Delta S|/S_0\ll1$ and $E/|q|\ll1$. Also, for $E>0$, $q=0$ cannot be a steady solution: the imposed freshwater transport would build an uncompensated [salinity](../../../../salinity.md) contrast.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the geophysical fluid dynamics course of the University of Oxford](../../../split.md)
5. [Geophysical fluid dynamics course of the University of Oxford](../../../../geophysical-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
