<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $p_a,p_v,p_{LV}$ be pressures in the [arterial reservoir](../../../../arterial-reservoir.md), [venous reservoir](../../../../venous-reservoir.md) and [left ventricle](../../../../left-ventricle.md). Constant [vascular compliances](../../../../vascular-compliance.md) $C_a,C_v$ relate volume changes to [pressure](../../../../pressure-split.md) changes. The [ventricular elastance](../../../../ventricular-elastance.md) relation is

$$
V_{LV}=V_0+\frac{p_{LV}}{E_{LV}(t)},
$$

where $V_0$ is the unstressed ventricular volume and $E_{LV}(t)>0$ is the time-dependent inverse compliance. Define the positive part $[x]_+=\max(x,0)$. The systemic, aortic-valve and mitral-valve flows are

$$
Q_c=\frac{p_a-p_v}{R_c},\qquad Q_a=\frac{[p_{LV}-p_a]_+}{R_a},\qquad Q_v=\frac{[p_v-p_{LV}]_+}{R_v}.
$$

Each $R$ is a positive [hydraulic resistance](../../../../hydraulic-resistance.md). The [aortic valve](../../../../aortic-valve.md) permits outflow only when ventricular [pressure](../../../../pressure-split.md) exceeds arterial [pressure](../../../../pressure-split.md), and the [mitral valve](../../../../mitral-valve.md) permits filling only when venous [pressure](../../../../pressure-split.md) exceeds ventricular [pressure](../../../../pressure-split.md).

[Mass conservation](../../../../mass-conservation.md), with [blood](../../../../blood.md) treated as incompressible, gives

$$
C_a\dot p_a=Q_a-Q_c,\qquad C_v\dot p_v=Q_c-Q_v,\qquad\frac{d}{dt}\left(\frac{p_{LV}}{E_{LV}}\right)=Q_v-Q_a.
$$

Substitution and multiplication of the first two equations by $R_c$ give exactly

$$
\boxed{\begin{aligned}
R_cC_a\dot p_a&=-(p_a-p_v)+\frac{R_c}{R_a}[p_{LV}-p_a]_+,\\
R_cC_v\dot p_v&=(p_a-p_v)-\frac{R_c}{R_v}[p_v-p_{LV}]_+,\\
\frac{d}{dt}(p_{LV}/E_{LV})&=\frac{[p_v-p_{LV}]_+}{R_v}-\frac{[p_{LV}-p_a]_+}{R_a}.
\end{aligned}}
$$

Adding the three original balances gives zero total volume change. This is a [three-compartment ventricular circulation model](../../../../three-compartment-ventricular-circulation-model.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the mathematical physiology course of the University of Oxford](../../../split.md)
5. [Mathematical physiology course of the University of Oxford](../../../../mathematical-physiology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
