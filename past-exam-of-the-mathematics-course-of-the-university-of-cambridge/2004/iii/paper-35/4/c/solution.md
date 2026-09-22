<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $K$ denote the strike, $\tau=T-t$, and suppose $S>0$, $K>0$, $\tau>0$ and $\sigma>0$. Under the [Black-Scholes model](../../../../../../black-scholes-model.md) and the [risk-neutral measure](../../../../../../risk-neutral-measure.md), $\log S_T$ is normal with

$$
m=\log S+(r-\sigma^2/2)\tau,\qquad v=\sigma\sqrt\tau.
$$

Applying [risk-neutral valuation](../../../../../../risk-neutral-pricing.md) to the [European call option](../../../../../../european-call-option.md) payoff gives

$$
C=e^{-r\tau}\mathbb E_{\mathbb Q}(S_T-K)^+
=e^{-r\tau}\int_{\log K}^{\infty}(e^u-K)\frac{e^{-(u-m)^2/(2v^2)}}{v\sqrt{2\pi}}\,du.
$$

Use $\xi=\Phi((u-m)/v)$, whose differential is precisely the normal density times $du$. The threshold is $\xi_K=\Phi((\log K-m)/v)$, so

$$
\boxed{C=\int_0^1g(\xi)d\xi,\qquad
 g(\xi)=e^{-r\tau}\left(e^{m+v\Phi^{-1}(\xi)}-K\right)^+.}
$$

Equivalently, rescale the tail interval to obtain $g_{\mathrm{tail}}(\eta)=e^{-r\tau}(1-\xi_K)\{\exp[m+v\Phi^{-1}(\xi_K+(1-\xi_K)\eta)]-K\}$ on $0<\eta<1$.

For independent uniform inputs, the [Monte Carlo estimator](../../../../../../monte-carlo-estimator.md) is $\widehat C_N=N^{-1}\sum_{j=1}^Ng(U_j)$. It is unbiased, converges by the [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md), and has [variance](../../../../../../variance-split.md) $\operatorname{Var}(g(U))/N$. The payoff has finite second moment because the lognormal stock has finite moments. Its estimated standard error is the sample [standard deviation](../../../../../../standard-deviation.md) divided by $\sqrt N$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
