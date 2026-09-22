# Noise sensitivity of a quadrature rule

↑ **Parent:** [Quadrature rule](quadrature-rule.md)

If the observed samples are $y_i=f(x_i)+\varepsilon_i$, the resulting [quadrature rule](quadrature-rule.md) changes by $\Delta Q=\sum_iw_i\varepsilon_i$. Bounded sample perturbations $|\varepsilon_i|\leq\delta$ therefore satisfy

$$
|\Delta Q|\leq\delta\sum_i|w_i|.
$$

For ordinary [numerical integration](numerical-integration.md) with nonnegative [quadrature weights](quadrature-weight.md) exact on [constant functions](constant-function.md), the bound is $(b-a)\delta$, independent of panel refinement. A common bias $\varepsilon_i=\delta$ attains it: the [quadrature error](quadrature-error.md) due to the [function](function-split.md) approximation may vanish while this sample error persists. Interpolating a fixed data set onto a finer grid likewise does not create new observations or remove its uncertainty.

With new samples whose errors are [independent random variables](independent-random-variables.md) of zero [expectation](expected-value.md) and common [variance](variance-split.md) $\sigma^2$, a different model gives

$$
\operatorname{Var}(\Delta Q)=\sigma^2\sum_iw_i^2.
$$

For equal panels this is $\sigma^2(b-a)^2/n$ for the [composite midpoint quadrature rule](composite-midpoint-quadrature-rule.md) and $\sigma^2h^2(n-1/2)$ for the [composite trapezoidal rule](composite-trapezoidal-rule.md). These [variance](variance-split.md) reductions require the stated independence and unbiasedness assumptions; a common bias or correlated sample errors need not shrink. The two displayed perturbation formulas follow directly from the [triangle inequality](triangle-inequality.md) and the [variance additivity for independent random variables](variance-additivity-for-independent-random-variables.md), respectively.

## ↑ Ancestors (7)

1. [Quadrature rule](quadrature-rule.md)
2. [Numerical integration](numerical-integration.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Composite midpoint quadrature rule](composite-midpoint-quadrature-rule.md)
- [Composite trapezoidal rule](composite-trapezoidal-rule.md)
- [Quadrature weight](quadrature-weight.md)
