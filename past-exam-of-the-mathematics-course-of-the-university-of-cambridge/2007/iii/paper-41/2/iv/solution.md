<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For the [Cox-Ross-Rubinstein diffusion approximation](../../../../../../cox-ross-rubinstein-diffusion-approximation.md), fix calendar maturity $T$, take $h=T/n$, and choose $u=e^{\sigma\sqrt h}$, $d=e^{-\sigma\sqrt h}$, and the one-step bank factor $b=e^{\rho h}$. For sufficiently fine mesh, $d<b<u$. The [risk-neutral probability](../../../../../../risk-neutral-probability.md) expands as

$$
q_h=\frac{e^{\rho h}-e^{-\sigma\sqrt h}}{e^{\sigma\sqrt h}-e^{-\sigma\sqrt h}}=\frac12+\frac{\rho-\sigma^2/2}{2\sigma}\sqrt h+O(h^{3/2}).
$$

Each [stock](../../../../../../stock.md) log-increment is $\pm\sigma\sqrt h$. Its mean under $Q$ is $(\rho-\sigma^2/2)h+O(h^2)$ and its variance is $\sigma^2h+O(h^2)$. Independent increments, their vanishing maximum size, and the [Donsker invariance principle](../../../../../../donsker-s-theorem.md) for this triangular array give the path limit

$$
\boxed{\log S_t^{(n)}\ \Longrightarrow\ \log S_0+(\rho-\sigma^2/2)t+\sigma W_t^Q.}
$$

Exponentiation gives the [geometric Brownian motion](../../../../../../geometric-brownian-motion.md) of the [Black-Scholes model](../../../../../../black-scholes-model.md), and the bank account tends to $e^{\rho t}$.

The physical model is matched by taking $p_h=(e^{\mu h}-d)/(u-d)$. Its corresponding limit has log drift $\mu-\sigma^2/2$, so $dS_t=\mu S_tdt+\sigma S_tdW_t^P$. The likelihood ratios from part (ii) have the matching continuous-time limit. With $\lambda=(\mu-\rho)/\sigma$, a Taylor expansion of their two possible log-multipliers gives

$$
\log L_n=-\lambda W_T^{(n)}-\frac12\lambda^2T+o(1),\qquad W_T^{(n)}=\sum_{k=1}^n\varepsilon_k\sqrt h-\frac{\mu-\sigma^2/2}{\sigma}T,
$$

where $\varepsilon_k$ is $+1$ or $-1$. Thus the limiting [Radon-Nikodym derivative](../../../../../../radon-nikodym-derivative.md) is the [Girsanov theorem](../../../../../../girsanov-theorem.md) density $\exp(-\lambda W_T^P-\lambda^2T/2)$, turning the physical [stock](../../../../../../stock.md) drift into $\rho$.

The binomial [risk-neutral pricing](../../../../../../risk-neutral-pricing.md) formula converges to $e^{-\rho T}\mathbb E_Q[f(S_T)]$ for bounded continuous terminal payoffs by convergence in distribution. For ordinary call and put payoffs, uniform [stock](../../../../../../stock.md) second-moment bounds give the required [uniform integrability](../../../../../../uniform-integrability.md) and hence convergence despite unboundedness. Bounded payoffs with discontinuities only at events of zero limiting probability are handled by the same weak-convergence criterion. Corresponding continuous path functionals can be treated at the process level. Arbitrary discontinuous path claims do not follow from weak convergence without further conditions. In the smooth limiting model, the discrete hedging difference quotient becomes the [delta hedge](../../../../../../delta-hedge.md) $V_x$, and its value satisfies the [Black-Scholes equation](../../../../../../black-scholes-equation.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
