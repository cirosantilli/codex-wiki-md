# Paper 22

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper22.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper22.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Work in discounted units with a riskless asset of value one, trivial initial information and finitely many risky assets. Let $Y=S_1-S_0\in L^2(P;\mathbb R^d)$ be their discounted gains. A terminal [attainable claim](../../../mathematical-finance.md#attainable-european-contingent-claim) has the form $v+\theta^TY$, whose initial cost is $v$. Their span

$$
\mathcal H=\operatorname{span}\{1,Y_1,\ldots,Y_d\}\subseteq L^2(P)
$$

is a finite-dimensional closed subspace of a [Hilbert space](../../../hilbert-space.md). For $H\in L^2(P)$, [one-period least-squares hedging](../../../mathematical-finance.md#one-period-quadratic-hedge) is its [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) onto $\mathcal H$.

Let $m=\mathbb EY$, $\Sigma=\operatorname{Cov}(Y)$ and $b=\operatorname{Cov}(Y,H)$. Remove redundant risky directions so that $\Sigma$ is invertible. Under absence of [arbitrage](../../../mathematical-finance.md#arbitrage), a gain direction with zero [variance](../../../variance.md) is a constant and must be zero, so this reduction loses no genuine trading opportunity. For freely chosen capital and holdings, minimizing

$$
\mathbb E(H-v-\theta^TY)^2
$$

first gives $v=\mathbb EH-\theta^Tm$. The remaining centered error is

$$
\operatorname{Var}H-2\theta^Tb+\theta^T\Sigma\theta.
$$

Completing the square yields

$$
\boxed{\theta^*=\Sigma^{-1}b,\quad v^*=\mathbb EH-m^T\Sigma^{-1}b,\quad
\min\mathbb E(H-v-\theta^TY)^2=\operatorname{Var}H-b^T\Sigma^{-1}b.}
$$

The residual $L=H-v^*-(\theta^*)^TY$ satisfies $\mathbb EL=0$ and $\mathbb E[LY]=0$, the [least-squares normal equations](../../../linear-regression.md#normal-equations-for-linear-least-squares). Exact [claim replication](../../../mathematical-finance.md#claim-replication) is possible precisely when this residual is zero. If capital is fixed at $v$, its normal equation instead gives the [fixed-capital quadratic hedge in a one-period market](../../../mathematical-finance.md#fixed-capital-quadratic-hedge-in-a-one-period-market)

$$
\theta(v)=\bigl(\mathbb E[YY^T]\bigr)^{-1}\mathbb E[Y(H-v)].
$$

Thus fixed-capital and freely optimized hedging are distinct problems.

A [dominated martingale measure](../../../mathematical-finance.md#dominated-martingale-measure) is a [probability measure](../../../probability-theory.md#probability-measure) $Q\ll P$ with integrable gains and $\mathbb E_QY=0$. Its density $Z$ obeys $Z\ge0$, $\mathbb EZ=1$, $\mathbb E[ZY]=0$. An [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure) additionally has $Z>0$ almost surely. Every such measure prices an attainable discounted claim $v+\theta^TY$ at $v$, but different measures may give different [expectations](../../../probability-theory.md#expected-value) to an unattainable claim.

The [minimal martingale measure in a one-period market](../../../mathematical-finance.md#minimal-martingale-measure-in-a-one-period-market) is defined by preserving the mean-zero [martingale](../../../martingale.md) directions orthogonal to the gain innovation $Y-m$. Among square-integrable densities it is

$$
\boxed{Z_*=1-m^T\Sigma^{-1}(Y-m).}
$$

Indeed $\mathbb EZ_*=1$, $\mathbb E[Z_*Y]=m-\Sigma\Sigma^{-1}m=0$, and for $\mathbb EL=0$, $\mathbb E[L(Y-m)]=0$ we have $\mathbb E[Z_*L]=0$. Conversely preservation of all these orthogonal directions puts $Z$ in $\operatorname{span}\{1,Y-m\}$; normalization and zero gain [expectations](../../../probability-theory.md#expected-value) then determine $Z_*$. Any other square-integrable signed pricing density differs from $Z_*$ by a vector in $\mathcal H^\perp$, so $Z_*$ also has the smallest $L^2$ norm. Its evaluation of a claim is

$$
\mathbb E[Z_*H]=\mathbb EH-m^T\Sigma^{-1}b=v^*.
$$

This is the capital of the optimal quadratic hedge, not automatically an arbitrage-free price. The formula may define only a [signed martingale measure](../../../mathematical-finance.md#signed-martingale-measure): $Z_*$ is a genuine dominated measure only if it is nonnegative, and equivalent only if strictly positive. For example, gains $(-1,1,2)$ with [probabilities](../../../probability-theory.md#probability) $(1/10,4/5,1/10)$ have $m=9/10$, $\Sigma=49/100$ and $Z_*(2)=-50/49$. Yet [probabilities](../../../probability-theory.md#probability) $(11/20,7/20,1/10)$ are all positive and have zero gain mean. Thus absence of arbitrage does not force a positive minimal density.

For the [market completeness](../../../mathematical-finance.md#complete-market) assertion, assume absence of arbitrage and hence existence of an [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure) $Q_0$. In finite states this is the usual [fundamental theorem of asset pricing](../../../mathematical-finance.md#fundamental-theorem-of-asset-pricing); the one-period version also holds with finitely many assets on a general [probability](../../../probability-theory.md#probability) space. [Market completeness](../../../mathematical-finance.md#complete-market) means that every bounded claim is attainable, equivalently $\mathcal H=L^2(P)$ in this square-integrable setting. We now prove [completeness and uniqueness of dominated martingale measures](../../../mathematical-finance.md#completeness-and-uniqueness-of-dominated-martingale-measures).

If the model is complete, replicate every indicator $\mathbf1_A$. Two [dominated martingale measures](../../../mathematical-finance.md#dominated-martingale-measure) both evaluate it at its unique [claim replication](../../../mathematical-finance.md#claim-replication) cost, and therefore assign every event $A$ the same [probability](../../../probability-theory.md#probability). They are identical.

Conversely let $k=\dim\mathcal H$ and suppose the model is incomplete. There exist $k+1$ disjoint events $A_j$ of positive [probability](../../../probability-theory.md#probability). Otherwise the [probability](../../../probability-theory.md#probability) space would have at most $k$ atoms: any non-atomic positive event could be split to increase the number. Its whole payoff space would then have dimension at most $k$, forcing equality with $\mathcal H$ and [market completeness](../../../mathematical-finance.md#complete-market). Choose a basis $h_1,\ldots,h_k$ of $\mathcal H$. Its members are integrable under $Q_0$, because they are combinations of the constant and the gains. The $k+1$ vectors

$$
\bigl(\mathbb E_{Q_0}[h_i\mathbf1_{A_j}]\bigr)_{i=1}^k\in\mathbb R^k
$$

are linearly dependent. Hence a nonzero bounded $g=\sum_j a_j\mathbf1_{A_j}$ satisfies $\mathbb E_{Q_0}[g h]=0$ for every $h\in\mathcal H$, in particular $h=1,Y_i$. For $0<\varepsilon<1/\|g\|_\infty$, define

$$
\frac{dQ_\pm}{dQ_0}=1\pm\varepsilon g.
$$

These strictly positive densities integrate to one, preserve every gain [expectation](../../../probability-theory.md#expected-value), and give distinct [equivalent martingale measures](../../../mathematical-finance.md#risk-neutral-measure). They are also dominated by $P$. Thus uniqueness is impossible in an [incomplete market](../../../mathematical-finance.md#incomplete-market), proving the equivalence under the stated no-arbitrage hypothesis.

That hypothesis is essential. On three positive-probability states, the gain $(0,1,2)$ has the unique [dominated martingale measure](../../../mathematical-finance.md#dominated-martingale-measure), concentrated on the first state, but its attainable span has dimension only two. The market is incomplete and admits arbitrage. This explains why uniqueness among merely dominated [probabilities](../../../probability-theory.md#probability) must not be used without an equivalent pricing measure or a no-arbitrage assumption.

## 2

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Fix a finite horizon $N$, a [filtration](../../../stochastic-process.md#filtration-probability-theory) $(\mathcal F_n)$, a positive [bank account](../../../mathematical-finance.md#bank-account) $B_n$ with predictable one-step growth, ex-dividend risky prices $S_n$, and asset dividends $D_n$ paid at date $n$. Put $s_n=S_n/B_n$ and $d_n=D_n/B_n$. An [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure) $Q$ makes the discounted cum-dividend gains

$$
g_n=s_n+\sum_{j=1}^n d_j
$$

[martingales](../../../martingale.md); equivalently $\mathbb E_Q[s_n-s_{n-1}+d_n\mid\mathcal F_{n-1}]=0$. It is these gains, not necessarily the discounted ex-dividend prices alone, which enter the definition.

Let $\theta_n$ be risky holdings chosen at date $n-1$ and carried to date $n$. Let $C_n$ be the portfolio's net cash distribution to its owner at date $n$, and $V_n$ its remaining value after that distribution and rebalancing. A [self-financing portfolio](../../../mathematical-finance.md#self-financing-portfolio) with these distributions has the budget identity

$$
\frac{V_n}{B_n}-\frac{V_{n-1}}{B_{n-1}}
=\theta_n^T(s_n-s_{n-1}+d_n)-\frac{C_n}{B_n}.
$$

To see this, value the previous [stock](../../../mathematical-finance.md#stock) and bank holdings at the new prices, add the asset dividends, subtract the owner distribution, and observe that the discounted bank holding is unchanged. Rebalancing then alters holdings but not value. An asset dividend reinvested in the portfolio is already in the gain term; it is not also an owner distribution.

For a predictable strategy whose gains are integrable under $Q$ (bounded holdings in a finite-state market suffice), conditioning the gain increment gives zero. Therefore discounted remaining wealth plus cumulative discounted owner payments is a [martingale](../../../martingale.md). Conditioning its terminal value proves the [multi-period dividend pricing identity](../../../mathematical-finance.md#multi-period-dividend-pricing-identity)

$$
\boxed{V_n=B_n\mathbb E_Q\left[\frac{V_N}{B_N}+\sum_{j=n+1}^N\frac{C_j}{B_j}\,\middle|\,\mathcal F_n\right].}
$$

The relation holds under every [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure) for which these integrability conditions hold. Each payment is discounted from its own payment date, not from one common terminal date. The expression inside the [expectation](../../../probability-theory.md#expected-value) is in [bank account](../../../mathematical-finance.md#bank-account) units; multiplication by $B_n$ returns current currency units.

When the portfolio is liquidated and all its final value is paid out, $V_N=0$ after liquidation and that value is included in $C_N$. The displayed identity then involves only future discounted distributions. Without liquidation, the terminal value must remain. A [bank account](../../../mathematical-finance.md#bank-account) holding with no coupons before redemption has positive value despite having no intervening dividends; omitting its redemption or terminal holding value would plainly give the wrong result. In an infinite horizon, deleting the terminal term instead requires a [dividend-price transversality condition](../../../mathematical-finance.md#dividend-price-transversality-condition), namely convergence of its conditional discounted [expectation](../../../probability-theory.md#expected-value) to zero.

For a traded asset the same proof gives its discounted expected dividends plus terminal sale value. For a replicated claim paid only at $N$, it gives $V_n=B_n\mathbb E_Q[H/B_N\mid\mathcal F_n]$. In a [complete market](../../../mathematical-finance.md#complete-market) this prices every admissible claim uniquely. In an [incomplete market](../../../mathematical-finance.md#incomplete-market) only the portfolio's attainable payout stream has this common value under all measures; an arbitrary unattainable payoff can have different [expectations](../../../probability-theory.md#expected-value) under different measures. For a merely dominated measure the conditional identity holds $Q$-almost surely; it makes no assertion on physical states assigned zero mass by $Q$. External capital injections must also be counted, as negative owner distributions. Thus the valuation principle follows from the gain [martingale](../../../martingale.md) and the trading budget, together with the terminal convention and integrability, rather than from unconditional averaging of arbitrary future cash flows.

## 3

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Here is the Brownian change-of-drift form of the [Girsanov theorem](../../../stochastic-calculus.md#girsanov-theorem). Let $W$ be a standard [Brownian motion](../../../brownian-motion.md) on $[0,T]$ and $\theta$ predictable with $\int_0^T\theta_s^2ds<\infty$ almost surely. Suppose the [stochastic exponential](../../../stochastic-calculus.md#doleans-dade-exponential)

$$
Z_t=\exp\left(-\int_0^t\theta_s\,dW_s-\frac12\int_0^t\theta_s^2ds\right)
$$

is a true [martingale](../../../martingale.md) with $\mathbb EZ_T=1$. Define $dQ=Z_TdP$. Then $Q$ is equivalent to $P$ and

$$
\boxed{W_t^Q=W_t+\int_0^t\theta_sds\text{ is a standard Brownian motion under }Q.}
$$

The same statement holds in $d$ dimensions with scalar products, squared norms and a vector drift. [Novikov's condition](../../../stochastic-calculus.md#novikov-s-condition) $\mathbb E\exp(\frac12\int_0^T\theta_s^2ds)<\infty$ is a standard sufficient condition for the true-martingale hypothesis. Bounded $\theta$ is enough for all applications below.

For the proof, [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives $dZ_t=-Z_t\theta_t\,dW_t$. The [Itô product rule](../../../stochastic-calculus.md#ito-product-rule) gives the cancellation

$$
d(Z_tW_t^Q)=W_t^QdZ_t+Z_t(dW_t+\theta_tdt)+d[Z,W]_t
=Z_t(1-\theta_tW_t^Q)dW_t.
$$

The two drift terms cancel because $d[Z,W]_t=-Z_t\theta_tdt$. Stop $W^Q$ when its absolute value reaches $n$, at a time $\tau_n$ capped by $T$. The same product calculation makes $Z_tW_{t\wedge\tau_n}^Q$ a [local martingale](../../../martingale.md#local-martingale) under $P$. Its absolute value is at most $nZ_t$; the density [martingale](../../../martingale.md) is uniformly integrable over this finite horizon, so the stopped product is a true [martingale](../../../martingale.md). Bayes' conditional identity then gives

$$
\mathbb E_Q[W_{t\wedge\tau_n}^Q\mid\mathcal F_s]
=Z_s^{-1}\mathbb E_P[Z_tW_{t\wedge\tau_n}^Q\mid\mathcal F_s]
=W_{s\wedge\tau_n}^Q.
$$

As $n$ increases, these stopping times exhaust the horizon by continuity. Thus $W^Q$ is a continuous [local martingale](../../../martingale.md#local-martingale) under $Q$. Adding a finite-variation drift does not change [quadratic variation](../../../stochastic-calculus.md#quadratic-variation), so $[W^Q]_t=t$.

To prove the Brownian conclusion rather than just assert it, for every real $u$ apply [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $F_t=\exp(iuW_t^Q+u^2t/2)$. Its differential is $iuF_t\,dW_t^Q$, and its modulus is bounded on the fixed horizon, so it is a true [martingale](../../../martingale.md). Consequently

$$
\mathbb E_Q[e^{iu(W_t^Q-W_s^Q)}\mid\mathcal F_s]=e^{-u^2(t-s)/2}.
$$

The conditional [characteristic function](../../../probability-theory.md#characteristic-function) identifies a centered normal increment with [variance](../../../variance.md) $t-s$, independent of the past. Together with continuity and $W_0^Q=0$, this proves the Brownian assertion. For vector $u$, the same argument uses $\|u\|^2$ and gives the multivariate version. If $|\theta|\le K$, stopping $Z$ and applying [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $Z^2$ gives a uniform second-moment bound $\mathbb EZ_{t\wedge\tau}^2\le e^{K^2t}$ by [Gronwall inequality](../../../probability-and-statistics.md#gronwall-inequality); this proves uniform integrability of the stopped densities and the needed true-martingale property in the bounded case.

In the [Black-Scholes model](../../../mathematical-finance.md#black-scholes-model) with its usual augmented Brownian [filtration](../../../stochastic-process.md#filtration-probability-theory), write $dS_t=S_t(\alpha dt+\sigma dW_t)$, $B_t=e^{\rho t}$, with $\sigma>0$. Take $\theta=(\alpha-\rho)/\sigma$, the [market price of risk](../../../mathematical-finance.md#market-price-of-risk). Under $Q$, the preceding change of drift gives

$$
dS_t=\rho S_tdt+\sigma S_t dW_t^Q,
$$

so $S_t/B_t$ is a [martingale](../../../martingale.md). The [Martingale representation theorem](../../../brownian-motion.md#martingale-representation-theorem) then makes integrable Brownian-market claims attainable and gives their [risk-neutral pricing](../../../mathematical-finance.md#risk-neutral-pricing) as discounted [conditional expectations](../../../measure-theory.md#conditional-expectation). The physical drift $\alpha$ has disappeared from the price dynamics.

For the joint terminal-value and maximum law, first use the [Brownian reflection principle](../../../brownian-motion.md#reflection-principle-wiener-process) at level $a>0$. Reflecting a path after its first hit of $a$ preserves its law as a [Brownian motion](../../../brownian-motion.md) and sends a terminal value $y<a$ to $2a-y>a$; the symmetry and strong Markov property of the post-hit increments justify this map. Thus, with $\varphi_t(y)=(2\pi t)^{-1/2}e^{-y^2/(2t)}$,

$$
P(W_t\in dy,\ \sup_{s\le t}W_s<a)
=[\varphi_t(y)-\varphi_t(2a-y)]\,dy\quad(y<a).
$$

Take the constant-drift exponential density $e^{\mu W_t-\mu^2t/2}$. By [Girsanov theorem](../../../stochastic-calculus.md#girsanov-theorem), the coordinate process under this tilted measure has the law of $W_s+\mu s$ under $P$. Consequently, for $t>0$ and $x\le a$,

$$
P(W_t^\mu\le x,M_t^\mu<a)
=\int_{-\infty}^x e^{\mu y-\mu^2t/2}[\varphi_t(y)-\varphi_t(2a-y)]\,dy.
$$

Completing the squares gives

$$
e^{\mu y-\mu^2t/2}\varphi_t(y)=\varphi_t(y-\mu t),\qquad
e^{\mu y-\mu^2t/2}\varphi_t(2a-y)=e^{2a\mu}\varphi_t(y-2a-\mu t).
$$

Integrating proves

$$
\boxed{P(W_t^\mu\le x,M_t^\mu<a)=
\Phi\!\left(\frac{x-\mu t}{\sqrt t}\right)
-e^{2a\mu}\Phi\!\left(\frac{x-2a-\mu t}{\sqrt t}\right).}
$$

Here $\Phi$ is the standard normal distribution function. The first variable is the terminal Brownian value, distinct from its running maximum.

Set $T=t_0$, $a=\log(b/S_0)/\sigma>0$ and $\mu=(\rho-\sigma^2/2)/\sigma$. Under the [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure), $\log(S_s/S_0)/\sigma=W_s^Q+\mu s$. Taking $x=a$ in the joint law gives the [probability](../../../probability-theory.md#probability) of not hitting the upper level. Complementing it and discounting the unit payment at maturity gives the [one-touch option](../../../mathematical-finance.md#one-touch-option) price

$$
\boxed{V_0=e^{-\rho T}\left[
\Phi\!\left(\frac{\mu T-a}{\sqrt T}\right)
+e^{2a\mu}\Phi\!\left(\frac{-a-\mu T}{\sqrt T}\right)\right].}
$$

The exponential weight is also $(b/S_0)^{2\rho/\sigma^2-1}$. The payment occurs at $T$, even if the barrier was hit earlier, so its discount factor is $e^{-\rho T}$, not a hitting-time discount factor.

## 4

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Assume $f\in C^{1,2}$ on positive prices before maturity and the usual local trading integrability. If its value is held in [stock](../../../mathematical-finance.md#stock) units $\delta_t$ and bank units $\beta_t$, then

$$
f(S_t,t)=\delta_t S_t+\beta_t B_t,\qquad
 df=\delta_t\,dS_t+\beta_t\,dB_t
$$

for a [self-financing portfolio](../../../mathematical-finance.md#self-financing-portfolio). The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) diffusion coefficient is $\sigma S_tf_x$, so $\sigma S_t>0$ forces $\delta_t=f_x(S_t,t)$ and $\beta_tB_t=f-S_tf_x$. Equating drifts yields

$$
f_t+\alpha xf_x+\frac12\sigma^2x^2f_{xx}
=\alpha xf_x+\rho(f-xf_x).
$$

The physical drift cancels, giving the [Black-Scholes equation](../../../mathematical-finance.md#black-scholes-equation)

$$
\boxed{f_t+\frac12\sigma^2x^2f_{xx}+\rho xf_x-\rho f=0.}
$$

Conversely, if the smooth function satisfies this equation, set $\delta=f_x$ and $\beta=(f-xf_x)/B$. Substituting into [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives exactly $df=\delta dS+\beta dB$, so these holdings are [self-financing](../../../mathematical-finance.md#self-financing-portfolio). This checks the holdings as well as the value equation; a [partial differential equation](../../../partial-differential-equation.md) solution does not justify arbitrary prescribed holdings. Appropriate admissibility and growth conditions are imposed when using it as an economic price.

For the [logarithmic stock payoff](../../../mathematical-finance.md#logarithmic-stock-payoff), let $\tau=T-t$ and condition on $S_t=x$. Under the [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure),

$$
S_T=x e^{(\rho-\sigma^2/2)\tau+\sigma\sqrt\tau Z},\qquad Z\sim N(0,1).
$$

The normal exponential moment $\mathbb Ee^{uZ}=e^{u^2/2}$ and its derivative $\mathbb E[Ze^{uZ}]=u e^{u^2/2}$ give

$$
\mathbb E_Q[S_T\log S_T\mid S_t=x]
=xe^{\rho\tau}\bigl[\log x+(\rho+\sigma^2/2)\tau\bigr].
$$

Therefore

$$
\boxed{f(x,t)=x\bigl[\log x+(\rho+\sigma^2/2)(T-t)\bigr],\qquad
\delta_t=\log S_t+1+(\rho+\sigma^2/2)(T-t).}
$$

The [option delta](../../../mathematical-finance.md#option-delta) is the displayed [stock](../../../mathematical-finance.md#stock) holding. The [bank account](../../../mathematical-finance.md#bank-account) value is $f-S_tf_x=-S_t$, so $\beta_t=-S_t/B_t$. Directly, $f_{xx}=1/x$ and $f_t=-x(\rho+\sigma^2/2)$ verify the [partial differential equation](../../../partial-differential-equation.md), while $f(x,T)=x\log x$ verifies the payoff. Lognormal moments give the required pricing integrability. Since $x\log x\ge-1/e$, the conditional price is bounded below over this finite horizon, so the resulting [claim replication](../../../mathematical-finance.md#claim-replication) has the usual admissibility property.

## 5

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

**Expected utility of terminal wealth.** Let initial wealth be $x_0>0$, maturity $T=t_0$, and stock-dollar investment $\pi_t$. A [self-financing strategy](../../../mathematical-finance.md#self-financing-portfolio) in the [Black-Scholes model](../../../mathematical-finance.md#black-scholes-model) has wealth

$$
dX_t=[\rho X_t+(\alpha-\rho)\pi_t]dt+\sigma\pi_t\,dW_t.
$$

Choose admissible strategies with nonnegative wealth, and an increasing strictly concave differentiable [utility function](../../../utility-function.md) $U$ satisfying the [Inada conditions](../../../utility-function.md#inada-conditions). Assume the required [expectations](../../../probability-theory.md#expected-value) are finite and the optimization is well posed; the resulting budget equation below must have a solution. Write $\lambda=(\alpha-\rho)/\sigma$ and

$$
H_T=e^{-\rho T}\exp(-\lambda W_T-\lambda^2T/2).
$$

This [state-price density](../../../mathematical-finance.md#state-price-density) is the discounted density of the unique [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure). Nonnegative discounted wealth is a [supermartingale](../../../martingale.md#supermartingale) under that measure, so every admissible terminal wealth $Y$ obeys the [state-price budget constraint](../../../mathematical-finance.md#state-price-budget-constraint) $\mathbb E[H_TY]\le x_0$.

Conversely a nonnegative terminal claim with finite such cost is financed by its conditional [martingale](../../../martingale.md) price, which remains nonnegative; Brownian [Martingale representation theorem](../../../brownian-motion.md#martingale-representation-theorem) constructs its holdings. Thus [market completeness](../../../mathematical-finance.md#complete-market) turns dynamic optimization into a terminal-payoff problem. Let $I=(U')^{-1}$ be the [inverse marginal utility](../../../utility-function.md#inverse-marginal-utility), and choose $y>0$ from $\mathbb E[H_T I(yH_T)]=x_0$. Then the [complete-market terminal utility optimizer](../../../utility-function.md#complete-market-terminal-utility-optimizer) is

$$
\boxed{Y^*=I(yH_T).}
$$

For any feasible $Y$, concavity gives the pointwise tangent inequality

$$
U(Y)\le U(Y^*)+U'(Y^*)(Y-Y^*)
=U(Y^*)+yH_T(Y-Y^*).
$$

Taking [expectations](../../../probability-theory.md#expected-value) and using the budget proves optimality; strict concavity gives uniqueness up to null events. The optimal wealth process is

$$
X_t^*=e^{-\rho(T-t)}\mathbb E_Q[Y^*\mid\mathcal F_t]
=H_t^{-1}\mathbb E_P[H_TY^*\mid\mathcal F_t].
$$

If its discounted [martingale](../../../martingale.md) has representation $d(e^{-\rho t}X_t^*)=\zeta_t dW_t^Q$, hold $\delta_t=e^{\rho t}\zeta_t/(\sigma S_t)$ [stock](../../../mathematical-finance.md#stock) units and invest the remainder in the [bank account](../../../mathematical-finance.md#bank-account). This derives the strategy, not only the terminal first-order condition.

The equivalent dynamic approach is the [Bellman equation for terminal-wealth utility](../../../mathematical-finance.md#bellman-equation-for-terminal-wealth-utility). For a smooth concave value $v(t,x)$, dynamic programming and [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) give

$$
v_t+\rho xv_x+\sup_\pi\left[(\alpha-\rho)\pi v_x+\frac12\sigma^2\pi^2v_{xx}\right]=0,
\qquad v(T,x)=U(x).
$$

For $v_{xx}<0$, maximizing the concave quadratic gives $\pi^*=-(\alpha-\rho)v_x/(\sigma^2v_{xx})$. For an arbitrary admissible control the Itô drift of $v(t,X_t)$ is nonpositive; localization and integrability therefore bound its expected terminal utility by $v(0,x_0)$. The maximizing control makes the drift zero, giving equality when the verification [expectations](../../../probability-theory.md#expected-value) are valid.

For [CRRA utility](../../../utility-function.md#constant-relative-risk-aversion-utility) $U(x)=x^{1-\gamma}/(1-\gamma)$, $\gamma>0$, $\gamma\ne1$, substitution gives

$$
v(t,x)=\frac{x^{1-\gamma}}{1-\gamma}
\exp\!\left((1-\gamma)\left[\rho+\frac{\lambda^2}{2\gamma}\right](T-t)\right),
\qquad\boxed{\frac{\pi_t^*}{X_t^*}=\frac{\alpha-\rho}{\gamma\sigma^2}.}
$$

The optimal [stock](../../../mathematical-finance.md#stock) fraction is constant. Its geometric wealth dynamics stay positive, so it is feasible. For [logarithmic utility](../../../utility-function.md#logarithmic-utility) the fraction is $(\alpha-\rho)/\sigma^2$ and $v(t,x)=\log x+(\rho+\lambda^2/2)(T-t)$. [Risk aversion](../../../utility-function.md#risk-aversion) controls the risky exposure, while the market price of risk controls its reward.

**Pricing claims depending on the path.** For a [path-dependent contingent claim](../../../mathematical-finance.md#path-dependent-contingent-claim) $C=F((S_u)_{0\le u\le T})$, the [risk-neutral pricing](../../../mathematical-finance.md#risk-neutral-pricing) process is

$$
V_t=e^{-\rho(T-t)}\mathbb E_Q[C\mid\mathcal F_t].
$$

For square-integrable discounted $C$, the Brownian [Martingale representation theorem](../../../brownian-motion.md#martingale-representation-theorem) gives $d(e^{-\rho t}V_t)=\varphi_t dW_t^Q$. Since $d(e^{-\rho t}S_t)=\sigma e^{-\rho t}S_t dW_t^Q$, the replicating holding is $\delta_t=\varphi_t/(\sigma e^{-\rho t}S_t)$, with bank units $(V_t-\delta_tS_t)/B_t$. Thus path dependence does not destroy [market completeness](../../../mathematical-finance.md#complete-market); it changes the information needed to determine the price and hedge.

For an arithmetic [Asian option](../../../mathematical-finance.md#asian-option), introduce $A_t=\int_0^tS_u du$ and seek $V_t=v(t,S_t,A_t)$. Because $dA_t=S_tdt$, [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives

$$
v_t+\rho s v_s+\frac12\sigma^2s^2v_{ss}+s v_a-\rho v=0,
\qquad v(T,s,a)=(a/T-K)^+.
$$

The [stock](../../../mathematical-finance.md#stock) holding is $v_s$. The state $a$ records the already observed average; current [stock](../../../mathematical-finance.md#stock) price alone cannot recover it.

A [Geometric Asian option](../../../mathematical-finance.md#geometric-asian-option) admits an explicit conditional calculation. Let $I_t=\int_0^t\log S_u du$ and $G_T=e^{I_T/T}$. Conditional on time $t$, the normal law of $\log G_T$ has mean and [variance](../../../variance.md)

$$
m_t=\frac{I_t+(T-t)\log S_t+\frac12(\rho-\sigma^2/2)(T-t)^2}{T},
\qquad q_t=\frac{\sigma^2(T-t)^3}{3T^2}.
$$

Indeed its random part is $\sigma T^{-1}\int_t^T(T-u)dW_u^Q$, by stochastic Fubini; the [Itô isometry](../../../stochastic-calculus.md#ito-isometry) gives $q_t$. Completing the square in a normal exponential integral proves the [conditional geometric-average Asian option formula](../../../mathematical-finance.md#conditional-geometric-average-asian-option-formula)

$$
V_t=e^{-\rho(T-t)}\left[e^{m_t+q_t/2}\Phi(d_1)-K\Phi(d_2)\right],
\quad d_2=\frac{m_t-\log K}{\sqrt{q_t}},\quad d_1=d_2+\sqrt{q_t},
$$

for $K>0,t<T$. This explicitly includes the known past log-average. Holding that past integral fixed when differentiating the price gives the [stock](../../../mathematical-finance.md#stock) holding

$$
\delta_t=\frac{T-t}{TS_t}e^{-\rho(T-t)}e^{m_t+q_t/2}\Phi(d_1).
$$

The normal-density derivative terms cancel because $e^{m_t+q_t/2}\varphi(d_1)=K\varphi(d_2)$.

For a [lookback option](../../../mathematical-finance.md#lookback-option) use $M_t=\max_{u\le t}S_u$. A floating-strike put pays $M_T-S_T$. Its price $v(t,s,m)$ obeys the ordinary [Black-Scholes equation](../../../mathematical-finance.md#black-scholes-equation) in $0<s<m$, with terminal value $m-s$. The extra Itô term is $v_m dM_t$; since $dM_t$ is carried by $S_t=M_t$, [self-financing](../../../mathematical-finance.md#self-financing-portfolio) requires the [running-maximum boundary for a lookback option](../../../mathematical-finance.md#running-maximum-boundary-for-a-lookback-option) $v_m(t,m,m)=0$ before maturity. Equivalently its price follows from the upper-hitting [probabilities](../../../probability-theory.md#probability) in Question 3:

$$
v(t,s,m)=e^{-\rho(T-t)}\left[m+\int_m^\infty P_Q\left(\max_{t\le u\le T}S_u\ge z\,\middle|\,S_t=s\right)dz\right]-s.
$$

This uses $\mathbb E\max(m,Z)=m+\int_m^\infty P(Z\ge z)dz$ and $\mathbb E_QS_T=se^{\rho(T-t)}$. For a [barrier option](../../../mathematical-finance.md#barrier-option), the state must additionally record whether the barrier has already been hit; a no-rebate knockout price has an absorbing zero boundary. These augmentations give tractable PDEs or conditional-expectation computations while retaining the same [martingale](../../../martingale.md) pricing and [claim replication](../../../mathematical-finance.md#claim-replication) principle.

## 6

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

The entire term structure is naturally indexed by observation time and maturity. Work under a [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure) $Q$ and let $f(t,T)$ be the [instantaneous forward rate](../../../mathematical-finance.md#instantaneous-forward-rate), with $0\le t\le T$. Define the [short rate](../../../mathematical-finance.md#short-rate) $r_t=f(t,t)$, the [bank account](../../../mathematical-finance.md#bank-account) $B_t=\exp(\int_0^t r_sds)$ and the [zero-coupon bond](../../../mathematical-finance.md#zero-coupon-bond) price

$$
P(t,T)=\exp\left(-\int_t^T f(t,u)du\right).
$$

An arbitrary Gaussian mean and [covariance](../../../variance.md#covariance) need not make these bond prices consistent. Absence of [arbitrage](../../../mathematical-finance.md#arbitrage) requires the discounted traded bonds to be [martingales](../../../martingale.md) under a suitable equivalent measure. We derive the constraint explicitly.

Consider the [Gaussian forward-rate field](../../../mathematical-finance.md#gaussian-forward-rate-field) $f(t,T)=m(t,T)+X(t,T)$ with deterministic mean and centered [Gaussian random field](../../../stochastic-process.md#gaussian-random-field) satisfying

$$
\operatorname{Cov}(X(s,T),X(t,U))=c(s\wedge t;T,U),\qquad c(0;T,U)=0.
$$

The maturity kernel is symmetric, and its increments in the first parameter must be positive semidefinite kernels. Assume continuity, separability and sufficient integrability for the following mean-square integrals and maturity derivatives. This [covariance](../../../variance.md#covariance) gives independent observation-time increments, while permitting correlated fluctuations across all maturities. The [filtration](../../../stochastic-process.md#filtration-probability-theory) contains the history of the whole observed forward curve.

For a fixed maturity $T$, collect the past [short rate](../../../mathematical-finance.md#short-rate) and the present curve into the [integrated Gaussian forward-rate process](../../../mathematical-finance.md#integrated-gaussian-forward-rate-process)

$$
Y(t,T)=\int_0^T X(t\wedge u,u)du,
\quad A(t,T)=\int_0^t m(u,u)du+\int_t^T m(t,u)du.
$$

Then $P(t,T)/B_t=e^{-A(t,T)-Y(t,T)}$. Its centered Gaussian [variance](../../../variance.md) is

$$
v(t,T)=\int_0^T\int_0^T c(t\wedge u\wedge w;u,w)du\,dw.
$$

For $s<t$ and an observed field coordinate $X(z,U)$ with $z\le s$, the [covariance](../../../variance.md#covariance) of $Y(t,T)-Y(s,T)$ with it is zero: the integrand is

$$
c(t\wedge u\wedge z;u,U)-c(s\wedge u\wedge z;u,U)=0.
$$

The [uncorrelated jointly Gaussian variables are independent](../../../probability-and-statistics.md#uncorrelated-jointly-normal-variables-are-independent) principle therefore makes the increment independent of the earlier field [filtration](../../../stochastic-process.md#filtration-probability-theory). Its [variance](../../../variance.md) is $v(t,T)-v(s,T)$, since the same [covariance](../../../variance.md#covariance) calculation gives $\operatorname{Cov}(Y(t,T),Y(s,T))=v(s,T)$. Conditional Gaussian exponential [expectation](../../../probability-theory.md#expected-value) now gives

$$
\mathbb E_Q[e^{-A(t,T)-Y(t,T)}\mid\mathcal F_s]
=e^{-A(t,T)-Y(s,T)+[v(t,T)-v(s,T)]/2}.
$$

Hence the exact bond-martingale condition is

$$
A(t,T)-A(0,T)=\frac12v(t,T).
$$

Differentiating in maturity, using symmetry of the [covariance](../../../variance.md#covariance), gives the [Gaussian forward-rate covariance drift restriction](../../../mathematical-finance.md#gaussian-forward-rate-covariance-drift-restriction)

$$
\boxed{m(t,T)=f(0,T)+\int_0^T c(t\wedge u;u,T)du.}
$$

This is necessary and sufficient. For sufficiency, the derivatives of the half-variance identity agree by the displayed restriction. Its integration constant also agrees at $T=t$, because

$$
A(t,t)-A(0,t)=\int_0^t\int_0^u c(w;w,u)dw\,du=\frac12v(t,t).
$$

Thus the full identity follows for every $T\ge t$, and the [conditional expectation](../../../measure-theory.md#conditional-expectation) calculation proves a true [martingale](../../../martingale.md), not merely zero formal drift. The initial mean $f(0,T)=-\partial_T\log P(0,T)$ fits the observed initial curve exactly; thereafter the mean adjustment is fixed by the [covariance](../../../variance.md#covariance).

If $c(t;T,U)=\int_0^t k_s(T,U)ds$ is time-differentiable, the forward drift is $a(t,T)=\int_t^T k_t(T,u)du$. Writing

$$
k_t(T,U)=\langle\sigma(t,T),\sigma(t,U)\rangle
$$

with deterministic finite- or Hilbert-space factor loadings gives the [Heath-Jarrow-Morton model](../../../mathematical-finance.md#heath-jarrow-morton-model)

$$
df(t,T)=\left\langle\sigma(t,T),\int_t^T\sigma(t,u)du\right\rangle dt
+\langle\sigma(t,T),dW_t^Q\rangle.
$$

With $\Sigma(t,T)=\int_t^T\sigma(t,u)du$, [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) independently verifies bond drift $r_t-\int_t^Ta(t,u)du+\|\Sigma(t,T)\|^2/2=r_t$. Finite-factor models give low-rank maturity correlations; a genuine random field or an infinite factor space permits a much richer [covariance](../../../variance.md#covariance) structure. Gaussian forward rates and [short rates](../../../mathematical-finance.md#short-rate) may be negative, although the exponential bond prices stay positive. Under a physical measure, a [Girsanov theorem](../../../stochastic-calculus.md#girsanov-theorem) market-risk-premium change adds $\langle\sigma,\lambda\rangle$ to the forward drift; deterministic premia preserve Gaussianity, whereas arbitrary adapted premia need not.

For a concrete two-parameter example, let $X$ be a standard [Brownian sheet](../../../stochastic-process.md#brownian-sheet), so $c(t;T,U)=t\min(T,U)$. The restriction gives

$$
m(t,T)=f(0,T)+\frac12tT^2-\frac16t^3\qquad(t\le T).
$$

Indeed $\int_0^T\min(t,u)u\,du=t^3/3+t(T^2-t^2)/2$. This demonstrates directly how a [Gaussian random field](../../../stochastic-process.md#gaussian-random-field) determines the compensating forward drift.

For the one-factor constant-volatility case, $\sigma(t,T)=\eta$, the [Constant-coefficient Ho-Lee model](../../../mathematical-finance.md#gaussian-short-rate-model-with-constant-coefficients) has

$$
f(t,T)=f(0,T)+\eta^2(tT-t^2/2)+\eta W_t^Q,
\qquad r_t=f(0,t)+\eta^2t^2/2+\eta W_t^Q,
$$

and

$$
P(t,T)=\frac{P(0,T)}{P(0,t)}
\exp\left[-\eta(T-t)W_t^Q-\frac12\eta^2tT(T-t)\right].
$$

These follow by integrating the explicit curve, not by assigning the short-rate drift independently. Exponentially decaying loadings $\eta e^{-\kappa(T-t)}$ instead give a Gaussian mean-reverting [Hull-White model](../../../mathematical-finance.md#hull-white-model), with bond-rate loading $(1-e^{-\kappa(T-t)})/\kappa$.

A practical advantage is an explicit [Gaussian bond-option formula](../../../mathematical-finance.md#gaussian-bond-option-formula). For a call of strike $K>0$ exercised at $T$ on a bond maturing at $U>T$, use the [T-forward measure](../../../mathematical-finance.md#t-forward-measure) with numéraire $P(t,T)$. The forward bond ratio $F_t=P(t,U)/P(t,T)$ has a [lognormal distribution](../../../probability-theory.md#log-normal-distribution) under that measure, with remaining integrated [variance](../../../variance.md)

$$
q=\int_t^T\|\Sigma(s,U)-\Sigma(s,T)\|^2ds.
$$

Its [martingale](../../../martingale.md) property makes the conditional log mean $\log F_t-q/2$. Evaluating the positive-part lognormal integral gives

$$
\boxed{C_t=P(t,U)\Phi(d_1)-KP(t,T)\Phi(d_2),\quad
 d_1=\frac{\log(F_t/K)+q/2}{\sqrt q},\quad d_2=d_1-\sqrt q.}
$$

For $q=0$, the limit is $(P(t,U)-KP(t,T))^+$. The forward measure accounts for the stochastic [short rate](../../../mathematical-finance.md#short-rate); discounting by one deterministic interest rate would generally be wrong. Calibration selects a positive-semidefinite [covariance](../../../variance.md#covariance) structure fitting observed rate co-movements and option prices, with the no-arbitrage mean restriction imposed afterward. With more independent factors than the available traded bond exposures span, the market is incomplete and additional claims need a specified pricing measure or risk-premium model. The Gaussian field is therefore a flexible curve model with explicit consistency and pricing equations, rather than a claim that all possible rate risks are hedgeable.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
