<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $\mathcal J=\star J$ be the current $(d-1)$-form on an oriented $d$-dimensional spacetime. For a slab bounded by two spacelike hypersurfaces $\Sigma_1,\Sigma_2$ and a side boundary $B$, the [Stokes theorem](../../../../../stokes-theorem.md) gives

$$
0=\int_Vd\mathcal J=\int_{\Sigma_2}\mathcal J-\int_{\Sigma_1}\mathcal J+\int_B\mathcal J.
$$

Thus $Q(\Sigma)=\int_\Sigma\mathcal J$ is conserved if the side flux vanishes, for example for a spatially compact current or appropriate falloff at infinity. With side flux it instead obeys the corresponding charge-balance equation. This is the differential-form version of current conservation.

For the [Abelian Chern--Simons theory](../../../../../abelian-chern-simons-theory.md), take $A\mapsto A+d\chi$ with a smooth compactly supported gauge parameter. The change in the gauge-field term is a boundary term because $d\chi\wedge dA=d(\chi\,dA)$. For the source,

$$
\mathcal J\wedge d\chi=d(\chi\mathcal J)-\chi\,d\mathcal J.
$$

Discarding the boundary terms, the action variation is

$$
\delta_\chi S=c\int\chi\,d\mathcal J.
$$

[Gauge invariance](../../../../../gauge-invariance.md) for every such $\chi$ and $c\ne0$ therefore gives **$d\star J=0$**. If $c=0$, the current decouples and [gauge invariance](../../../../../gauge-invariance.md) places no condition on it. On a spacetime with boundary, boundary conditions or boundary degrees of freedom are also needed to handle the discarded terms; on a nontrivial compact gauge bundle, large-gauge invariance is an additional global issue.

For the field equation, use

$$
\delta(A\wedge dA)=2\delta A\wedge dA-d(A\wedge\delta A).
$$

The [one-form](../../../../../one-form.md) $\delta A$ commutes with the [two-form](../../../../../2-form.md) $\mathcal J$ under the [wedge product](../../../../../exterior-product.md), so

$$
\delta S=\int\delta A\wedge(2dA-c\mathcal J)
$$

up to the boundary term. Consequently

$$
\boxed{2dA=c\star J.}
$$

Applying $d$ and using $d^2=0$ again gives current conservation for $c\ne0$. The factor two comes from varying both occurrences of $A$.

Orient a spatial region $D$ so its boundary is $\gamma$, and define $Q_D=\int_D\mathcal J$. Applying [Stokes theorem](../../../../../stokes-theorem.md) and the field equation yields

$$
\boxed{\Phi=\oint_\gamma A=\int_DdA=\frac c2Q_D.}
$$

For a [U(1) connection](../../../../../u-1-connection.md), in a convention with unit minimal charge, the gauge-invariant quantity is its [holonomy](../../../../../holonomy.md) $e^{i\Phi}$, the Wilson-loop or Aharonov-Bohm phase. A large [gauge transformation](../../../../../gauge-transformation.md) can change the chosen representative of $\Phi$ by $2\pi n$. Therefore **$\Phi$ is a phase angle modulo $2\pi$, rather than an absolute gauge-invariant real number**. A particle of charge $q$ has phase $e^{iq\Phi}$ in the corresponding normalization. The flux-charge relation thus attaches a gauge phase to enclosed charge.

The metric variation requires specifying the independent source. The pure Chern-Simons term $A\wedge dA$ has no metric dependence, hence contributes zero [stress-energy tensor](../../../../../stress-energy-tensor.md). If the [one-forms](../../../../../one-form.md) named in the question have fixed covariant components $A_\mu,J_\mu$, the [Hodge star](../../../../../hodge-star-operator.md) in the source does depend on the metric:

$$
S_{\mathrm{source}}=-c\int d^3x\,\sqrt{-g}\,g^{\rho\sigma}J_\rho A_\sigma.
$$

Using $\delta\sqrt{-g}=-\sqrt{-g}g_{\mu\nu}\delta g^{\mu\nu}/2$ gives

$$
\delta S_{\mathrm{source}}
=-c\int d^3x\,\sqrt{-g}\left[J_{(\mu}A_{\nu)}-\frac12g_{\mu\nu}J_\rho A^\rho\right]\delta g^{\mu\nu}.
$$

Under that literal fixed-one-form convention,

$$
\boxed{T_{\mu\nu}=2cJ_{(\mu}A_{\nu)}-cg_{\mu\nu}J_\rho A^\rho.}
$$

There is another common convention in the topological source theory: hold the conserved [two-form](../../../../../2-form.md) $\mathcal J=\star J$, equivalently the vector current density, fixed as the metric varies. Then both $A\wedge dA$ and $\mathcal J\wedge A$ are metric-independent, and **$T_{\mu\nu}=0$** for this action. These are different variations, not contradictory calculations. The [Chern-Simons source stress convention](../../../../../chern-simons-source-stress-convention.md) explains why a source prescription is necessary; a dynamical matter source would contribute its own action and stress as well.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
