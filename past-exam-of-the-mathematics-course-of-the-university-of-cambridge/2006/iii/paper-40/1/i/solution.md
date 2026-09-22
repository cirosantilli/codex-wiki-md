<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take $S_t$ to be the ex-dividend [stock](../../../../../../stock.md) price: the date-$t$ output has already been paid when trading occurs. Receiving $\theta_td_t$ units of fruit and selling $\theta_t-\theta_{t+1}$ shares gives the [discrete dividend budget equation](../../../../../../discrete-dividend-budget-equation.md)

$$
\boxed{C_t=\theta_td_t+(\theta_t-\theta_{t+1})S_t,\qquad C_t+S_t\theta_{t+1}=(S_t+d_t)\theta_t.}
$$

The entering holding $\theta_t$ is chosen with date-$(t-1)$ information, while $C_t$ and the next holding $\theta_{t+1}$ may use date-$t$ information. The output is the consumption good and price numéraire; its stochastic law is exogenous to the individual's price-taking choice.

For the interior differentiable case, attach an adapted [Lagrange multiplier](../../../../../../lagrange-multiplier.md) $\Lambda_t$ to each [budget constraint](../../../../../../budget-constraint.md). On a finite horizon, with the terminal holding fixed or its continuation value included, the [optimization Lagrangian](../../../../../../optimization-lagrangian.md) is

$$
\mathcal L=\mathbb E\sum_t\left\{\beta^tU(C_t)+\Lambda_t\big[(S_t+d_t)\theta_t-S_t\theta_{t+1}-C_t\big]\right\}.
$$

An adapted variation in $C_t$ gives $\Lambda_t=\beta^tU'(C_t)$. An arbitrary date-$t$ measurable variation in $\theta_{t+1}$ affects two adjacent terms. Its coefficient must have zero conditional mean, so

$$
\boxed{\Lambda_tS_t=\mathbb E[\Lambda_{t+1}(S_{t+1}+d_{t+1})\mid\mathcal F_t],\qquad\Lambda_t=\beta^tU'(C_t).}
$$

These are the Euler equations of [marginal utility pricing in a dividend economy](../../../../../../marginal-utility-pricing-in-a-dividend-economy.md). If the [utility function](../../../../../../utility-function-split.md) is merely concave, a supporting slope replaces $U'$; binding consumption or trading restrictions give the corresponding inequalities rather than unconstrained equalities.

With known initial information and $\Lambda_0>0$, normalize $\zeta_t=\Lambda_t/\Lambda_0$. This is a [state-price density](../../../../../../state-price-density.md) for the traded asset. In particular,

$$
S_t=\mathbb E_t\left[\frac{\zeta_{t+1}}{\zeta_t}(S_{t+1}+d_{t+1})\right],\qquad
\frac{\zeta_{t+1}}{\zeta_t}=\beta\frac{U'(C_{t+1})}{U'(C_t)}.
$$

The ratio is the stochastic discount factor: payment in a state with greater marginal utility has a higher marginal value. For a priced contingent payoff $H$ at $t+1$, its price is $\mathbb E_t[(\zeta_{t+1}/\zeta_t)H]$; pricing arbitrary claims uniquely also requires [market completeness](../../../../../../complete-market.md). The deflated cumulative gains $\zeta_tS_t+\sum_{s=1}^t\zeta_sd_s$ form a [martingale](../../../../../../martingale-split.md) whenever the displayed terms are integrable.

Iterating the Euler equation gives

$$
\zeta_tS_t=\mathbb E_t\left[\sum_{s=t+1}^N\zeta_sd_s+\zeta_NS_N\right].
$$

Under the [dividend-price transversality condition](../../../../../../dividend-price-transversality-condition.md) and the needed integrability, this becomes the fundamental price

$$
\boxed{S_t=\frac1{\zeta_t}\mathbb E_t\sum_{s>t}\zeta_sd_s.}
$$

Thus an infinite-horizon price is not automatically just a dividend sum: its terminal term must vanish. Telescoping the individual [budget constraints](../../../../../../budget-constraint.md) similarly gives

$$
\mathbb E\sum_{t=0}^N\zeta_tC_t
=\zeta_0\theta_0(S_0+d_0)-\mathbb E[\zeta_NS_N\theta_{N+1}].
$$

A no-Ponzi lower restriction on this final term gives the consumption budget inequality; its vanishing gives equality. Together with the supporting-line inequality for a [concave](../../../../../../concave-function.md) [utility function](../../../../../../utility-function-split.md), the Euler equations and these terminal conditions supply the usual sufficiency argument for an admissible candidate. In an [incomplete market](../../../../../../incomplete-market.md), each optimal agent's marginal utility can supply a different [state-price density](../../../../../../state-price-density.md) pricing the same traded tree.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
