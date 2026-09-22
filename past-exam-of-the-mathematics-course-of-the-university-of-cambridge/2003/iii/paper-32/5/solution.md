<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use the physical dynamics of the [Black-Scholes model](../../../../../black-scholes-model.md), $dS_t/S_t=\mu dt+\sigma dW_t$, with bank rate $\rho$ and $\sigma>0$. Write $\lambda=(\mu-\rho)/\sigma$ for the [market price of risk](../../../../../market-price-of-risk.md). If $w_t$ is [portfolio wealth](../../../../../portfolio-wealth.md), $\pi_t$ the dollar amount in stock, and $c_t\geq0$ the [consumption](../../../../../consumption.md) rate, the budget dynamics are

$$
dw_t=[\rho w_t+\pi_t(\mu-\rho)-c_t]dt+\sigma\pi_t\,dW_t.
$$

Admissible controls are progressively measurable, locally integrable in the required drift and diffusion norms, and keep $w_t\geq0$. Such a solvency restriction excludes doubling-type strategies. In a complete Brownian market, the [investment-consumption problem](../../../../../investment-consumption-problem.md) is to maximize

$$
\mathbb E\!\left[\int_0^T e^{-\delta t}u(c_t)dt+e^{-\delta T}U(w_T)\right],
$$

where the [utility functions](../../../../../utility-function-split.md) are increasing and concave. A terminal-only problem omits the integral. Strict concavity gives uniqueness of optimal consumption and terminal wealth when an optimum exists.

The [state-price density](../../../../../state-price-density.md) is

$$
H_t=e^{-\rho t}\exp(-\lambda W_t-\lambda^2t/2).
$$

The [Itô formula](../../../../../ito-s-lemma.md) gives

$$
d(H_tw_t)+H_tc_tdt=H_t(\sigma\pi_t-\lambda w_t)dW_t.
$$

Thus $H_tw_t+\int_0^tH_sc_sds$ is a nonnegative [local martingale](../../../../../local-martingale.md), hence a [supermartingale](../../../../../supermartingale.md), yielding the [state-price budget constraint](../../../../../state-price-budget-constraint.md)

$$
\mathbb E\!\left[H_Tw_T+\int_0^TH_tc_tdt\right]\leq w_0.
$$

Conversely, a nonnegative consumption plan and terminal payoff $\xi$ satisfying budget equality and the necessary [integrability](../../../../../integrability.md) can be financed in the Brownian [complete market](../../../../../complete-market.md). Define

$$
w_t=H_t^{-1}\mathbb E\!\left[H_T\xi+\int_t^TH_sc_sds\,\middle|\,\mathcal F_t\right].
$$

The [Brownian martingale representation theorem](../../../../../brownian-martingale-representation-theorem.md) for the total future budget supplies a stochastic-integral coefficient; comparing it with $H_t(\sigma\pi_t-\lambda w_t)$ defines $\pi_t$. This reconstructs the wealth equation with $w_t\geq0$. Localization gives the representation for integrable positive budgets when an $L^2$ assumption is not available.

For smooth strictly concave utilities with the usual marginal-utility range, let $I_u=(u')^{-1}$ and $I_U=(U')^{-1}$ be the [inverse marginal utility](../../../../../inverse-marginal-utility.md) functions. The Lagrange-multiplier solution is

$$
\boxed{c_t^*=I_u(ye^{\delta t}H_t),\qquad\xi^*=I_U(ye^{\delta T}H_T),}
$$

where $y>0$ makes the budget an equality. This is a global argument, not merely formal differentiation: the [concave supporting-tangent inequality](../../../../../concave-supporting-tangent-inequality.md) gives

$$
e^{-\delta t}[u(c_t)-u(c_t^*)]\leq yH_t(c_t-c_t^*),
$$

with the analogous terminal inequality. Taking expectations, integrating, and applying the budget bound makes the difference in objectives nonpositive. Replication of the candidate budget proves attainability and optimality whenever these expectations are well-defined and finite. If the marginal-utility ranges or integrability conditions fail, existence must be established separately rather than inferred from the first-order equations.

A detailed example is [constant relative risk aversion utility](../../../../../constant-relative-risk-aversion-utility.md) $u(c)=c^{1-\gamma}/(1-\gamma)$ and $U(w)=\eta w^{1-\gamma}/(1-\gamma)$, with $\gamma>0$, $\gamma\ne1$, $\eta>0$, and $\delta\geq0$. Put

$$
k=\frac{\delta+(\gamma-1)(\rho+\lambda^2/(2\gamma))}{\gamma},\qquad b(\tau)=\int_0^\tau e^{-ks}ds+\eta^{1/\gamma}e^{-k\tau}.
$$

The optimal plans from the marginal-utility equations are $c_t^*=(ye^{\delta t}H_t)^{-1/\gamma}$ and $\xi^*=\eta^{1/\gamma}(ye^{\delta T}H_T)^{-1/\gamma}$. The [normal distribution](../../../../../normal-distribution.md) of $W_t$ gives, for $a=1-1/\gamma$,

$$
\mathbb EH_t^a=\exp[-a\rho t+\tfrac12a(a-1)\lambda^2t].
$$

The budget therefore becomes $y^{-1/\gamma}b(T)=w_0$, determining the multiplier explicitly. Independent Brownian increments in the conditional budget formula give $w_t^*=c_t^*b(T-t)$. The diffusion coefficient of $c_t^*$ is $(\lambda/\gamma)c_t^*$, so matching the wealth diffusion determines the dollar stock holding. Consequently the [finite-horizon power-utility investment and consumption](../../../../../finite-horizon-power-utility-investment-and-consumption.md) optimum is

$$
\boxed{c_t^*=\frac{w_t^*}{b(T-t)},\qquad\pi_t^*=\frac{\mu-\rho}{\gamma\sigma^2}w_t^*,\qquad w_T^*=\eta^{1/\gamma}c_T^*.}
$$

All candidate moments are finite on a finite horizon, since powers of a lognormal [state-price density](../../../../../state-price-density.md) have finite moments. The budget and tangent argument above therefore verify optimality in this example, including admissibility and positive wealth.

For another verification of the formulas, the [Hamilton-Jacobi-Bellman equation](../../../../../hamilton-jacobi-bellman-equation.md) for a value function with discount measured from the current time is

$$
0=V_t-\delta V+\sup_{c\geq0,\pi}\left\{\frac{c^{1-\gamma}}{1-\gamma}+(\rho w+\pi(\mu-\rho)-c)V_w+\tfrac12\sigma^2\pi^2V_{ww}\right\},\qquad V(w,T)=\frac{\eta w^{1-\gamma}}{1-\gamma}.
$$

Substitute $V(w,t)=b(T-t)^\gamma w^{1-\gamma}/(1-\gamma)$. The two concave maximizations give the displayed controls, and the remaining equation is $b'(\tau)=1-kb(\tau)$ with $b(0)=\eta^{1/\gamma}$, exactly solved by the formula above. Thus

$$
\boxed{V(w,t)=\frac{b(T-t)^\gamma w^{1-\gamma}}{1-\gamma}.}
$$

For $k=0$, interpret the integral as $\tau$, so $b(\tau)=\tau+\eta^{1/\gamma}$. Unlike the infinite-horizon [Merton consumption-investment problem](../../../../../merton-consumption-investment-problem.md), finite horizons do not require $k>0$. Consumption vanishes in the terminal-only formulation; then the integral term in $b$ is absent and the optimal stock fraction remains $(\mu-\rho)/(\gamma\sigma^2)$. Logarithmic utility is handled directly with inverse marginal utility $1/z$ and the same wealth-to-consumption formula at $\gamma=1$, with $k=\delta$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
