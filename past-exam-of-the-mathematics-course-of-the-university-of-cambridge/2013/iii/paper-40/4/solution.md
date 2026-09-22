<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**Pricing kernel and replication.** In the nondegenerate [Black-Scholes model](../../../../../black-scholes-model.md), put $\kappa=(\mu-r)/\sigma$ and normalize the [state-price density](../../../../../state-price-density.md) by $\zeta_0=1$. The process is

$$
\boxed{\zeta_t=\exp\{-rt-\kappa W_t-\tfrac12\kappa^2t\},\qquad
d\zeta_t=-\zeta_t(r\,dt+\kappa\,dW_t).}
$$

The density $e^{rt}\zeta_t$ changes probability to the [risk-neutral measure](../../../../../risk-neutral-measure.md). Under that measure $W_t+\kappa t$ is a [Brownian motion](../../../../../brownian-motion-split.md) and the stock drift is $r$. Thus an integrable [contingent claim](../../../../../contingent-claim.md) $H$ has time-$t$ price

$$
\boxed{P_t=\frac{\mathbb E[\zeta_T H\mid\mathcal F_t]}{\zeta_t}
=e^{-r(T-t)}\mathbb E^{\mathbb Q}[H\mid\mathcal F_t].}
$$

In the usual augmented [natural Brownian filtration](../../../../../natural-brownian-filtration.md), the [Brownian martingale representation theorem](../../../../../brownian-martingale-representation-theorem.md) supplies a [replicating strategy](../../../../../replicating-strategy.md); this is the [complete market](../../../../../complete-market.md) assumption. For a nonnegative [admissible trading strategy](../../../../../admissible-trading-strategy.md) without intermediate [consumption](../../../../../consumption.md), the [state-price budget constraint](../../../../../state-price-budget-constraint.md) is $\mathbb E[\zeta_Tw_T]\leq w_0$, with equality for a fully invested replicated claim. In particular

$$
\mathbb E\zeta_T=e^{-rT},\qquad \mathbb E[\zeta_TS_T]=S_0.
$$

**Feasibility and the largest slope.** First take the intended regime $r>0$, $T>0$, $w_0,S_0>0$, and the usual nonnegative [portfolio wealth](../../../../../portfolio-wealth.md) constraint. The [terminal wealth floor](../../../../../terminal-wealth-floor.md) is

$$
\xi=w_0+\alpha(S_T-S_0).
$$

For any feasible claim the [state-price budget constraint](../../../../../state-price-budget-constraint.md) implies

$$
w_0\geq\mathbb E[\zeta_Tw_T]\geq
\mathbb E[\zeta_T\xi]
=w_0e^{-rT}+\alpha S_0(1-e^{-rT}).
$$

Therefore $\alpha\leq w_0/S_0$. Conversely, when $0\leq\alpha\leq w_0/S_0$, hold $\alpha$ shares and put the remaining $w_0-\alpha S_0$ in the [continuous-time bank account](../../../../../continuous-time-bank-account.md). Its terminal [portfolio wealth](../../../../../portfolio-wealth.md) is

$$
\alpha S_T+(w_0-\alpha S_0)e^{rT}
\geq\alpha S_T+(w_0-\alpha S_0)=\xi.
$$

Hence

$$
\boxed{\bar\alpha=\frac{w_0}{S_0}.}
$$

At equality, $\xi=\bar\alpha S_T$ has cost exactly $w_0$. Positivity of the [state-price density](../../../../../state-price-density.md) forces $w_T=\bar\alpha S_T$ almost surely: any strict improvement would cost more. **Invest all initial [portfolio wealth](../../../../../portfolio-wealth.md) in $w_0/S_0$ shares and hold them until $T$.**

**Optimal payoff below the feasibility limit.** For $\alpha<\bar\alpha$ the floor is strictly positive, and its price is strictly less than $w_0$. Assume the [utility function](../../../../../utility-function-split.md) is increasing, differentiable and strictly [concave](../../../../../concave-function.md), satisfies the [Inada conditions](../../../../../inada-conditions.md), and has the integrability needed for the finite-budget optimization. These are the usual hypotheses implicit in using [inverse marginal utility](../../../../../inverse-marginal-utility.md). For each positive multiplier $\lambda$, maximize

$$
U(y)-\lambda\zeta_Ty\qquad\text{over }y\geq\xi
$$

separately in every state. Its derivative decreases through zero at $I(\lambda\zeta_T)$, so the [floored marginal utility optimizer](../../../../../floored-marginal-utility-optimizer.md) is

$$
\boxed{w_T^*=\max\{w_0+\alpha(S_T-S_0),\,I(\lambda\zeta_T)\}.}
$$

The multiplier is characterized by

$$
\boxed{\mathbb E\!\left[\zeta_T\max\{\xi,I(\lambda\zeta_T)\}\right]=w_0,\qquad \lambda>0.}
$$

Under the stated integrability hypotheses the left side is continuous and decreasing, tends to the floor cost as $\lambda\uparrow\infty$, and tends to infinity as $\lambda\downarrow0$. It is strictly decreasing wherever it exceeds the floor cost: on the event where the inverse-marginal-utility payoff exceeds the floor, a larger multiplier strictly reduces that payoff. Therefore the budget determines a unique finite multiplier. For [CRRA utility](../../../../../constant-relative-risk-aversion-utility.md) the [inverse marginal utility](../../../../../inverse-marginal-utility.md) is $I(y)=y^{-1/R}$; lognormal moments provide the needed integrability.

For completeness, pointwise maximality gives, for any feasible competing terminal [portfolio wealth](../../../../../portfolio-wealth.md) $Y$,

$$
U(Y)-\lambda\zeta_TY
\leq U(w_T^*)-\lambda\zeta_Tw_T^*.
$$

Taking expectations and using $\mathbb E[\zeta_TY]\leq w_0=\mathbb E[\zeta_Tw_T^*]$ proves optimality. Strict [concavity](../../../../../concave-function.md) gives uniqueness of the terminal claim. Its price process

$$
w_t^*=\frac{\mathbb E[\zeta_Tw_T^*\mid\mathcal F_t]}{\zeta_t}
$$

is nonnegative and starts from $w_0$; [claim replication](../../../../../claim-replication.md) therefore turns the payoff optimizer into an admissible portfolio.

**What the missing interest-rate hypothesis changes.** The PDF does not explicitly assume $r>0$ or give the utility and admissibility hypotheses above. These omissions matter. At $r=0$, under nonnegative admissibility, the largest feasible slope remains $w_0/S_0$: for larger slopes the positive-part floor costs strictly more than $w_0$, since $S_T$ has support $(0,\infty)$. But every $\alpha\leq w_0/S_0$ already gives floor cost exactly $w_0$, so the only feasible terminal claim is $\xi$. There is no spare budget for an inverse-marginal-utility improvement. For example $\alpha=0$, $\kappa\ne0$ and [CRRA utility](../../../../../constant-relative-risk-aversion-utility.md) make $\mathbb E[\zeta_T\max\{w_0,I(\lambda\zeta_T)\}]>w_0$ for every finite $\lambda$. The prescribed positive finite multiplier then does not exist.

For negative $r$, nonnegative admissibility requires the effective floor $\xi_+=\max\{\xi,0\}$. Define its cost

$$
G(\alpha)=\mathbb E[\zeta_T(w_0+\alpha(S_T-S_0))_+].
$$

This is continuous and convex. For $\alpha\leq w_0/S_0$ it equals $w_0e^{-rT}+\alpha S_0(1-e^{-rT})$, exceeding $w_0$ below the endpoint. At $\alpha_0=w_0/S_0$, $G(\alpha_0)=w_0$ and $G'(\alpha_0)=S_0(1-e^{-rT})<0$. Above that endpoint the lognormal stock gives strict convexity, and $G(\alpha)\to\infty$. Thus there is a unique second root $\alpha_1>\alpha_0$ of $G(\alpha_1)=w_0$, the feasible slopes are $[\alpha_0,\alpha_1]$, and the largest is $\alpha_1$. Equivalently, for $\alpha>\alpha_0$ the floor price is $\alpha$ times the [European call option](../../../../../european-call-option.md) price with strike $S_0-w_0/\alpha$. At the upper endpoint replicate $\xi_+$; in the interval with strict budget slack the same [floored marginal utility optimizer](../../../../../floored-marginal-utility-optimizer.md) applies with $\xi_+$.

If instead [portfolio wealth](../../../../../portfolio-wealth.md) may be negative and utility is defined on all real [portfolio wealth](../../../../../portfolio-wealth.md), the floor itself has its affine replication cost: at $r=0$ every slope is feasible, and at negative $r$ every $\alpha\geq w_0/S_0$ is feasible. There is then no largest finite slope. **The intended stock-only endpoint and strict-slack optimizer use positive interest and standard nonnegative admissibility.**

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
