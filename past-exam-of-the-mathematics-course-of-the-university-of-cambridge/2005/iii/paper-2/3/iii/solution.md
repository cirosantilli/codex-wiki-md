<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [Weyl group](../../../../../../weyl-group.md) acts on the [weight lattice](../../../../../../weight-lattice.md) by its [root reflections](../../../../../../root-reflection.md) and extends to ring automorphisms of the [group ring of a weight lattice](../../../../../../group-ring-of-a-weight-lattice.md):

$$
w\left(\sum_\lambda a_\lambda e(\lambda)\right)=\sum_\lambda a_\lambda e(w\lambda),\qquad
s_\alpha\lambda=\lambda-\lambda(H_\alpha)\alpha.
$$

[Weights](../../../../../../weight-representation-theory.md) and their multiplicities in a finite-dimensional [Lie algebra representation](../../../../../../lie-algebra-representation.md) of a [semisimple Lie algebra](../../../../../../semisimple-lie-algebra-split.md) are permuted by this action, so its [formal character](../../../../../../formal-character-of-a-weight-module.md) is Weyl-invariant.

Choose a set $\Phi^+$ of [positive roots](../../../../../../positive-root.md) and put

$$
\rho=\frac12\sum_{\alpha\in\Phi^+}\alpha=\sum_i\omega_i,\qquad
A_\nu=\sum_{w\in W}\det(w)e(w\nu).
$$

Here $\omega_i$ are the [fundamental weights](../../../../../../fundamental-weight.md), and $\det(w)=(-1)^{\ell(w)}$, where the [Coxeter length](../../../../../../coxeter-length.md) $\ell(w)$ counts [positive roots](../../../../../../positive-root.md) carried to negative ones. For a [dominant integral weight](../../../../../../dominant-integral-weight.md) $\lambda$, let $L(\lambda)$ denote the finite-dimensional [Irreducible Lie algebra representation](../../../../../../irreducible-lie-algebra-representation.md) of [highest weight](../../../../../../highest-weight-of-a-representation.md) $\lambda$. The [Weyl character formula](../../../../../../weyl-character-formula.md) is

$$
\boxed{\operatorname{char}L(\lambda)=\frac{A_{\lambda+\rho}}{A_\rho}
=\frac{\sum_{w\in W}\det(w)e(w(\lambda+\rho))}
{e(\rho)\prod_{\alpha\in\Phi^+}(1-e(-\alpha))}.}
$$

The second denominator expression is the [Weyl denominator formula](../../../../../../weyl-denominator-formula.md). Both alternants change sign under each [root reflection](../../../../../../root-reflection.md); their quotient is invariant. Although written as a fraction, the theorem asserts that it is a finite element of $\mathbb Z[\Lambda_W]$ with the nonnegative coefficients given by [weight](../../../../../../weight-representation-theory.md) multiplicities. The [highest-weight classification](../../../../../../highest-weight-classification-of-finite-dimensional-semisimple-lie-algebra-modules.md) specifies which $\lambda$ label the irreducibles, while the [root system](../../../../../../root-system.md) and choice of [positive roots](../../../../../../positive-root.md) determine every other term.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
