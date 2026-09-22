<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use $\theta_t$ for the dollar amount invested in the [stock](../../../../../stock.md); the number of shares is $\theta_t/S_t$. The [bank account](../../../../../bank-account.md) contains $w_t-\theta_t$ dollars. With no intermediate [consumption](../../../../../consumption.md), the [self-financing portfolio](../../../../../self-financing-portfolio.md) equation is

$$
\boxed{dw_t=r_t(w_t-\theta_t)dt+\theta_t\frac{dS_t}{S_t}
=[r_tw_t+\theta_t(\mu_t-r_t)]dt+\theta_t\sigma_tdW_t.}
$$

If instead $\theta$ denotes share holdings, replace each dollar $\theta_t$ here by $S_t\theta_t$. The equation says that trading only reallocates existing [portfolio wealth](../../../../../portfolio-wealth.md); gains come from cash interest and stock returns.

For the standard unconstrained complete-diffusion formulation, assume the completed [natural Brownian filtration](../../../../../natural-brownian-filtration.md), initial wealth $w_0>0$, and nonnegative admissible wealth. Define the [market price of risk](../../../../../market-price-of-risk.md) $\kappa_t=(\mu_t-r_t)/\sigma_t$. The boundedness assumptions make $\kappa$ bounded. The [state-price density](../../../../../state-price-density.md) normalized at zero is

$$
\boxed{\zeta_t=\exp\left(-\int_0^t r_sds-\int_0^t\kappa_sdW_s-\frac12\int_0^t\kappa_s^2ds\right),\qquad d\zeta_t=-\zeta_t(r_tdt+\kappa_tdW_t).}
$$

Its money-market-adjusted process $Z_t=e^{\int_0^t r_sds}\zeta_t$ is a true [martingale](../../../../../martingale-split.md) by the [Novikov condition](../../../../../novikov-s-condition.md). Under $d\mathbb Q=Z_Td\mathbb P$, the [Girsanov theorem](../../../../../girsanov-theorem.md) gives $W_t^{\mathbb Q}=W_t+\int_0^t\kappa_sds$ as a [Brownian motion](../../../../../brownian-motion-split.md), and the discounted stock has zero drift.

The [Itô product rule](../../../../../ito-product-rule.md) applied to the wealth equation gives

$$
d(\zeta_tw_t)=\zeta_t(\sigma_t\theta_t-\kappa_tw_t)dW_t.
$$

For nonnegative admissible wealth this is a [nonnegative local martingale](../../../../../nonnegative-local-martingale.md), hence a [supermartingale](../../../../../supermartingale.md). Therefore every affordable terminal payoff $X=w_T$ satisfies the [state-price budget constraint](../../../../../state-price-budget-constraint.md) $\mathbb E[\zeta_TX]\leq w_0$. Nonzero volatility and the [Brownian martingale representation theorem](../../../../../brownian-martingale-representation-theorem.md) allow replication of nonnegative claims with finite state-price cost.

For a differentiable strictly [concave](../../../../../concave-function.md) [utility function](../../../../../utility-function-split.md) with the usual conditions ensuring an interior integrable optimizer, put $I=(U')^{-1}$, the [inverse marginal utility](../../../../../inverse-marginal-utility.md). Pointwise maximization of $U(x)-y\zeta_Tx$ gives

$$
\boxed{w_T^*=I(y\zeta_T),\qquad \mathbb E[\zeta_TI(y\zeta_T)]=w_0.}
$$

The second equation determines the positive constant $y$. To prove optimality, use the [concave supporting-tangent inequality](../../../../../concave-supporting-tangent-inequality.md):

$$
U(X)-U(w_T^*)\leq U'(w_T^*)(X-w_T^*)=y\zeta_T(X-w_T^*).
$$

Taking expectations and using the budget bound proves that the candidate dominates every admissible affordable payoff, whenever the utility expectations are well defined. This is the [complete-market terminal utility optimizer](../../../../../complete-market-terminal-utility-optimizer.md).

The actual wealth and dollar [portfolio](../../../../../investment-portfolio.md) are as explicit as general adapted coefficients permit. Let

$$
N_t=\mathbb E[\zeta_TI(y\zeta_T)\mid\mathcal F_t],\qquad dN_t=h_tdW_t.
$$

The [Brownian martingale representation theorem](../../../../../brownian-martingale-representation-theorem.md), with localization if only $L^1$ integrability is initially known, gives $h$. The [dollar portfolio from a deflated wealth martingale](../../../../../dollar-portfolio-from-a-deflated-wealth-martingale.md) is

$$
\boxed{w_t^*=\frac{N_t}{\zeta_t},\qquad
\theta_t^*=\frac{h_t/\zeta_t+\kappa_tw_t^*}{\sigma_t}.}
$$

The bank holds $w_t^*-\theta_t^*$ dollars. Equivalently, with $B_t=e^{\int_0^t r_sds}$, $w_t^*=B_t\mathbb E^{\mathbb Q}[w_T^*/B_T\mid\mathcal F_t]$. These formulas need no unjustified differentiability of a value function with random coefficients.

The printed assumption that $U$ is only increasing and concave does not guarantee that the interior formula exists, or even that the optimal value is finite. In general replace the inverse formula by an affordable selection

$$
X^*(\omega)\in\operatorname*{arg\,max}_{x\in\mathcal D}\{U(x)-y\zeta_T(\omega)x\},
$$

where $\mathcal D$ is the wealth domain; boundary choices or supporting slopes handle nondifferentiability. Existence, finite cost and replication still have to hold. A concrete obstruction is the [unbounded linear terminal-wealth utility](../../../../../unbounded-linear-terminal-wealth-utility.md): take $U(x)=x$, $r=0$, $\mu=\sigma=1$, and the Brownian filtration. Then $\zeta_T=e^{-W_T-T/2}$. For $A_n=\{\zeta_T<1/n\}$, the bounded nonnegative claim

$$
X_n=\frac{w_0\mathbf1_{A_n}}{\mathbb E[\zeta_T\mathbf1_{A_n}]}
$$

is replicable, costs $w_0$, and has $\mathbb EX_n>nw_0$. Thus there is no finite optimal expected utility under the literal utility hypotheses alone. Also, bounded coefficients do not ensure [market completeness](../../../../../complete-market.md) in an arbitrarily enlarged filtration containing untraded randomness; the full replication formula uses the Brownian market information assumption stated above.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
