<h1 id="6/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the corrected [generating series of the Kostant partition function](../../../../../../generating-series-of-the-kostant-partition-function.md) and the permitted [Weyl character formula](../../../../../../weyl-character-formula.md):

$$
\chi_\lambda
=\left(\sum_{w\in W}\varepsilon(w)e^{w(\lambda+\rho)-\rho}\right)
\left(\sum_\nu p(\nu)e^{-\nu}\right).
$$

For a fixed $w$, the coefficient of $e^\mu$ arises exactly when

$$
w(\lambda+\rho)-\rho-\nu=\mu,
\qquad\text{that is,}\qquad
\nu=w(\lambda+\rho)-(\mu+\rho).
$$

There are only finitely many Weyl-group terms, and the [partition function](../../../../../../canonical-partition-function.md) vanishes outside the cone of nonnegative [root](../../../../../../root-of-a-root-system.md) combinations. [Coefficient extraction](../../../../../../coefficient-extraction.md) is therefore legitimate in the formal completion used in the preceding part. Summing the signed contributions proves

$$
\boxed{m_\lambda(\mu)=\sum_{w\in W}\varepsilon(w)\,p\bigl(w(\lambda+\rho)-(\mu+\rho)\bigr).}
$$

This proves the [Kostant multiplicity formula](../../../../../../kostant-multiplicity-formula.md) for every [compact](../../../../../../compact-space.md) [connected](../../../../../../connected-space.md) [Lie group](../../../../../../lie-group.md), not just the [unitary groups](../../../../../../unitary-group.md). In the presence of a central [torus](../../../../../../torus.md), [roots](../../../../../../root-of-a-root-system.md) have zero central component, so the [partition function](../../../../../../canonical-partition-function.md) automatically gives zero for any incompatible central [weight](../../../../../../weight-representation-theory.md). Also $\rho$ need not itself be an integral [weight](../../../../../../weight-representation-theory.md) for the given global [group](../../../../../../group-split.md): $w\rho-\rho$ always belongs to the [root lattice](../../../../../../root-lattice.md), so every argument in the formula is nevertheless integral whenever $\lambda$ and $\mu$ are integral [group](../../../../../../group-split.md) [weights](../../../../../../weight-representation-theory.md).

As a normalization check, for $SU(2)$ write a [highest weight](../../../../../../highest-weight-of-a-representation.md) as the [nonnegative integer](../../../../../../natural-number.md) $\ell$, with [positive root](../../../../../../positive-root.md) $2$ and $\rho=1$. The two Weyl-group terms give

$$
m_\ell(\mu)=p(\ell-\mu)-p(-\ell-\mu-2).
$$

Since $p(a)=1$ precisely when $a$ is even and nonnegative, this is one for $\mu=\ell,\ell-2,\ldots,-\ell$ and zero otherwise, including the cancellation below the lowest [weight](../../../../../../weight-representation-theory.md). This recovers the full familiar [weight string](../../../../../../weight-string.md).

## ↑ Ancestors (11)

1. [2](../2.md)
2. [6](../../6.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
