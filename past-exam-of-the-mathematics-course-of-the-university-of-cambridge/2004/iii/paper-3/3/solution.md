<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $\mathfrak g$ be a finite-dimensional complex [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md), choose a [Cartan subalgebra](../../../../../cartan-subalgebra.md) $\mathfrak t$ and a set $R^+$ of [positive roots](../../../../../positive-root.md), and write $W$ for the [Weyl group](../../../../../weyl-group.md). Let $\lambda$ be a [dominant integral weight](../../../../../dominant-integral-weight.md) and $L(\lambda)$ the finite-dimensional irreducible [highest-weight representation](../../../../../highest-weight-representation.md) with that highest weight. If $L(\lambda)_\mu$ denotes its [weight space](../../../../../weight-space.md) of weight $\mu$, its [formal character](../../../../../formal-character-of-a-weight-module.md) is $\operatorname{ch}L(\lambda)=\sum_\mu\dim L(\lambda)_\mu\,e^\mu$. The symbols $e^\mu$ belong to the [group algebra](../../../../../group-algebra.md) of the [weight lattice](../../../../../weight-lattice.md) and multiply by $e^\mu e^\nu=e^{\mu+\nu}$; they are formal symbols, not matrix exponentials.

Put $\rho=\frac12\sum_{\alpha\in R^+}\alpha$, the [half-sum of positive roots](../../../../../half-sum-of-positive-roots.md), and let $\ell(w)$ be the [Coxeter length](../../../../../coxeter-length.md) of $w$, the least number of simple reflections expressing it. Then $(-1)^{\ell(w)}=\det(w)$ in the real reflection representation. The [Weyl character formula](../../../../../weyl-character-formula.md) states

$$
\boxed{\operatorname{ch}L(\lambda)=\frac{\displaystyle\sum_{w\in W}(-1)^{\ell(w)}e^{w(\lambda+\rho)}}{\displaystyle\sum_{w\in W}(-1)^{\ell(w)}e^{w\rho}}.}
$$

By the [Weyl denominator formula](../../../../../weyl-denominator-formula.md), the denominator is $e^\rho\prod_{\alpha\in R^+}(1-e^{-\alpha})$, giving the equivalent expression

$$
\boxed{\operatorname{ch}L(\lambda)=\frac{\displaystyle\sum_{w\in W}\det(w)e^{w(\lambda+\rho)-\rho}}{\displaystyle\prod_{\alpha\in R^+}(1-e^{-\alpha})}.}
$$

The quotient can be interpreted in the fraction field of the formal group algebra; the theorem says it simplifies to the finite [formal character](../../../../../formal-character-of-a-weight-module.md) above. In particular the apparent denominator does not mean that the representation has infinitely many weights.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
