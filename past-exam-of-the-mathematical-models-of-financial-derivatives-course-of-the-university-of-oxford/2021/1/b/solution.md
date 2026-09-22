<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $\theta_t=(\mu-r)S_t/\sigma$. The [Girsanov theorem](../../../../girsanov-theorem.md) uses the density

$$
Z_T=\exp\left(-\int_0^T\theta_u\,dW_u-\frac12\int_0^T\theta_u^2\,du\right),\qquad
W_t^{\mathbb Q}=W_t+\int_0^t\theta_u\,du.
$$

For these nonexplosive [linear stochastic differential equations](../../../../linear-stochastic-differential-equation.md), the [linear drift change of measure](../../../../linear-drift-change-of-measure.md) ensures that $Z$ is a true [martingale](../../../../martingale-split.md) on each finite horizon. This matters: a stochastic exponential being a local [martingale](../../../../martingale-split.md) alone would not prove that its terminal expectation is one. Its strict positivity gives an equivalent [risk-neutral measure](../../../../risk-neutral-measure.md) $\mathbb Q$, under which

$$
\boxed{dS_t=rS_t\,dt+\sigma\,dW_t^{\mathbb Q}.}
$$

The discounted asset is then a [martingale](../../../../martingale-split.md). The [Feynman-Kac formula](../../../../feynman-kac-formula.md), equivalently [risk-neutral valuation](../../../../risk-neutral-pricing.md) of the replicable claim, gives

$$
\boxed{V(t,s)=e^{-r\tau}\mathbb E_{\mathbb Q}[F(S_T)\mid S_t=s].}
$$

Here the payoff must meet the usual integrability and replication assumptions; the bounded digital payoff below does.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../split.md)
5. [Mathematical models of financial derivatives course of the University of Oxford](../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
