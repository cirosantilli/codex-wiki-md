# Debiased-Lasso remainder bound

↑ **Parent:** [Debiased Lasso](debiased-lasso.md)

Let $\widehat\Sigma=X^TX/n$ and use [Nodewise Lasso](nodewise-lasso.md) with $\lambda_j>0$ and nonzero design columns. Form $c_j$ with entry $j$ equal to one and other entries $-\widehat\gamma^{(j)}$, and put row $j$ of $\widehat\Theta$ equal to $c_j^T/\widehat\tau_j^2$. The [nodewise-Lasso residual identity](nodewise-lasso-residual-identity.md) and the [Karush-Kuhn-Tucker conditions](karush-kuhn-tucker-conditions.md) show that the diagonal of $\widehat\Theta\widehat\Sigma$ equals one and its row-$j$ off-diagonal entries have magnitude at most $\lambda_j/\widehat\tau_j^2$. For the [Debiased Lasso](debiased-lasso.md),

$$
\sqrt n(\widehat b-\beta^0)=\widehat\Theta X^T\varepsilon/\sqrt n+\Delta,\qquad \Delta=\sqrt n(\widehat\Theta\widehat\Sigma-I)(\beta^0-\widehat\beta).
$$

The displayed bound follows row by row from [Holder inequality](holder-inequality.md). If the noise is conditionally [multivariate normal](multivariate-normal-distribution.md) with [covariance](covariance.md) $\sigma^2I$, and the nodewise fits and tuning parameters depend only on $X$, the first term is conditionally normal with [covariance](covariance.md) $\sigma^2\widehat\Theta\widehat\Sigma\widehat\Theta^T$.

## ↑ Ancestors (6)

1. [Debiased Lasso](debiased-lasso.md)
2. [Lasso](lasso.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Gaussian identity design for debiased Lasso](gaussian-identity-design-for-debiased-lasso.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-205/6/solution.md)
