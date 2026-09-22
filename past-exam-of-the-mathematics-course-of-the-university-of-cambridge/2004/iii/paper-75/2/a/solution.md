<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\beta$ for the [thermal expansion coefficient](../../../../../../thermal-expansion-coefficient.md), $\nu$ for [kinematic viscosity](../../../../../../kinematic-viscosity.md), $\kappa$ for [thermal diffusivity](../../../../../../thermal-diffusivity.md), and $k_T=\rho c_p\kappa$ for [thermal conductivity](../../../../../../thermal-conductivity.md). For a temperature difference $\Delta>0$ across depth $h$,

$$
\mathrm{Ra}=\frac{g\beta\Delta h^3}{\nu\kappa},\qquad \mathrm{Nu}=\frac{qh}{k_T\Delta}.
$$

The [four-thirds convective heat-transfer law](../../../../../../four-thirds-convective-heat-transfer-law.md) posits $\mathrm{Nu}=C\mathrm{Ra}^{1/3}$ at high [Rayleigh number](../../../../../../rayleigh-number.md), and therefore

$$
\boxed{q=K\Delta^{4/3},\qquad K=Ck_T\left(\frac{g\beta}{\nu\kappa}\right)^{1/3}}.
$$

The layer depth cancels. A useful physical justification is a mixed interior with thin conductive [boundary layers](../../../../../../boundary-layer.md) of thickness $\delta$, each maintained near a fixed critical local [Rayleigh number](../../../../../../rayleigh-number.md): $g\beta\Delta_b\delta^3/(\nu\kappa)\sim\mathrm{Ra}_{\rm crit}$ and $q\sim k_T\Delta_b/\delta$. Eliminating $\delta$ gives the exponent $4/3$. Whether $\Delta$ denotes the whole-layer contrast or the drop across one [boundary layer](../../../../../../boundary-layer.md) changes the coefficient, not the exponent.

Assume [Boussinesq approximation](../../../../../../boussinesq-approximation.md), constant material properties, a laterally extensive statistically turbulent [Rayleigh-Bénard convection](../../../../../../rayleigh-benard-convection.md) layer, negligible side-wall [heat transfer](../../../../../../heat-transfer.md), no rotation or imposed shear, approximately uniform bulk temperature, and the same specified [Prandtl number](../../../../../../prandtl-number.md) regime when choosing $C$. The closure is empirical and regime dependent; high [Rayleigh number](../../../../../../rayleigh-number.md) alone does not make it exact or extend it to the impulsive conductive initial transient.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
