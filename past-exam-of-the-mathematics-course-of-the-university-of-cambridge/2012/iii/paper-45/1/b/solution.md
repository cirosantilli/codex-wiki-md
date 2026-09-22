<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [supercharge](../../../../../../supersymmetry-generator.md) is an odd [Weyl spinor](../../../../../../weyl-spinor.md) generator. The mixed [anticommutator](../../../../../../anticommutator.md) has one undotted and one dotted index, hence transforms as a [Lorentz four-vector](../../../../../../four-vector.md). In the minimal [Super-Poincaré algebra](../../../../../../super-poincare-algebra.md), its only spacetime generator is the [four-momentum](../../../../../../four-momentum.md), so covariance fixes it to $c\sigma^\mu_{\alpha\dot\beta}P_\mu$. Normalizing the charges canonically fixes $c=2$:

$$
\boxed{\{Q_\alpha,\bar Q_{\dot\beta}\}
=2\sigma^\mu_{\alpha\dot\beta}P_\mu.}
$$

The number two is a normalization, not something Lorentz covariance alone could fix under $Q\mapsto aQ$.

For an explicit closure calculation, use left [Grassmann derivatives](../../../../../../grassmann-derivative.md) in [superspace](../../../../../../superspace.md) and the differential translation convention $P_\mu=i\partial_\mu$:

$$
Q_\alpha=\frac\partial{\partial\theta^\alpha}
-i\sigma^\mu_{\alpha\dot\beta}\bar\theta^{\dot\beta}\partial_\mu,
\qquad
\bar Q_{\dot\beta}=-\frac\partial{\partial\bar\theta^{\dot\beta}}
+i\theta^\alpha\sigma^\mu_{\alpha\dot\beta}\partial_\mu.
$$

Each of the two derivative-coordinate cross terms contributes $i\sigma^\mu\partial_\mu$; the other terms cancel by anticommutativity. This proves the displayed coefficient. The same calculation gives $\{Q,Q\}=\{\bar Q,\bar Q\}=0$ and $[P_\mu,Q]=[P_\mu,\bar Q]=0$. There is no scalar central charge for a single [supersymmetry](../../../../../../supersymmetry-split.md) label: symmetry of the [anticommutator](../../../../../../anticommutator.md) is incompatible with a term proportional only to the antisymmetric $\epsilon_{\alpha\beta}$.

In the massive rest frame $P_\mu=(m,0,0,0)$, the mixed relation is $\{Q_\alpha,Q_\beta^\dagger\}=2m\delta_{\alpha\beta}$. These positive [canonical anticommutation relations](../../../../../../canonical-anticommutation-relations.md) supply the input for the normalization and finite [fermionic Fock space](../../../../../../fermionic-fock-space.md) in the question-level continuation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
