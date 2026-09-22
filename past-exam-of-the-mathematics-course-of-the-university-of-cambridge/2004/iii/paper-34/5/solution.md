<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Write $T=t_0$, and specify the physical [Black-Scholes model](../../../../../black-scholes-model.md) as $dS_t/S_t=\mu\,dt+\sigma\,dW_t$, with constant $\sigma>0$ and bank rate $\rho$. The physical drift $\mu$ is needed for an [expected utility](../../../../../expected-utility.md) calculation; a pricing model specified only under a [risk-neutral measure](../../../../../risk-neutral-measure.md) does not determine the investor's preferences over risky positions. Put

$$
\vartheta=\frac{\mu-\rho}{\sigma},\quad Z_t=e^{-\vartheta W_t-\vartheta^2t/2},\quad \xi_t=e^{-\rho t}Z_t.
$$

Here $\vartheta$ is the [market price of risk](../../../../../market-price-of-risk.md), $Z_T$ is the density of the [risk-neutral measure](../../../../../risk-neutral-measure.md) $Q$, and $\xi$ is the [state-price density](../../../../../state-price-density.md). The [Girsanov theorem](../../../../../girsanov-theorem.md) makes $W_t^Q=W_t+\vartheta t$ a [Brownian motion](../../../../../brownian-motion-split.md) under $Q$.

For a dollar holding $\pi_t$ in the [stock](../../../../../stock.md) and [consumption](../../../../../consumption.md) rate $c_t$, the [portfolio wealth](../../../../../portfolio-wealth.md) equation is

$$
dV_t=\{\rho V_t+(\mu-\rho)\pi_t-c_t\}dt+\sigma\pi_t\,dW_t,\qquad V_0=w_0.
$$

Since $d\xi_t=-\rho\xi_tdt-\vartheta\xi_tdW_t$, integration by parts gives the useful [deflated wealth equation with consumption](../../../../../deflated-wealth-equation-with-consumption.md)

$$
d(\xi_tV_t)+\xi_tc_tdt=\xi_t(\sigma\pi_t-\vartheta V_t)\,dW_t.
$$

For strategies with a true deflated gain [martingale](../../../../../martingale-split.md), terminal wealth $X=V_T$ and [consumption](../../../../../consumption.md) obey the [state-price budget constraint](../../../../../state-price-budget-constraint.md)

$$
\mathbb E_P\left[\xi_TX+\int_0^T\xi_tc_tdt\right]=w_0.
$$

For nonnegative wealth and consumption, the admissibility condition can instead give a budget inequality; increasing utilities use the full budget at an optimum. Conversely, suitable integrable payoff and consumption plans with this budget are financeable in the Brownian [complete market](../../../../../complete-market.md). To construct the strategy, set

$$
M_t=\mathbb E_P\left[\xi_TX+\int_0^T\xi_sc_sds\,\middle|\,\mathcal F_t\right],\qquad
V_t=\xi_t^{-1}\left(M_t-\int_0^t\xi_sc_sds\right).
$$

By the [Brownian martingale representation theorem](../../../../../brownian-martingale-representation-theorem.md), write $dM_t=H_t\,dW_t$. The required dollar stock holding is $\pi_t=(H_t/\xi_t+\vartheta V_t)/\sigma$; substitution in the deflated gain equation verifies financing. Remaining wealth goes into the [bank account](../../../../../bank-account.md). For square-integrable data the representation holds directly, and localization handles the customary integrable admissible data.

First take no [consumption](../../../../../consumption.md). For an increasing strictly [concave](../../../../../concave-function.md) differentiable [utility function](../../../../../utility-function-split.md) whose marginal derivative can be inverted, let $I_u=(u')^{-1}$. Choose $\lambda>0$ so that

$$
\boxed{X^*=I_u(\lambda\xi_T),\qquad\mathbb E_P[\xi_TX^*]=w_0.}
$$

This candidate is not merely a first-order guess. The [concave supporting-tangent inequality](../../../../../concave-supporting-tangent-inequality.md) gives, pointwise,

$$
u(X)\leq u(X^*)+u'(X^*)(X-X^*)=u(X^*)+\lambda\xi_T(X-X^*).
$$

Taking [expectations](../../../../../expected-value.md) and using the budget proves $\mathbb E u(X)\leq\mathbb E u(X^*)$ for every feasible competitor. Finance the optimizer by its [risk-neutral pricing](../../../../../risk-neutral-pricing.md) value $V_t=e^{-\rho(T-t)}\mathbb E_Q[X^*\mid\mathcal F_t]$, using the preceding representation to find the holdings.

For a merely [concave](../../../../../concave-function.md) differentiable [utility function](../../../../../utility-function-split.md), the general formulation is to select $X^*(\omega)$ from the maximizers of $u(x)-\lambda\xi_T(\omega)x$ over its wealth domain, and choose the multiplier to satisfy the budget. If increasing utility is not assumed, the equality-budget multiplier may have either sign; the positive-multiplier inverse formula above is for increasing utility. Flat portions allow multiple maximizers; boundaries require one-sided inequalities rather than equality of marginal derivatives. Existence of a multiplier, integrability and an admissible maximizer must be checked. Concavity alone does not guarantee a well-posed problem: with unrestricted dollar positions, linear utility $u(x)=x$ and $\mu>\rho$ permits unbounded expected terminal wealth. The explicit utilities below satisfy the needed conditions in their stated domains.

For [exponential utility](../../../../../constant-absolute-risk-aversion-utility.md) $u(x)=(1-e^{-ax})/a$ on $\mathbb R$, $u'(x)=e^{-ax}$ and $I_u(y)=-\log y/a$. Therefore

$$
X^*=-\frac1a\log(\lambda\xi_T)
=-\frac{\log\lambda}{a}+\frac{\rho T}{a}+\frac{\vartheta W_T}{a}+\frac{\vartheta^2T}{2a}.
$$

The budget is equivalently $\mathbb E_QX^*=w_0e^{\rho T}$, since $\xi_T=e^{-\rho T}dQ/dP$. Under $Q$, $\mathbb E_QW_T=-\vartheta T$, giving $\log\lambda=\rho T-\vartheta^2T/2-aw_0e^{\rho T}$. Hence

$$
X^*=w_0e^{\rho T}+\frac{\vartheta}{a}W_T^Q,\qquad
V_t=e^{-\rho(T-t)}\left(w_0e^{\rho T}+\frac{\vartheta}{a}W_t^Q\right).
$$

Matching the Brownian coefficient of $dV$ with $\sigma\pi_t$ gives the [finite-horizon exponential-utility portfolio](../../../../../finite-horizon-exponential-utility-portfolio.md)

$$
\boxed{\pi_t^*=\frac{\mu-\rho}{a\sigma^2}e^{-\rho(T-t)}.}
$$

Hold $\pi_t^*/S_t$ shares and invest $V_t-\pi_t^*$ in the [bank account](../../../../../bank-account.md). This is a dollar amount, not a fixed wealth fraction. The Gaussian exponential formula also gives the optimal [expected utility](../../../../../expected-utility.md)

$$
\boxed{\mathbb E_Pu(X^*)=\frac{1-\exp(-aw_0e^{\rho T}-\vartheta^2T/2)}{a}.}
$$

This calculation uses unrestricted wealth and an admissibility class permitting the displayed Gaussian terminal wealth, with integrable deflated gains and the relevant exponential moment. A nonnegative-wealth constraint would change the optimizer; no such constraint is imposed on this exponential-utility example.

For both terminal and running [utility function](../../../../../utility-function-split.md), choose $X$ and a nonnegative adapted [consumption](../../../../../consumption.md) rate $c$ to maximize $\mathbb E_P[u(X)+\int_0^Tv(c_t)dt]$ subject to the combined budget. Pointwise maximization of $u(x)-\lambda\xi_Tx$ and $v(c)-\lambda\xi_tc$ gives, for interior strictly [concave](../../../../../concave-function.md) cases,

$$
X^*=I_u(\lambda\xi_T),\qquad c_t^*=I_v(\lambda\xi_t),\qquad
\mathbb E_P\left[\xi_TX^*+\int_0^T\xi_tc_t^*dt\right]=w_0.
$$

Apply the [concave supporting-tangent inequality](../../../../../concave-supporting-tangent-inequality.md) to $u$ and to $v$ at every time, then integrate and take [expectations](../../../../../expected-value.md). The difference in objectives is at most $\lambda$ times the difference in budget expenditures, which is nonpositive. This proves optimality, not just the marginal conditions. The financing value is

$$
V_t=\xi_t^{-1}\mathbb E_P\left[\xi_TX^*+\int_t^T\xi_sc_s^*ds\,\middle|\,\mathcal F_t\right].
$$

The question's consumption rate $R_t$ is denoted $c_t$ here to keep it distinct from interest-rate notation.

For [logarithmic utility](../../../../../logarithmic-utility.md) with $u(x)=a\log x$, $v(x)=b\log x$, assume $a,b,w_0>0$ and positive wealth and [consumption](../../../../../consumption.md). The marginal conditions and budget give

$$
\lambda=\frac{a+bT}{w_0},\qquad X^*=\frac{a}{\lambda\xi_T},\qquad c_t^*=\frac{b}{\lambda\xi_t}.
$$

Each state-price-weighted payment is deterministic, so conditional valuation immediately gives $V_t=[a+b(T-t)]/(\lambda\xi_t)$. Put $A_t=a+b(T-t)$. Since the [Itô formula](../../../../../ito-s-lemma.md) gives $d(1/\xi_t)=(1/\xi_t)[(\rho+\vartheta^2)dt+\vartheta dW_t]$, this value satisfies

$$
dV_t=V_t\left(\rho+\vartheta^2-\frac{b}{A_t}\right)dt+\vartheta V_t\,dW_t.
$$

Comparison with the wealth equation verifies the complete [finite-horizon logarithmic investment and consumption](../../../../../finite-horizon-logarithmic-investment-and-consumption.md) strategy:

$$
\boxed{V_t=\frac{A_t}{\lambda\xi_t},\qquad R_t^*=c_t^*=\frac{bV_t}{A_t},\qquad\pi_t^*=\frac{\mu-\rho}{\sigma^2}V_t.}
$$

Thus the optimal share holding is $\pi_t^*/S_t$, and the remaining value $V_t-\pi_t^*$ is in the [bank account](../../../../../bank-account.md); borrowing or shorting is allowed if that value or the stock holding is negative. Terminal wealth is positive and consumption is positive throughout. Finally $\mathbb E\log\xi_t=-(\rho+\vartheta^2/2)t$, so the optimal objective, if desired explicitly, is

$$
\boxed{a\log\frac{aw_0}{a+bT}+bT\log\frac{bw_0}{a+bT}+\left(\rho+\frac{\vartheta^2}{2}\right)\left(aT+\frac{bT^2}{2}\right).}
$$

Finite-horizon lognormal moments ensure the budget and expected utilities are finite, completing the feasibility and optimality checks.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
