<h1 id="b/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

[Systole](../../../../systole.md) is ventricular contraction and ejection; [diastole](../../../../diastole.md) includes ventricular relaxation and filling. Let $V_a,V_v,V_{LV}$ denote arterial, venous and left-ventricular blood volumes. Let $Q^+$ flow through the aortic valve into the arteries, $Q_c$ through the peripheral circulation, and $Q^-$ through the mitral valve into the ventricle. Conservation of volume gives

$$
\boxed{\dot V_a=Q^+-Q_c,\quad\dot V_v=Q_c-Q^-,\quad\dot V_{LV}=Q^--Q^+.}
$$

The same $Q_c$ leaves arteries and enters veins because the capillary compartment has no changing stored volume in this approximation. Adding the equations conserves total modeled blood volume.

Use constant [vascular compliances](../../../../vascular-compliance.md) $C_a,C_v$, with $\dot V_a=C_a\dot p_a$ and $\dot V_v=C_v\dot p_v$, and [ventricular elastance](../../../../ventricular-elastance.md) $p_{LV}=E_{LV}(t)(V_{LV}-V_0)$. The [hydraulic resistances](../../../../hydraulic-resistance.md) and ideal one-way valves give

$$
Q_c=\frac{p_a-p_v}{R_c},\qquad Q^+=\frac{[p_{LV}-p_a]^+}{R_a},\qquad Q^-=\frac{[p_v-p_{LV}]^+}{R_v},
$$

where $[z]^+=\max(z,0)$. Substitution into the conservation equations gives the two stated arterial/venous pressure equations. Since $V_{LV}-V_0=p_{LV}/E_{LV}$, differentiating this identity gives the third equation. The positive parts encode valve closure against a reverse pressure difference.

During isovolumetric contraction both valves are closed. Let $V^+$ be the end-diastolic ventricular volume, $V_0$ its unstressed reference volume, and $p_a^+$ arterial pressure before ejection. The rapidly raised elastance generates $E_s(V^+-V_0)$, so the aortic valve opens if $\boxed{E_s(V^+-V_0)>p_a^+}$.

During ejection, $R_a/R_c\ll1$ makes the open-valve pressure drop small on the peripheral drainage time scale, so $p_{LV}\approx p_a$. The mitral valve is closed, and adding arterial and ventricular volume balances eliminates $Q^+$. With $p_v\ll p_a$ this gives

$$
R_cC_a\dot p_a+R_c\frac{d(p_a/E_{LV})}{dt}\approx-p_a.
$$

For approximately constant systolic elastance, set $C_s=1/E_s$ and reset time to the start of the slow ejection phase. Then

$$
\boxed{p_a(t)\approx\hat p_a\exp\!\left[-\frac{t}{R_c(C_a+C_s)}\right].}
$$

Here $\hat p_a$ is the matched pressure at that start. If peripheral outflow is negligible during the preceding [rapid artery-ventricle pressure equilibration](../../../../rapid-artery-ventricle-pressure-equilibration.md), conservation gives the more explicit $\hat p_a=[C_ap_a^++V^+-V_0]/(C_a+C_s)$.

After aortic closure the ventricular volume is fixed at the end-systolic value $V^-$. Relaxation decreases $E_{LV}$ until the mitral valve opens at $p_{LV}=p_v$, hence $\boxed{E_{LV}\sim p_v/(V^--V_0)}$, with $p_v$ the venous filling pressure at opening. During filling the aortic valve is closed, so $R_cC_a\dot p_a=-(p_a-p_v)\approx-p_a$. With $p_a^-$ the arterial pressure at the start of filling and time reset there,

$$
\boxed{p_a(t)\approx p_a^-e^{-t/(R_cC_a)}.}
$$

The change from $C_a+C_s$ to $C_a$ is physical: the ejecting ventricle shares the arterial pressure during systole, whereas a closed aortic valve disconnects it during filling.

## ↑ Ancestors (12)

1. [7](../7.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the mathematics and the environment and mathematical physiology course of the University of Oxford](../../../split.md)
5. [Mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../mathematics-and-the-environment-and-mathematical-physiology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
