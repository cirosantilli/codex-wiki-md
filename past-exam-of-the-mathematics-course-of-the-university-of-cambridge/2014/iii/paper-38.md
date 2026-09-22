# Paper 38

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_38.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_38.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)
  - [d](#6/d)
    - [Solution](#6/d/solution)
  - [e](#6/e)
    - [Solution](#6/e/solution)

## 1

↑ **Parent:** [Paper 38](paper-38.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Choose a [localizing sequence](../../../martingale.md#localizing-sequence) of discrete-time [stopping times](../../../martingale.md#stopping-time) $\tau_j\uparrow\infty$ for $X$. For fixed integer $t$, every stopped value is bounded in absolute value by the finite sum

$$
|X_{t\wedge\tau_j}|\leq\sum_{u=0}^t|X_u|.
$$

That sum is [integrable](../../../measure-theory.md#integrability) under the hypothesis. Since $X^{\tau_j}$ is a [martingale](../../../martingale.md),

$$
\mathbb E[X_{t\wedge\tau_j}\mid\mathcal F_{t-1}]
=X_{(t-1)\wedge\tau_j}.
$$

The [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem), including its conditional version, now removes the stopping. Thus $\mathbb E[X_t\mid\mathcal F_{t-1}]=X_{t-1}$. The process is [adapted](../../../stochastic-process.md#adapted-process) and [integrable](../../../measure-theory.md#integrability) by hypothesis, so **$X$ is a true discrete-time [martingale](../../../martingale.md)**. This is the [integrable discrete-time local martingale is a martingale](../../../martingale.md#integrable-discrete-time-local-martingale-is-a-martingale) criterion. The finite sum dominating stopped values is the crucial discrete-time feature.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The stopped processes are nonnegative [martingales](../../../martingale.md). Their [expectations](../../../probability-theory.md#expected-value) equal the finite deterministic value $X_0$. The [Fatou lemma](../../../measure-theory.md#fatou-s-lemma) gives, for each fixed integer $t$,

$$
\mathbb E X_t\leq\liminf_j\mathbb E X_{t\wedge\tau_j}=X_0<\infty.
$$

Thus every $X_t$ is [integrable](../../../measure-theory.md#integrability). Apply the preceding discrete-time criterion to conclude **$X$ is a [martingale](../../../martingale.md)**, not merely a [supermartingale](../../../martingale.md#supermartingale). This is the [nonnegative discrete-time local martingale is a martingale](../../../martingale.md#nonnegative-discrete-time-local-martingale-is-a-martingale) result; its conclusion does not extend to arbitrary continuous-time nonnegative [local martingales](../../../martingale.md#local-martingale).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Predictability means $K_s$ is $\mathcal F_{s-1}$-measurable. If $|K_s|\leq L$, each product $K_s(M_s-M_{s-1})$ is [integrable](../../../measure-theory.md#integrability), and the finite sum defining $Y_t$ is [integrable](../../../measure-theory.md#integrability). Pulling the bounded [predictable](../../../martingale.md#predictable-process) factor out of the [conditional expectation](../../../measure-theory.md#conditional-expectation) gives

$$
\mathbb E[Y_t-Y_{t-1}\mid\mathcal F_{t-1}]
=K_t\mathbb E[M_t-M_{t-1}\mid\mathcal F_{t-1}]=0.
$$

Therefore **the bounded [predictable](../../../martingale.md#predictable-process) [martingale transform](../../../martingale.md#martingale-transform) $Y$ is a [martingale](../../../martingale.md) starting at zero**.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Stop just before a large [predictable](../../../martingale.md#predictable-process) coefficient would be used. Set

$$
\sigma_j=\inf\{t\geq0:|K_{t+1}|>j\},
$$

with the infimum of the empty set equal to infinity. Because $K_{t+1}$ is $\mathcal F_t$-measurable, $\sigma_j$ is a [stopping time](../../../martingale.md#stopping-time). The increment of the stopped [martingale transform](../../../martingale.md#martingale-transform) is

$$
Y_{t\wedge\sigma_j}-Y_{(t-1)\wedge\sigma_j}
=\mathbf1_{\{t\leq\sigma_j\}}K_t(M_t-M_{t-1}).
$$

Its coefficient is [predictable](../../../martingale.md#predictable-process) and bounded by $j$: the first coefficient exceeding $j$ occurs at the step after stopping, and is never included. Part (c) makes $Y^{\sigma_j}$ a [martingale](../../../martingale.md). Since the finitely many $K_s$ on any fixed finite horizon are finite almost surely, $\sigma_j\uparrow\infty$ almost surely. Thus

$$
\boxed{Y\text{ is a discrete-time local martingale}.}
$$

This is [predictable-coefficient localization of a martingale transform](../../../martingale.md#predictable-coefficient-localization-of-a-martingale-transform). Stopping after taking the large increment would not give the required bound.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

First propagate terminal nonnegativity backwards; it is not necessary to assume nonnegative wealth at intermediate dates. Suppose $Y_t\geq0$ and define

$$
A_j=\{|Y_{t-1}|\leq j,\ |K_t|\leq j\}\in\mathcal F_{t-1}.
$$

These events increase to the whole space up to a null set. On $A_j$, both the old value and the coefficient are bounded, so $\mathbf1_{A_j}Y_t$ is [integrable](../../../measure-theory.md#integrability) and

$$
\mathbb E[\mathbf1_{A_j}Y_t\mid\mathcal F_{t-1}]
=\mathbf1_{A_j}Y_{t-1}.
$$

The left side is nonnegative; hence $Y_{t-1}\geq0$ on every $A_j$, and therefore almost surely. Starting from $t=T$, induction gives $Y_t\geq0$ for every $0\leq t\leq T$.

The process stopped at $T$ is now a nonnegative discrete-time [local martingale](../../../martingale.md#local-martingale). Part (b) makes it a [martingale](../../../martingale.md) with initial value zero. Consequently $\mathbb E Y_T=0$, and a nonnegative random variable with zero [expectation](../../../probability-theory.md#expected-value) vanishes almost surely:

$$
\boxed{Y_T=0\quad\text{almost surely}.}
$$

This is the [terminal nonnegativity criterion for a finite-horizon martingale transform](../../../martingale.md#terminal-nonnegativity-criterion-for-a-finite-horizon-martingale-transform). A finite deterministic horizon is essential to the backward induction.

## 2

↑ **Parent:** [Paper 38](paper-38.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A trading strategy chooses a vector $H_t$ of holdings for the period $(t-1,t]$, with $H_t$ measurable with respect to $\mathcal F_{t-1}$. Its end-of-period wealth is $X_t=H_t\cdot P_t$. Rebalancing at date $t$ is [self-financing](../../../mathematical-finance.md#self-financing-portfolio) when

$$
H_{t+1}\cdot P_t=H_t\cdot P_t;
$$

new holdings cost exactly the value released by the old holdings. With fixed initial capital $x$, the equivalent gains identity is

$$
\boxed{X_t=x+\sum_{u=1}^t H_u\cdot(P_u-P_{u-1}).}
$$

A [European contingent claim](../../../mathematical-finance.md#european-contingent-claim) is a maturity-$T$ payoff $\xi$ measurable with respect to $\mathcal F_T$. It is attainable if there exists a [predictable](../../../martingale.md#predictable-process) [self-financing strategy](../../../mathematical-finance.md#self-financing-portfolio) and an initial capital $x$ for which $X_T=\xi$ almost surely. Such a strategy is a [replicating strategy](../../../mathematical-finance.md#replicating-strategy), and $x$ is its initial replication cost. Holdings are understood only up to the maturity being replicated.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

On a finite sample space, all real-valued holdings over the finite interval $0,\ldots,T$ are bounded after null states are discarded. The gains identity is therefore a bounded [predictable](../../../martingale.md#predictable-process) [martingale transform](../../../martingale.md#martingale-transform) of the vector [martingale](../../../martingale.md) $P$, summed over its coordinates. It follows that $X$ is a [martingale](../../../martingale.md), so

$$
\boxed{x=\mathbb E X_T=\mathbb E\xi.}
$$

Here the replication cost is a prescribed deterministic initial capital, as in the definition of attainability. The stronger intermediate identity is $X_t=\mathbb E[\xi\mid\mathcal F_t]$. If initial capital is instead allowed to be $\mathcal F_0$-measurable and random, the corresponding statement is $X_0=\mathbb E[\xi\mid\mathcal F_0]$; its unconditional [expectation](../../../probability-theory.md#expected-value) still equals $\mathbb E\xi$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $\pi_t$ be the [predictable](../../../martingale.md#predictable-process) [stock](../../../mathematical-finance.md#stock) holding during $(t-1,t]$. Cash has constant price, so [self-financing](../../../mathematical-finance.md#self-financing-portfolio) gives

$$
X_t-X_{t-1}=\pi_t(S_t-S_{t-1}),\qquad
X_t=\mathbb E[\xi\mid\mathcal F_t].
$$

Put $\mathcal G=\mathcal F_{t-1}$. The [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation) and $\mathcal F_t$-measurability of $S_t$ give

$$
\operatorname{Cov}(\xi,S_t\mid\mathcal G)
=\operatorname{Cov}(X_t,S_t\mid\mathcal G).
$$

Since $X_{t-1}$, $S_{t-1}$ and $\pi_t$ are $\mathcal G$-measurable, substituting the gains identity yields

$$
\operatorname{Cov}(X_t,S_t\mid\mathcal G)
=\pi_t\operatorname{Var}(S_t\mid\mathcal G).
$$

The denominator is positive on every positive-probability parent atom. If it were zero on such an atom, $S_t$ would be constant there, and the [martingale](../../../martingale.md) property would force that constant to equal $S_{t-1}$, contradicting the nonzero-increment assumption. Hence

$$
\boxed{\pi_t=\frac{\operatorname{Cov}(\xi,S_t\mid\mathcal F_{t-1})}
{\operatorname{Var}(S_t\mid\mathcal F_{t-1})},\qquad1\leq t\leq T.}
$$

This is [conditional covariance hedge ratio](../../../martingale.md#recovery-of-a-martingale-transform-integrand-by-conditional-covariance). It uses attainability; a regression coefficient alone would not replicate a general unattainable payoff. After maturity one may liquidate into cash, so the same formula gives zero for later dates wherever its denominator remains nonzero. On a finite sample space a [martingale](../../../martingale.md) cannot have nonzero increments forever; the stated nondegeneracy is naturally a finite-maturity assumption.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Work conditionally on a positive-probability atom of $\mathcal F_{T-1}$. Let $Z$ have the [conditional distribution](../../../probability-theory.md#conditional-distribution) of $S_T$ there, and let $Z'$ be an independent copy of that conditional law. The finite sample space makes all [expectations](../../../probability-theory.md#expected-value) finite. Then

$$
2\operatorname{Cov}(g(Z),Z)
=\mathbb E[(g(Z)-g(Z'))(Z-Z')].
$$

Strict increase of $g$ makes the integrand nonnegative, and strictly positive whenever $Z\ne Z'$. The [conditional variance](../../../variance.md#conditional-variance) is positive by part (c), so the [conditional distribution](../../../probability-theory.md#conditional-distribution) is nondegenerate and $\mathbb P(Z\ne Z')>0$. Thus the numerator of the hedge ratio is strictly positive on every such atom. The denominator is also positive, giving

$$
\boxed{\pi_T>0\quad\text{almost surely}.}
$$

This is [strict positive covariance with an increasing payoff](../../../variance.md#strict-positive-covariance-with-an-increasing-payoff). The independent copy is taken from the [conditional distribution](../../../probability-theory.md#conditional-distribution), not from an unrelated unconditional distribution.

## 3

↑ **Parent:** [Paper 38](paper-38.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Write the [discount factor](../../../mathematical-finance.md#discount-factor) as $D_t=B_t^{-1}=\exp(-\int_0^t r_sds)$. Splitting the time integral at $t$ gives

$$
\frac{P(t,T)}{B_t}
=\mathbb E^{\mathbb Q}[D_T\mid\mathcal F_t].
$$

The random variable $D_T$ lies in $(0,1]$ because the [short rate](../../../mathematical-finance.md#short-rate) is nonnegative and continuous on the finite maturity interval. A process of [conditional expectations](../../../measure-theory.md#conditional-expectation) of an [integrable](../../../measure-theory.md#integrability) terminal variable is a [martingale](../../../martingale.md), by the [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation). Therefore

$$
\boxed{D_tP(t,T)\text{ is a bounded }\mathbb Q\text{-martingale}.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The terminal density is strictly positive and has [expectation](../../../probability-theory.md#expected-value) one under the usual deterministic initial bond-price convention. Its density process is

$$
Z_t=\mathbb E^{\mathbb Q}\left[\frac{D_T}{P(0,T)}\,\middle|\,\mathcal F_t\right]
=\frac{D_tP(t,T)}{P(0,T)}.
$$

For $0\leq s\leq t\leq T$, the [Bayes formula for conditional expectation](../../../probability-theory.md#bayes-formula-for-conditional-expectation) under a change of measure gives

$$
\begin{aligned}
\mathbb E^{\mathbb Q_T}\left[\frac{B_t}{P(t,T)}\,\middle|\,\mathcal F_s\right]
&=\frac1{Z_s}\mathbb E^{\mathbb Q}\left[Z_t\frac{B_t}{P(t,T)}\,\middle|\,\mathcal F_s\right]\\
&=\frac1{Z_sP(0,T)}=\frac{B_s}{P(s,T)}.
\end{aligned}
$$

The same calculation at $s=0$ gives the finite [expectation](../../../probability-theory.md#expected-value) $1/P(0,T)$, so this is a true [martingale](../../../martingale.md), not just a formal conditional identity. Thus **the [continuous-time bank account](../../../mathematical-finance.md#continuous-time-bank-account) measured in units of the maturity-$T$ bond is a $\mathbb Q_T$-[martingale](../../../martingale.md)**. This is the [forward measure](../../../mathematical-finance.md#forward-measure) change of [numéraire](../../../mathematical-finance.md#numeraire). If the initial bond price were random rather than given, [integrability](../../../measure-theory.md#integrability) of its reciprocal would need to be included for this true-martingale assertion.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

To avoid confusing the [continuous-time bank account](../../../mathematical-finance.md#continuous-time-bank-account) with the coefficient of $r_t$, denote the latter by $b(\tau)$ and the other coefficient by $a(\tau)$, where $\tau=T-t$. Apply the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $D_t[a(\tau)+b(\tau)r_t]$. Since the expression is affine in $r$, its second rate derivative is zero. Its drift is

$$
D_t\left[-a'(\tau)-b'(\tau)r_t+b(\tau)r_t(r_t-1)
-r_t(a(\tau)+b(\tau)r_t)\right]dt.
$$

The quadratic terms cancel. The remaining expression is

$$
D_t\{-a'(\tau)+[-b'(\tau)-a(\tau)-b(\tau)]r_t\}\,dt.
$$

It vanishes when $a'=0$ and $b'=-a-b$. For a unit bond payoff choose terminal conditions $a(0)=1$, $b(0)=0$, giving

$$
\boxed{a(\tau)=1,\qquad b(\tau)=e^{-\tau}-1.}
$$

The resulting [local martingale](../../../martingale.md#local-martingale) is $D_t[1-(1-e^{-\tau})r_t]$. The allowed bound $0\leq r_t\leq1$ puts it between zero and one, so the [bounded local martingale criterion](../../../martingale.md#bounded-local-martingale-criterion) makes it a true [martingale](../../../martingale.md). At maturity it equals $D_T$. Comparing with part (a) therefore gives

$$
\boxed{P(t,T)=1-(1-e^{-(T-t)})r_t.}
$$

In particular $e^{-(T-t)}\leq P(t,T)\leq1$, and $P(T,T)=1$. This is [linear bond pricing in a bounded short-rate diffusion](../../../mathematical-finance.md#linear-bond-pricing-in-a-bounded-short-rate-diffusion); choosing zero coefficients would produce a [local martingale](../../../martingale.md#local-martingale) but would not price the required terminal payoff.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Use the same affine drift cancellation with terminal conditions $a(0)=0$, $b(0)=1$. It gives $a(\tau)=0$, $b(\tau)=e^{-\tau}$, so

$$
D_te^{-(T-t)}r_t
=\mathbb E^{\mathbb Q}[D_Tr_T\mid\mathcal F_t].
$$

The process is bounded, which justifies the [conditional expectation](../../../measure-theory.md#conditional-expectation) identity. The [Bayes formula for conditional expectation](../../../probability-theory.md#bayes-formula-for-conditional-expectation) for the [forward measure](../../../mathematical-finance.md#forward-measure) now gives

$$
\begin{aligned}
\mathbb E^{\mathbb Q_T}[r_T\mid\mathcal F_t]
&=\frac{\mathbb E^{\mathbb Q}[D_Tr_T\mid\mathcal F_t]}
{\mathbb E^{\mathbb Q}[D_T\mid\mathcal F_t]}\\
&=\boxed{\frac{e^{-(T-t)}r_t}{1-(1-e^{-(T-t)})r_t}}.
\end{aligned}
$$

The denominator is positive; the ratio lies in $[0,1]$ and equals $r_T$ at maturity. This is the [forward-measure terminal rate in a linear bond model](../../../mathematical-finance.md#forward-measure-terminal-rate-in-a-linear-bond-model).

## 4

↑ **Parent:** [Paper 38](paper-38.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Buy one lower-strike [European call option](../../../mathematical-finance.md#european-call-option) and sell one higher-strike [European call option](../../../mathematical-finance.md#european-call-option). The initial cost is $C(K_i)-C(K_{i+1})<0$, so the strategy releases strictly positive cash. Its terminal payoff is

$$
(S_1-K_i)^+-(S_1-K_{i+1})^+\geq0
$$

for every [stock](../../../mathematical-finance.md#stock) price. Thus it is an [arbitrage](../../../mathematical-finance.md#arbitrage): a positive initial receipt accompanies a nonnegative terminal obligation. One may consume the receipt immediately, or hold it in cash to make a zero-initial-capital strategy with strictly positive terminal wealth. This is the [vertical-spread arbitrage for increasing call prices](../../../mathematical-finance.md#vertical-spread-arbitrage-for-increasing-call-prices).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Buy half a call at each neighboring strike and sell one call at the middle strike. Its cost is

$$
\frac12C(K_{i-1})+\frac12C(K_{i+1})-C(K_i)<0.
$$

For fixed terminal [stock](../../../mathematical-finance.md#stock) price $s$, the function $K\mapsto(s-K)^+$ is [convex](../../../real-analysis.md#convex-function). Since $K_i$ is the midpoint, the payoff

$$
\frac12(s-K_{i-1})^++\frac12(s-K_{i+1})^+-(s-K_i)^+
$$

is nonnegative for every $s$. More explicitly, it is zero outside $[K_{i-1},K_{i+1}]$, equals $(s-K_{i-1})/2$ on $[K_{i-1},K_i]$, and equals $(K_{i+1}-s)/2$ on $[K_i,K_{i+1}]$. The negative cost and nonnegative payoff produce an [arbitrage](../../../mathematical-finance.md#arbitrage). This is the [butterfly-spread arbitrage for nonconvex call prices](../../../mathematical-finance.md#butterfly-spread-arbitrage-for-nonconvex-call-prices).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Use positive strikes, the natural real-power domain of this price curve. For any such $K$, the stock-minus-call payoff is

$$
S_1-(S_1-K)^+=\min(S_1,K)>0
$$

almost surely, since $S_1>0$. Therefore the call price must be strictly below the [stock](../../../mathematical-finance.md#stock) price $S_0=1$: if $C(K)\geq1$, buying [stock](../../../mathematical-finance.md#stock) and selling the call has nonpositive initial cost and strictly positive terminal payoff. Also a negative call price is an immediate [arbitrage](../../../mathematical-finance.md#arbitrage) by buying the call.

For $p<0$, $1+K^p>K^p$ and raising to the negative power $1/p$ reverses the inequality, giving $(1+K^p)^{1/p}<K$ and $C(K)<0$. The expression is undefined at $p=0$. For $0<p<1$, strict [concavity](../../../real-analysis.md#concave-function) of the power implies $(1+K)^p<1+K^p$, whence

$$
C(K)=(1+K^p)^{1/p}-K>1.
$$

At $p=1$, $C(K)=1$. Every defined case with $p\leq1$ therefore violates the necessary no-arbitrage bounds. Consequently

$$
\boxed{p>1.}
$$

This argument does not require a dense family of strikes; even one positive-strike call gives the contradiction. The strict stock-minus-call payoff explains why the borderline $p=1$ is also excluded.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Use zero-interest cash as the one-period [numéraire](../../../mathematical-finance.md#numeraire), consistent with the stated expectation-price formula. For $p>1$, differentiate the proposed call-price curve twice. The first derivative and the candidate density are

$$
\begin{aligned}
C'(u)&=u^{p-1}(1+u^p)^{1/p-1}-1,\\
\boxed{f_p(u)=C''(u)}&=\boxed{(p-1)u^{p-2}(1+u^p)^{1/p-2},\qquad u>0.}
\end{aligned}
$$

This is the [power call-curve pricing density](../../../mathematical-finance.md#power-call-curve-pricing-density). It is strictly positive. Its integral is $C'(\infty)-C'(0+)=1$, and its survival function is $-C'(u)$. Since $C(0+)=1$ and $C(\infty)=0$,

$$
\int_0^\infty u f_p(u)\,du
=\int_0^\infty[-C'(u)]\,du=1.
$$

Likewise, integrating the survival function from $K$ onwards gives

$$
\int_0^\infty(u-K)^+f_p(u)\,du=C(K).
$$

Thus a market whose terminal [stock](../../../mathematical-finance.md#stock) has this law under an [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure) prices the [stock](../../../mathematical-finance.md#stock) at one, every proposed call at $C(K)$, and any [integrable](../../../measure-theory.md#integrability) claim $g(S_1)$ at $\int g(u)f_p(u)du$. The finite-market [fundamental theorem of asset pricing](../../../mathematical-finance.md#fundamental-theorem-of-asset-pricing) says that an equivalent measure pricing every traded discounted payoff by [expectation](../../../probability-theory.md#expected-value) excludes [arbitrage](../../../mathematical-finance.md#arbitrage). This proves the intended conclusion when such an equivalent pricing law is part of the model. For example, take the canonical terminal state space $(0,\infty)$ with [stock](../../../mathematical-finance.md#stock) equal to its coordinate and physical law equivalent to the positive density $f_p$.

There is, however, a genuine insufficiency in the literal finite-strike formulation: a finite list of call prices and no-arbitrage alone do not force this pricing law, nor even a continuous terminal distribution. Here is an explicit counterexample. Take $p=2$, one strike $K=1$, and two terminal [stock](../../../mathematical-finance.md#stock) values

$$
a=\frac12,\qquad b=2+\sqrt2,
\qquad\mathbb Q(S_1=b)=3-2\sqrt2.
$$

Give the lower [stock](../../../mathematical-finance.md#stock) value the remaining strictly positive probability and take this as the physical measure too. Direct calculation gives $\mathbb E S_1=1$ and

$$
\mathbb E(S_1-1)^+=\sqrt2-1=C(1),
$$

so the [stock](../../../mathematical-finance.md#stock)/cash/call market is arbitrage-free. Now let

$$
g(u)=(u-a)^2(u-b)^2e^{-u}.
$$

This bounded nonnegative function is zero at both actual [stock](../../../mathematical-finance.md#stock) values, so $g(S_1)=0$ almost surely. Yet $\int g(u)f_2(u)du>0$. Charging that positive amount for the identically zero payoff creates an [arbitrage](../../../mathematical-finance.md#arbitrage) by selling it. In fact no Lebesgue probability density can price every claim correctly on this two-state market.

Therefore **the displayed $f_p$ is the intended continuous pricing density, but the promised no-arbitrage extension requires an equivalent pricing measure with this terminal law; a full call curve identifies that law if such a measure exists, but it does not follow from the printed finite-strike hypotheses alone**. This is the [finite-strike nonidentification of a pricing density](../../../mathematical-finance.md#finite-strike-nonidentification-of-a-pricing-density). The counterexample and the corrected sufficient hypothesis account for the literal and intended readings separately.

## 5

↑ **Parent:** [Paper 38](paper-38.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Multiply the linear [stochastic differential equation](../../../stochastic-calculus.md#stochastic-differential-equation) by $e^{-at}$. The [Itô product rule](../../../stochastic-calculus.md#ito-product-rule) gives

$$
Z_t=e^{at}z+b\int_0^t e^{a(t-s)}\,dW_s.
$$

The integrand is deterministic, so the [Itô integral](../../../stochastic-calculus.md#ito-integral) has a centered [normal distribution](../../../probability-theory.md#normal-distribution). Its [variance](../../../variance.md), by the [Itô isometry](../../../stochastic-calculus.md#ito-isometry), is

$$
b^2\int_0^t e^{2a(t-s)}ds
=\begin{cases}\displaystyle\frac{b^2}{2a}(e^{2at}-1),&a\ne0,\\b^2t,&a=0.\end{cases}
$$

Hence

$$
\boxed{Z_t\sim N\left(e^{at}z,\frac{b^2}{2a}(e^{2at}-1)\right)\quad(a\ne0).}
$$

At $a=0$ the correct continuous-limit formula is $N(z,b^2t)$. A zero [variance](../../../variance.md), for example when $b=0$, denotes the deterministic distribution. For $a<0$ the [variance](../../../variance.md) is still positive because both numerator and denominator in its quotient are negative. This is the [explicit Ornstein-Uhlenbeck solution](../../../stochastic-process.md#explicit-ornstein-uhlenbeck-solution), allowing either sign of the linear drift coefficient.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Choose the [market price of risk](../../../mathematical-finance.md#market-price-of-risk) $\lambda_t=(\mu-rS_t)/\sigma$. The [Girsanov theorem](../../../stochastic-calculus.md#girsanov-theorem), with the hypotheses allowed in the question, gives an [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure) $\mathbb Q$ under which

$$
dW_t^{\mathbb Q}=dW_t+\lambda_tdt,\qquad
dS_t=rS_tdt+\sigma dW_t^{\mathbb Q}.
$$

Thus the [stock](../../../mathematical-finance.md#stock) under the [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure) is a linear [Gaussian](../../../probability-theory.md#normal-distribution) diffusion. In particular, for $\tau=T-t$ its conditional mean and standard deviation are

$$
m=e^{r\tau}S_t,\qquad
v=\sigma\sqrt{\frac{e^{2r\tau}-1}{2r}}.
$$

Put $\phi(x)=(2\pi)^{-1/2}e^{-x^2/2}$ and let $\Phi$ be the standard [normal distribution](../../../probability-theory.md#normal-distribution) function. For $N\sim N(0,1)$,

$$
\mathbb E(m+vN-K)^+=(m-K)\Phi((m-K)/v)+v\phi((m-K)/v),
$$

since $\int_{-d}^\infty x\phi(x)dx=\phi(d)$. Discounting this [expectation](../../../probability-theory.md#expected-value) gives the [call price in an arithmetic stock model with interest](../../../mathematical-finance.md#call-price-in-an-arithmetic-stock-model-with-interest). A particularly convenient expression is

$$
\begin{aligned}
\nu(\tau)&=\sigma\sqrt{\frac{1-e^{-2r\tau}}{2r}},
&d(t,s)&=\frac{s-Ke^{-r\tau}}{\nu(\tau)},\\
\boxed{C(t,s)}&=\boxed{(s-Ke^{-r\tau})\Phi(d(t,s))+\nu(\tau)\phi(d(t,s))}.
\end{aligned}
$$

At maturity define $C(T,s)=(s-K)^+$. This value is nonnegative because it is a discounted [expectation](../../../probability-theory.md#expected-value) of a nonnegative payoff.

For $t<T$, hold $\pi_t=C_s(t,S_t)$ shares and hold $\beta_t=[C(t,S_t)-\pi_tS_t]/B_t$ units of the [continuous-time bank account](../../../mathematical-finance.md#continuous-time-bank-account). The pricing function solves

$$
C_t+rsC_s+\tfrac12\sigma^2C_{ss}-rC=0.
$$

The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) under the physical measure therefore gives

$$
dC(t,S_t)=C_s(t,S_t)dS_t+r[C(t,S_t)-S_tC_s(t,S_t)]dt
=\pi_t dS_t+\beta_t dB_t.
$$

This proves [self-financing](../../../mathematical-finance.md#self-financing-portfolio) and terminal replication, with wealth always $C(t,S_t)\geq0$. The coefficients are locally smooth before maturity, and the strategy extends to maturity through its continuous wealth limit and the square-integrable discounted payoff representation.

To see minimality, any other nonnegative [self-financing portfolio](../../../mathematical-finance.md#self-financing-portfolio) replicating the payoff has discounted wealth a nonnegative [local martingale](../../../martingale.md#local-martingale) under $\mathbb Q$, hence a [supermartingale](../../../martingale.md#supermartingale). Its initial capital $x$ must satisfy $x\geq\mathbb E^{\mathbb Q}[e^{-rT}(S_T-K)^+]=C(0,S_0)$. The strategy constructed above attains equality. Thus

$$
\boxed{x_{\min}=C(0,S_0).}
$$

The additive physical diffusion may take negative [stock](../../../mathematical-finance.md#stock) values; the formula and nonnegative replicating wealth remain valid. Replacing it by a multiplicative Black–Scholes diffusion would give the wrong price and hedge.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Differentiate the [Gaussian](../../../probability-theory.md#normal-distribution) price with respect to $s$. The terms involving derivatives of $d$ cancel because $\phi'(d)=-d\phi(d)$ and $s-Ke^{-r\tau}=\nu d$. Thus the [delta hedge](../../../mathematical-finance.md#delta-hedge) is

$$
\boxed{\pi_t=C_s(t,S_t)=\Phi\left(\frac{S_t-Ke^{-r(T-t)}}{
\sigma\sqrt{(1-e^{-2r(T-t)})/(2r)}}\right).}
$$

For every $t<T$, $\nu>0$ and $S_t$ is finite, so $0<\pi_t<1$. At maturity its limiting value is the payoff derivative $\mathbf1_{\{S_T>K\}}$ except at the kink, an event of probability zero under the equivalent [Gaussian](../../../probability-theory.md#normal-distribution) law. Consequently **the [stock](../../../mathematical-finance.md#stock) holding is always nonnegative and never exceeds one**. The initial drift $\mu$ does not enter this hedge; it is removed by the change to the [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure).

## 6

↑ **Parent:** [Paper 38](paper-38.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

The mark-to-market value of holdings $H_t$ in the asset-price vector is the [dot product](../../../linear-algebra.md#dot-product) $X_t=H_t\cdot P_t$. A [self-financing strategy](../../../mathematical-finance.md#self-financing-portfolio) pays for every rebalancing from within the [portfolio](../../../mathematical-finance.md#investment-portfolio). Over a short interval, the gains on the currently held assets are $H_t\cdot dP_t$, while [consumption](../../../mathematical-finance.md#consumption) removes $c_tdt$ units of wealth. Therefore

$$
\boxed{X_t=H_t\cdot P_t,\qquad dX_t=H_t\cdot dP_t-c_tdt.}
$$

The holdings are [predictable](../../../martingale.md#predictable-process) and [integrable](../../../measure-theory.md#integrability) against the price [semimartingale](../../../stochastic-calculus.md#semimartingale); the [consumption](../../../mathematical-finance.md#consumption) rate is nonnegative and suitably measurable. This is the continuous-time self-financing-with-consumption convention.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Use the [state-price density](../../../mathematical-finance.md#state-price-density) as a positive [local martingale deflator](../../../mathematical-finance.md#local-martingale-deflator), so each component of $YP$ is a [local martingale](../../../martingale.md#local-martingale). The [Itô product rule](../../../stochastic-calculus.md#ito-product-rule) and the wealth equation give

$$
d(YX)=YH\cdot dP-Yc\,dt+X\,dY+d[Y,X].
$$

The [consumption](../../../mathematical-finance.md#consumption) term has [finite variation](../../../real-analysis.md#total-variation-of-a-function), and the [quadratic covariation](../../../stochastic-calculus.md#quadratic-covariation) of a [stochastic integral](../../../stochastic-calculus.md#stochastic-integral) satisfies $d[Y,X]=H\cdot d[Y,P]$. Also $X=H\cdot P$. Regrouping the terms therefore gives

$$
\boxed{d(Y_tX_t)=H_t\cdot d(Y_tP_t)-Y_tc_t\,dt.}
$$

The differential before $YP$ is necessary: the first term is a stochastic gain, not the level of the deflated [portfolio](../../../mathematical-finance.md#investment-portfolio). It is missing in the printed display. This is the [deflated wealth equation with consumption](../../../mathematical-finance.md#deflated-wealth-equation-with-consumption).

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

The integral against the local-martingale vector $YP$ is a [local martingale](../../../martingale.md#local-martingale), provided the [predictable](../../../martingale.md#predictable-process) holdings are stochastically [integrable](../../../measure-theory.md#integrability). Integrating part (b) gives

$$
M_t=Y_tX_t-Y_0X_0+\int_0^tY_sc_sds.
$$

Both $Y_tX_t$ and the cumulative deflated [consumption](../../../mathematical-finance.md#consumption) are nonnegative. Hence $M_t\geq-Y_0X_0$. With the usual finite deterministic initial capital, the shifted process

$$
M_t+Y_0X_0=Y_tX_t+\int_0^tY_sc_sds
$$

is a nonnegative [local martingale](../../../martingale.md#local-martingale), and is therefore a [supermartingale](../../../martingale.md#supermartingale). For completeness, a [localizing sequence](../../../martingale.md#localizing-sequence) turns it into true [martingales](../../../martingale.md); conditional [Fatou lemma](../../../measure-theory.md#fatou-s-lemma) for their nonnegative stopped values gives the [supermartingale](../../../martingale.md#supermartingale) inequality and ordinary Fatou gives [integrability](../../../measure-theory.md#integrability) at each time. Subtracting the initial constant proves

$$
\boxed{M\text{ is a supermartingale with }M_0=0.}
$$

This is [supermartingale control of deflated consumption gains](../../../mathematical-finance.md#supermartingale-control-of-deflated-consumption-gains). It uses $c\geq0$ as well as $X\geq0$; an unrestricted [stochastic integral](../../../stochastic-calculus.md#stochastic-integral) is not necessarily a true [supermartingale](../../../martingale.md#supermartingale).

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

Part (c) gives $\mathbb E M_t\leq0$. Since $Y_tX_t\geq0$, its integrated identity implies

$$
\mathbb E\int_0^tY_sc_sds\leq Y_0X_0
$$

for every finite $t$. The cumulative [consumption](../../../mathematical-finance.md#consumption) increases with $t$, so the [monotone convergence theorem](../../../measure-theory.md#monotone-convergence-theorem) yields

$$
\boxed{\mathbb E\int_0^\infty Y_tc_tdt\leq Y_0X_0.}
$$

This is the infinite-horizon [state-price budget constraint](../../../mathematical-finance.md#state-price-budget-constraint). No terminal-wealth convergence or vanishing assumption is needed for this inequality.

<h3 id="6/e">e</h3>

↑ **Parent:** [6](#6)

<h4 id="6/e/solution">Solution</h4>

↑ **Parent:** [E](#6/e)

[Concavity](../../../real-analysis.md#concave-function) gives the supporting-tangent inequality

$$
U(\hat c_t)-U(c_t)\leq U'(c_t)(\hat c_t-c_t).
$$

Multiply by the [discount factor](../../../mathematical-finance.md#discount-factor) $e^{-bt}$ and use the first-order condition $e^{-bt}U'(c_t)=Y_t$. This gives the pointwise [marginal-utility verification of optimal consumption](../../../utility-function.md#marginal-utility-verification-of-optimal-consumption) inequality

$$
e^{-bt}[U(\hat c_t)-U(c_t)]\leq Y_t(\hat c_t-c_t).
$$

Apply the budget inequality from part (d) to the competing admissible strategy, and use equality for the proposed one:

$$
\mathbb E\int_0^\infty Y_t\hat c_tdt\leq Y_0X_0
=\mathbb E\int_0^\infty Y_tc_tdt.
$$

The two weighted [consumption](../../../mathematical-finance.md#consumption) integrals are finite, so their difference is [integrable](../../../measure-theory.md#integrability). Under the usual positive discount-rate assumption $b>0$, the utility integrals are also [integrable](../../../measure-theory.md#integrability): $U(0)\leq U(x)\leq L$ for a finite upper bound $L$, and $\int_0^\infty e^{-bt}dt=1/b$. Integrating the tangent inequality and taking [expectations](../../../probability-theory.md#expected-value) therefore gives

$$
\boxed{\mathbb E\int_0^\infty e^{-bt}U(c_t)dt
\geq\mathbb E\int_0^\infty e^{-bt}U(\hat c_t)dt.}
$$

Economically, both consumers face the same state-price budget, and the candidate spends it exactly where its discounted marginal utility equals the state price. This is [utility duality with martingale deflators](../../../utility-function.md#utility-duality-with-martingale-deflators) in its [consumption](../../../mathematical-finance.md#consumption) form.

A positive $b$, or another hypothesis making the infinite-horizon objectives well defined and permitting this integration, is needed. The printed question does not specify the sign of $b$. Bounded utility alone does not ensure that an undiscounted infinite time integral exists: a bounded integrand can have both infinite positive and negative parts. Thus the conclusion is established under the standard discount convention $b>0$, and also whenever the displayed objectives satisfy the stated [integrability](../../../measure-theory.md#integrability) conditions; without either convention the literal infinite-horizon comparison need not be a defined mathematical expression.

This can occur within an admissible financial model, not just for an abstract bounded integrand. Take $U(x)=1-2e^{-x}$ and $b=0$. Choose a deterministic smooth nonnegative $c$ with successive unit-length plateaus alternating between zero and the integer $n$, and connect them over intervals whose lengths have finite sum. Then $\int_0^\infty2c_te^{-c_t}dt<\infty$: the high-plateau contributions sum to $\sum_{n\geq1}2ne^{-n}$ and the transition integrand is bounded by $2/e$. Set

$$
Y_t=2e^{-c_t},\qquad B_t=Y_0/Y_t,\qquad
X_t=\frac1{Y_t}\int_t^\infty Y_sc_sds.
$$

The bank account is a positive deterministic [Itô process](../../../stochastic-calculus.md#ito-process) and $Y_tB_t=Y_0$, so $Y$ is a [state-price density](../../../mathematical-finance.md#state-price-density). Holding $X_t/B_t$ bank units finances consumption with nonnegative wealth and exact budget equality. Also $U'(c_t)=Y_t$. Nevertheless every zero plateau contributes $-1$ to the utility integral, while each sufficiently high plateau contributes a fixed positive amount. Both its negative and positive parts are infinite, so the undiscounted objective is undefined. This establishes why the missing discount or objective-integrability hypothesis is substantive.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
