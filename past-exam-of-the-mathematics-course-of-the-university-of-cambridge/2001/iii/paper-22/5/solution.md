<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

**Expected utility of terminal wealth.** Let initial wealth be $x_0>0$, maturity $T=t_0$, and stock-dollar investment $\pi_t$. A [self-financing strategy](../../../../../self-financing-portfolio.md) in the [Black-Scholes model](../../../../../black-scholes-model.md) has wealth

$$
dX_t=[\rho X_t+(\alpha-\rho)\pi_t]dt+\sigma\pi_t\,dW_t.
$$

Choose admissible strategies with nonnegative wealth, and an increasing strictly concave differentiable [utility function](../../../../../utility-function-split.md) $U$ satisfying the [Inada conditions](../../../../../inada-conditions.md). Assume the required [expectations](../../../../../expected-value.md) are finite and the optimization is well posed; the resulting budget equation below must have a solution. Write $\lambda=(\alpha-\rho)/\sigma$ and

$$
H_T=e^{-\rho T}\exp(-\lambda W_T-\lambda^2T/2).
$$

This [state-price density](../../../../../state-price-density.md) is the discounted density of the unique [equivalent martingale measure](../../../../../risk-neutral-measure.md). Nonnegative discounted wealth is a [supermartingale](../../../../../supermartingale.md) under that measure, so every admissible terminal wealth $Y$ obeys the [state-price budget constraint](../../../../../state-price-budget-constraint.md) $\mathbb E[H_TY]\le x_0$.

Conversely a nonnegative terminal claim with finite such cost is financed by its conditional [martingale](../../../../../martingale-split.md) price, which remains nonnegative; Brownian [Martingale representation theorem](../../../../../martingale-representation-theorem.md) constructs its holdings. Thus [market completeness](../../../../../complete-market.md) turns dynamic optimization into a terminal-payoff problem. Let $I=(U')^{-1}$ be the [inverse marginal utility](../../../../../inverse-marginal-utility.md), and choose $y>0$ from $\mathbb E[H_T I(yH_T)]=x_0$. Then the [complete-market terminal utility optimizer](../../../../../complete-market-terminal-utility-optimizer.md) is

$$
\boxed{Y^*=I(yH_T).}
$$

For any feasible $Y$, concavity gives the pointwise tangent inequality

$$
U(Y)\le U(Y^*)+U'(Y^*)(Y-Y^*)
=U(Y^*)+yH_T(Y-Y^*).
$$

Taking [expectations](../../../../../expected-value.md) and using the budget proves optimality; strict concavity gives uniqueness up to null events. The optimal wealth process is

$$
X_t^*=e^{-\rho(T-t)}\mathbb E_Q[Y^*\mid\mathcal F_t]
=H_t^{-1}\mathbb E_P[H_TY^*\mid\mathcal F_t].
$$

If its discounted [martingale](../../../../../martingale-split.md) has representation $d(e^{-\rho t}X_t^*)=\zeta_t dW_t^Q$, hold $\delta_t=e^{\rho t}\zeta_t/(\sigma S_t)$ [stock](../../../../../stock.md) units and invest the remainder in the [bank account](../../../../../bank-account.md). This derives the strategy, not only the terminal first-order condition.

The equivalent dynamic approach is the [Bellman equation for terminal-wealth utility](../../../../../bellman-equation-for-terminal-wealth-utility.md). For a smooth concave value $v(t,x)$, dynamic programming and [Itô formula](../../../../../ito-s-lemma.md) give

$$
v_t+\rho xv_x+\sup_\pi\left[(\alpha-\rho)\pi v_x+\frac12\sigma^2\pi^2v_{xx}\right]=0,
\qquad v(T,x)=U(x).
$$

For $v_{xx}<0$, maximizing the concave quadratic gives $\pi^*=-(\alpha-\rho)v_x/(\sigma^2v_{xx})$. For an arbitrary admissible control the Itô drift of $v(t,X_t)$ is nonpositive; localization and integrability therefore bound its expected terminal utility by $v(0,x_0)$. The maximizing control makes the drift zero, giving equality when the verification [expectations](../../../../../expected-value.md) are valid.

For [CRRA utility](../../../../../constant-relative-risk-aversion-utility.md) $U(x)=x^{1-\gamma}/(1-\gamma)$, $\gamma>0$, $\gamma\ne1$, substitution gives

$$
v(t,x)=\frac{x^{1-\gamma}}{1-\gamma}
\exp\!\left((1-\gamma)\left[\rho+\frac{\lambda^2}{2\gamma}\right](T-t)\right),
\qquad\boxed{\frac{\pi_t^*}{X_t^*}=\frac{\alpha-\rho}{\gamma\sigma^2}.}
$$

The optimal [stock](../../../../../stock.md) fraction is constant. Its geometric wealth dynamics stay positive, so it is feasible. For [logarithmic utility](../../../../../logarithmic-utility.md) the fraction is $(\alpha-\rho)/\sigma^2$ and $v(t,x)=\log x+(\rho+\lambda^2/2)(T-t)$. [Risk aversion](../../../../../risk-aversion.md) controls the risky exposure, while the market price of risk controls its reward.

**Pricing claims depending on the path.** For a [path-dependent contingent claim](../../../../../path-dependent-contingent-claim.md) $C=F((S_u)_{0\le u\le T})$, the [risk-neutral pricing](../../../../../risk-neutral-pricing.md) process is

$$
V_t=e^{-\rho(T-t)}\mathbb E_Q[C\mid\mathcal F_t].
$$

For square-integrable discounted $C$, the Brownian [Martingale representation theorem](../../../../../martingale-representation-theorem.md) gives $d(e^{-\rho t}V_t)=\varphi_t dW_t^Q$. Since $d(e^{-\rho t}S_t)=\sigma e^{-\rho t}S_t dW_t^Q$, the replicating holding is $\delta_t=\varphi_t/(\sigma e^{-\rho t}S_t)$, with bank units $(V_t-\delta_tS_t)/B_t$. Thus path dependence does not destroy [market completeness](../../../../../complete-market.md); it changes the information needed to determine the price and hedge.

For an arithmetic [Asian option](../../../../../asian-option.md), introduce $A_t=\int_0^tS_u du$ and seek $V_t=v(t,S_t,A_t)$. Because $dA_t=S_tdt$, [Itô formula](../../../../../ito-s-lemma.md) gives

$$
v_t+\rho s v_s+\frac12\sigma^2s^2v_{ss}+s v_a-\rho v=0,
\qquad v(T,s,a)=(a/T-K)^+.
$$

The [stock](../../../../../stock.md) holding is $v_s$. The state $a$ records the already observed average; current [stock](../../../../../stock.md) price alone cannot recover it.

A [Geometric Asian option](../../../../../geometric-asian-option.md) admits an explicit conditional calculation. Let $I_t=\int_0^t\log S_u du$ and $G_T=e^{I_T/T}$. Conditional on time $t$, the normal law of $\log G_T$ has mean and [variance](../../../../../variance-split.md)

$$
m_t=\frac{I_t+(T-t)\log S_t+\frac12(\rho-\sigma^2/2)(T-t)^2}{T},
\qquad q_t=\frac{\sigma^2(T-t)^3}{3T^2}.
$$

Indeed its random part is $\sigma T^{-1}\int_t^T(T-u)dW_u^Q$, by stochastic Fubini; the [Itô isometry](../../../../../ito-isometry.md) gives $q_t$. Completing the square in a normal exponential integral proves the [conditional geometric-average Asian option formula](../../../../../conditional-geometric-average-asian-option-formula.md)

$$
V_t=e^{-\rho(T-t)}\left[e^{m_t+q_t/2}\Phi(d_1)-K\Phi(d_2)\right],
\quad d_2=\frac{m_t-\log K}{\sqrt{q_t}},\quad d_1=d_2+\sqrt{q_t},
$$

for $K>0,t<T$. This explicitly includes the known past log-average. Holding that past integral fixed when differentiating the price gives the [stock](../../../../../stock.md) holding

$$
\delta_t=\frac{T-t}{TS_t}e^{-\rho(T-t)}e^{m_t+q_t/2}\Phi(d_1).
$$

The normal-density derivative terms cancel because $e^{m_t+q_t/2}\varphi(d_1)=K\varphi(d_2)$.

For a [lookback option](../../../../../lookback-option.md) use $M_t=\max_{u\le t}S_u$. A floating-strike put pays $M_T-S_T$. Its price $v(t,s,m)$ obeys the ordinary [Black-Scholes equation](../../../../../black-scholes-equation.md) in $0<s<m$, with terminal value $m-s$. The extra Itô term is $v_m dM_t$; since $dM_t$ is carried by $S_t=M_t$, [self-financing](../../../../../self-financing-portfolio.md) requires the [running-maximum boundary for a lookback option](../../../../../running-maximum-boundary-for-a-lookback-option.md) $v_m(t,m,m)=0$ before maturity. Equivalently its price follows from the upper-hitting [probabilities](../../../../../probability.md) in Question 3:

$$
v(t,s,m)=e^{-\rho(T-t)}\left[m+\int_m^\infty P_Q\left(\max_{t\le u\le T}S_u\ge z\,\middle|\,S_t=s\right)dz\right]-s.
$$

This uses $\mathbb E\max(m,Z)=m+\int_m^\infty P(Z\ge z)dz$ and $\mathbb E_QS_T=se^{\rho(T-t)}$. For a [barrier option](../../../../../barrier-option.md), the state must additionally record whether the barrier has already been hit; a no-rebate knockout price has an absorbing zero boundary. These augmentations give tractable PDEs or conditional-expectation computations while retaining the same [martingale](../../../../../martingale-split.md) pricing and [claim replication](../../../../../claim-replication.md) principle.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
