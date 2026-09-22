<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $a_c\ll R$ be the contact radius of the adhering [neutrophil](../../../../../../neutrophil.md). Indentation is of order $a_c^2/R$, so the elastic [strain](../../../../../../strain.md) is of order $a_c/R$ within a region of volume $a_c^3$. The elastic [energy](../../../../../../energy.md) is consequently $G a_c^5/R^2$, while adhesion lowers the [energy](../../../../../../energy.md) by order $Ja_c^2$. Balancing these terms gives

$$
a_c\sim\left(\frac{JR^2}{G}\right)^{1/3},\qquad \frac{a_c}{R}\sim\left(\frac{J}{GR}\right)^{1/3}.
$$

This estimate requires weak adhesion, $J\ll GR$.

For an [adhesive-cell rolling threshold](../../../../../../adhesive-cell-rolling-threshold.md), assume peeling the rear bonds dissipates work of order $J$ per unit contact area. Rolling through angle $d\theta$ sweeps contact area of order $a_cR\,d\theta$, giving resisting moment $M_r\sim Ja_cR$. A surrounding fluid of [dynamic viscosity](../../../../../../dynamic-viscosity.md) $\eta$ supplies a moment of order $\eta\dot\gamma R^3$. Equating moments yields

$$
\boxed{\dot\gamma_c\sim\frac{Ja_c}{\eta R^2}\sim\frac{J^{4/3}}{\eta G^{1/3}R^{4/3}}.}
$$

A dimensionless numerical coefficient depends on the contact and near-wall [Stokes flow](../../../../../../stokes-flow-split.md). Fluid viscosity is indispensable to a rate estimate, even though the contact model alone specifies only $R,G,J$.

A perfectly reversible elastic adhesive contact does not lose net [energy](../../../../../../energy.md) when an unchanged contact footprint translates. It therefore does not, by itself, justify a finite rolling threshold. The above estimate assumes adhesive hysteresis or irreversible bond peeling. If equilibrium adhesion is $J$ but the work lost during peeling and rebinding is $\Delta J$, retain $a_c\sim(JR^2/G)^{1/3}$ and replace $J$ by $\Delta J$ only in the resisting moment: $\dot\gamma_c\sim\Delta J\,a_c/(\eta R^2)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
