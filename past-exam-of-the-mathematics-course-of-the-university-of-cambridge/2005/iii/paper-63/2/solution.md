<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Hold the metric fixed when varying the [gauge potential](../../../../../gauge-field.md), put $F=dA$, and take variations with compact support or with appropriate fixed boundary data. The [Hodge star operator](../../../../../hodge-star-operator.md) then gives

$$
\delta S_{\rm kin}=-\int d(\delta A)\wedge *F=-\int\delta A\wedge d*F-\int d(\delta A\wedge *F).
$$

For the Abelian [Chern-Simons 5-form](../../../../../chern-simons-5-form.md), the two occurrences of $F$ commute as even-degree [differential forms](../../../../../differential-form-split.md). Since $dF=0$,

$$
\delta(A\wedge F\wedge F)=\delta A\wedge F\wedge F+2A\wedge d(\delta A)\wedge F
=3\delta A\wedge F\wedge F-2d(A\wedge\delta A\wedge F).
$$

The factor three comes from all three appearances of $A$, including those hidden in $F=dA$. The bulk variation is therefore

$$
\delta S=\int\delta A\wedge(-d*F+3cF\wedge F)+\text{boundary terms},
$$

and the [Abelian Chern-Simons five-form field equation](../../../../../abelian-chern-simons-five-form-field-equation.md) is

$$
\boxed{d*F=3cF\wedge F,\qquad dF=0.}
$$

Under an Abelian [gauge transformation](../../../../../gauge-transformation.md) $A\mapsto A+d\lambda$, the [gauge field strength](../../../../../gauge-field-strength.md) stays fixed and the action changes by

$$
\Delta S=c\int d\lambda\wedge F\wedge F=c\int d(\lambda F\wedge F)=c\int_{\partial M}\lambda F\wedge F.
$$

Thus the local integrand is not gauge invariant, but its change is a boundary term by the [Generalized Stokes theorem](../../../../../generalized-stokes-theorem.md). With the stated boundary conditions the variational bulk equations are unchanged; they depend only on $F$ and the metric, so they are manifestly gauge invariant. On a spacetime with boundary, gauge transformations nonzero at the boundary require boundary conditions or boundary degrees of freedom; the bulk claim does not assert invariance of every possible boundary action.

For the metric variation, write the kinetic action in components,

$$
S_{\rm kin}=-\frac14\int d^5x\sqrt{-g}\,F_{\rho\sigma}F^{\rho\sigma}.
$$

At fixed covariant components $A_\mu$ and $F_{\mu\nu}$,

$$
\delta\sqrt{-g}=-\frac12\sqrt{-g}\,g_{\mu\nu}\delta g^{\mu\nu},\qquad
\delta(F_{\rho\sigma}F^{\rho\sigma})=2F_{\mu\rho}F_\nu{}^\rho\delta g^{\mu\nu}.
$$

Substituting into the given definition of the [stress-energy tensor](../../../../../stress-energy-tensor.md) yields

$$
\boxed{T_{\mu\nu}=F_{\mu\rho}F_\nu{}^\rho-\frac14g_{\mu\nu}F_{\rho\sigma}F^{\rho\sigma}.}
$$

The [Chern-Simons 5-form](../../../../../chern-simons-5-form.md) uses only [wedge products of differential forms](../../../../../wedge-product-of-differential-forms.md) and orientation, with no metric or [Hodge star operator](../../../../../hodge-star-operator.md). Its bulk metric derivative is zero, so **the Chern-Simons term contributes no bulk stress-energy tensor**. The displayed tensor is generally not traceless in five dimensions: $T^\mu{}_\mu=-F_{\rho\sigma}F^{\rho\sigma}/4$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
