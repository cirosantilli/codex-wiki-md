<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the metric [Levi-Civita connection](../../../../../levi-civita-connection.md) and hold the covariant potential $A_a$ fixed when varying the metric. Symmetry of the connection cancels its terms in the [electromagnetic field tensor](../../../../../electromagnetic-field-tensor.md):

$$
F_{ab}=\nabla_aA_b-\nabla_bA_a=\partial_aA_b-\partial_bA_a.
$$

The [Electromagnetic Bianchi identity](../../../../../electromagnetic-bianchi-identity.md) follows from commuting partial derivatives, or $F=dA$ and $d^2=0$. Written covariantly it is $\nabla_cF_{ab}+\nabla_aF_{bc}+\nabla_bF_{ca}=0$, since total antisymmetrization also cancels the symmetric connection terms. Hence $\boxed{F_{[ab;c]}=0}$ without using any field equation.

For the potential variation, $\delta F_{ab}=\nabla_a\delta A_b-\nabla_b\delta A_a$. Antisymmetry in the [Maxwell action](../../../../../maxwell-action.md) gives

$$
\delta_AS=-\frac1{4\pi}\int\sqrt{-g}\,F^{ab}\nabla_a\delta A_b\,d^4x=-\frac1{4\pi}\int\sqrt{-g}\,(\nabla_bF^{ab})\delta A_a\,d^4x,
$$

where the second equality is integration by parts followed by relabeling; compactly supported variations, or vanishing boundary variations, remove the surface term. Arbitrary $\delta A_a$ therefore give the source-free [Maxwell equations](../../../../../maxwell-equations.md)

$$
\boxed{\nabla_bF^{ab}=0.}
$$

No gauge fixing of $A$ is needed for this variational calculation.

In signature $(+---)$ define the [Hilbert stress-energy tensor](../../../../../hilbert-stress-energy-tensor.md) by $\delta_gS=\tfrac12\int\sqrt{-g}\,T_{ab}\delta g^{ab}\,d^4x$. Since the independent covariant potential makes $F_{ab}$ metric independent,

$$
\delta\sqrt{-g}=-\tfrac12\sqrt{-g}\,g_{ab}\delta g^{ab},\qquad\delta(F_{cd}F^{cd})=2F_a{}^cF_{bc}\delta g^{ab}.
$$

Combining these two terms yields the [electromagnetic stress-energy tensor](../../../../../electromagnetic-stress-energy-tensor.md)

$$
\boxed{T^{ab}=\frac1{4\pi}\left[-F^a{}_cF^{bc}+\frac14g^{ab}F_{cd}F^{cd}\right].}
$$

Equivalently $\delta S=-\tfrac12\int\sqrt{-g}\,T^{ab}\delta g_{ab}$. The overall stress-variation sign has been matched to the signature and action. As a check, in an orthonormal frame $F_{cd}F^{cd}=2(B^2-E^2)$ and $T^{00}=(E^2+B^2)/(8\pi)>0$ for a nonzero field; copying a mostly-plus formula without changing conventions would fail this check.

Let $J^a=\nabla_bF^{ab}$. Contract the Bianchi identity with $F^{bc}$ to obtain $2F^{bc}\nabla_bF_{ac}=\tfrac12\nabla_a(F_{cd}F^{cd})$, hence $F^{bc}\nabla_bF^a{}_c=\tfrac14\nabla^a(F_{cd}F^{cd})$. Differentiating the stress tensor cancels these derivative terms and gives the [electromagnetic stress-energy divergence identity](../../../../../electromagnetic-stress-energy-divergence-identity.md)

$$
\boxed{\nabla_bT^{ab}=\frac1{4\pi}F^a{}_cJ^c.}
$$

Thus Maxwell's equation implies stress conservation for any field. Conversely, where the matrix $F^a{}_c$ is nonsingular, conservation implies $J^c=0$ by matrix inversion. When it is singular, conservation only says that $J$ lies in its kernel, so the converse cannot be inferred without the printed nonsingularity assumption.

For the first-order formulation, temporarily call the independently constructed potential curvature $f_{ab}(A)=\nabla_aA_b-\nabla_bA_a$. In the [first-order Maxwell action](../../../../../first-order-maxwell-action.md), vary the independent antisymmetric $F^{ab}$, with $F_{ab}=g_{ac}g_{bd}F^{cd}$. Its variation is

$$
\delta_FS_{\rm first}=\frac1{8\pi}\int\sqrt{-g}\,[F_{ab}-f_{ab}(A)]\delta F^{ab}\,d^4x,
$$

so $F_{ab}=f_{ab}(A)$. Varying $A$ independently gives exactly $\nabla_bF^{ab}=0$, by the same integration-by-parts calculation as before. Eliminating the auxiliary field algebraically makes the integrand $f^{ab}f_{ab}-2f^{ab}f_{ab}=-f^{ab}f_{ab}$, recovering the original [Maxwell action](../../../../../maxwell-action.md). The Bianchi identity then follows from $f=dA$. Metric variation also agrees after elimination: the chain-rule term from the eliminated field multiplies its already vanishing field equation. Thus the two actions give the same source-free electromagnetic dynamics and stress tensor. The Palatini procedure here means independent first-order field variables, not an additional variation of the spacetime connection.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
