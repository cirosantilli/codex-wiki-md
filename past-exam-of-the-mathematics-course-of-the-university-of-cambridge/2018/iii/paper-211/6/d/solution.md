<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

With constant coefficients, $\lambda=(\mu-r)/\sigma$ is constant, so the [stochastic exponential](../../../../../../doleans-dade-exponential.md) $Z_t=e^{rt}Y_t$ is a true [martingale](../../../../../../martingale-split.md). Under its [equivalent martingale measure](../../../../../../risk-neutral-measure.md) $\mathbb Q$, the [stock](../../../../../../stock.md) follows the [Black-Scholes model](../../../../../../black-scholes-model.md) $dS_t=S_t(rdt+\sigma dW_t^{\mathbb Q})$. The Gaussian exponential [moment](../../../../../../moment.md) gives the value of the [power option](../../../../../../power-option.md)

$$
V_t=e^{-r(T-t)}\mathbb E_{\mathbb Q}[\sqrt{S_T}\mid\mathcal F_t]=\sqrt{S_t}\exp\!\left(-\left(\frac r2+\frac{\sigma^2}8\right)(T-t)\right).
$$

The [option delta](../../../../../../option-delta.md) is $\partial_sV=V/(2s)$, so the [replicating strategy](../../../../../../replicating-strategy.md) holds

$$
\boxed{\theta_t=\frac{V_t}{2S_t},\qquad\eta_t=\frac{V_t}{2B_t},\qquad V_0=\sqrt{S_0}\exp\!\left(-\left(\frac r2+\frac{\sigma^2}8\right)T\right).}
$$

Half the wealth value is in the [stock](../../../../../../stock.md) and half in the [bank account](../../../../../../bank-account.md), with continuous rebalancing. To check the [self-financing portfolio](../../../../../../self-financing-portfolio.md) property under the original measure, the [Itô formula](../../../../../../ito-s-lemma.md) gives $dV_t=\frac12(r+\mu)V_tdt+\frac12\sigma V_tdW_t=\theta_tdS_t+\eta_tdB_t$. Also $V_T=\sqrt{S_T}$ and $V_t>0$.

The payoff is unbounded, so the bounded-payoff restriction of part (c) is not invoked automatically; the [Black-Scholes model](../../../../../../black-scholes-model.md) has the necessary finite Gaussian [moments](../../../../../../moment.md), and the explicit strategy attains $V_0=\mathbb E[Y_T\sqrt{S_T}]$. The [supermartingale](../../../../../../supermartingale.md) bound from part (b) therefore proves its minimality. The cost is independent of the physical [drift](../../../../../../drift-coefficient.md) $\mu$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
