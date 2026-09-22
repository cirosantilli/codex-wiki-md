# Bounded-coefficient asset deflator

↑ **Parent:** [Martingale deflator](martingale-deflator.md)

For asset dynamics $dS=\operatorname{diag}(S)(\mu\,dt+\sigma\,dW)$, let $\lambda=\sigma^{-1}\mu$ and $Z=\mathcal E(-\int\lambda^T\,dW)$. The [Itô product rule](ito-product-rule.md) cancels the drift of each $ZS^i$, leaving the displayed [stochastic integral](stochastic-integral.md). When $\mu$ is bounded and $\sigma\sigma^T\geq\varepsilon I$, $\lambda$ is bounded and the [Novikov condition](novikov-s-condition.md) makes $Z$ a true [martingale](martingale-split.md) on every finite horizon. If $\sigma$ is also bounded, each $ZS^i/S_0^i$ satisfies the [Novikov condition](novikov-s-condition.md) as a [stochastic exponential](doleans-dade-exponential.md) with bounded integrand $\sigma_i-\lambda$, so it too is a true [martingale](martingale-split.md).

## ↑ Ancestors (7)

1. [Martingale deflator](martingale-deflator.md)
2. [Risk-neutral measure](risk-neutral-measure.md)
3. [Mathematical finance](mathematical-finance-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-42/4/solution.md)
