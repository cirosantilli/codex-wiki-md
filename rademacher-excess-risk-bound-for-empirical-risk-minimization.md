# Rademacher excess-risk bound for empirical risk minimization

↑ **Parent:** [Rademacher complexity](rademacher-complexity.md)

For a zero-one-valued [loss class](loss-class.md) $\mathcal F$, the excess [misclassification risk](misclassification-risk.md) of an [empirical risk minimizer](empirical-risk-minimization.md) $\widehat h$ over a population minimizer $h^*$ satisfies

$$
R(\widehat h)-R(h^*)
\leq2\mathcal R_n(\mathcal F)
+\sqrt{\frac{2\log(2/\delta)}n}
$$

with [probability](probability-theory-split.md) at least $1-\delta$. The proof combines [Rademacher symmetrization](rademacher-symmetrization-inequality.md) with the [Bounded differences inequality](mcdiarmid-s-inequality.md) for the supremum of the empirical excess-loss process.

The observable version is

$$
R(\widehat h)-R(h^*)
\leq2\widehat{\mathcal R}(\mathcal F(Z_{1:n}))
+2\sqrt{\frac{2\log(3/\delta)}n}.
$$

It follows by another application of the [Bounded differences inequality](mcdiarmid-s-inequality.md) to the [Empirical Rademacher complexity](empirical-rademacher-complexity.md).

## ↑ Ancestors (6)

1. [Rademacher complexity](rademacher-complexity.md)
2. [Statistical learning theory](statistical-learning-theory.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
