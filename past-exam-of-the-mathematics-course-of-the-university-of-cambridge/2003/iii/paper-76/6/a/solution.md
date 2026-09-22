<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume [Boussinesq approximation](../../../../../../boussinesq-approximation.md), no wind, a uniform exterior, negligible source volume, sharp well-mixed internal layers, point-source [pure plume](../../../../../../pure-plume.md) entrainment and thin openings represented by discharge coefficients $C_b,C_t$. Let $g_1'=g\Delta\rho_1/\rho$ be the upper-layer reduced gravity. Steady volume conservation makes the magnitudes of inlet and outlet flow equal to $Q$.

If the opening pressure drops are $\Delta p_b$ and $\Delta p_t$, the orifice laws and hydrostatic pressure difference give

$$
Q=C_bA_b\sqrt{2\Delta p_b/\rho}=C_tA_t\sqrt{2\Delta p_t/\rho},
\qquad \Delta p_b+\Delta p_t=\rho g_1'(H-h_1).
$$

Define the reduced area by

$$
\boxed{A^*=\left[\frac{2}{(C_bA_b)^{-2}+(C_tA_t)^{-2}}\right]^{1/2}.}
$$

Then the throughflow in this [displacement ventilation](../../../../../../displacement-ventilation.md) model is

$$
\boxed{Q_b=Q_t=Q=A^*\sqrt{g_1'(H-h_1)}.}
$$

Lower-layer conservation requires $Q=Q_p(h_1)=CB_1^{1/3}h_1^{5/3}$. Global buoyancy conservation gives $g_1'Q=B_1$. Eliminating $Q,g_1'$ yields

$$
Q^3=(A^*)^2B_1(H-h_1),\qquad
\boxed{\frac{A^*}{H^2C^{3/2}}=\left[\frac{(h_1/H)^5}{1-h_1/H}\right]^{1/2}.}
$$

This uniquely determines an interface height between zero and $H$ for a given positive area parameter. Opening area controls the nondimensional height; source strength controls the density contrast and flow magnitude. Factors of two depend on the stated effective-area convention, which has been fixed explicitly here.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
