# Paper 39

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper39.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper39.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
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

## 1

↑ **Parent:** [Paper 39](paper-39.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For the [autoregressive process of order one](../../../time-series.md#autoregressive-process-of-order-one), the formula at $t=0$ reads $r_0=r_0$, with an empty sum. If it holds at time $t$, substitution into the recursion gives

$$
r_{t+1}=\beta\left(\beta^tr_0+\sum_{s=1}^t\beta^{t-s}\xi_s\right)+\xi_{t+1}
=\beta^{t+1}r_0+\sum_{s=1}^{t+1}\beta^{t+1-s}\xi_s.
$$

Thus [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) proves

$$
\boxed{r_t=\beta^tr_0+\sum_{s=1}^t\beta^{t-s}\xi_s.}
$$

No restriction such as $|\beta|<1$ is needed for this finite-time identity.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Put $n=T-t$ and define the finite [geometric series](../../../real-analysis.md#geometric-series)

$$
A_0=0,\qquad A_j=\sum_{k=0}^{j-1}\beta^k
=\begin{cases}(1-\beta^j)/(1-\beta),&\beta\ne1,\\j,&\beta=1.\end{cases}
$$

Starting the [autoregressive process of order one](../../../time-series.md#autoregressive-process-of-order-one) at time $t$ gives $r_{t+k}=\beta^kr_t+\sum_{j=1}^k\beta^{k-j}\xi_{t+j}$. Consequently

$$
\sum_{k=1}^n r_{t+k}=\beta A_nr_t+\sum_{j=1}^nA_{n-j+1}\xi_{t+j},\qquad
\frac{B_t}{B_T}=\exp\left(-\sum_{k=1}^nr_{t+k}\right).
$$

The future innovations are [independent and identically distributed random variables](../../../random-variable.md#independent-and-identically-distributed-random-variables), independent of $\mathcal F_t$. Factorizing their exponential [conditional expectation](../../../measure-theory.md#conditional-expectation) and using the [cumulant-generating function](../../../probability-theory.md#cumulant-generating-function) $K$ yields

$$
P(t,T)=e^{-\beta A_nr_t}\prod_{j=1}^n\mathbb E[e^{-A_{n-j+1}\xi_1}]
=\exp\left(-\beta A_nr_t+\sum_{j=1}^nK(-A_j)\right).
$$

Thus the [exponential-affine bond pricing](../../../mathematical-finance.md#exponential-affine-bond-pricing) coefficients are

$$
\boxed{Q(t,T)=-\beta A_{T-t},\qquad R(t,T)=\sum_{j=1}^{T-t}K(-A_j).}
$$

They vanish at maturity, giving $P(T,T)=1$. Everywhere finiteness of $K$ ensures that each [zero-coupon bond](../../../mathematical-finance.md#zero-coupon-bond) price is positive and finite, including when $\beta$ is zero, negative, or one.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $q(T)$ denote the original [zero-coupon bond](../../../mathematical-finance.md#zero-coupon-bond) price $P(0,T)$ computed above. A deterministic shift $h_t$ of the [short rate](../../../mathematical-finance.md#short-rate), with $h_0=0$, gives $\widehat r_t=r_t+h_t$. Subtracting the two recursions shows that the required added drift is

$$
\alpha_t=h_t-\beta h_{t-1}.
$$

Since the shift is nonrandom, the new [discount factor](../../../mathematical-finance.md#discount-factor) differs by $\exp(-\sum_{s=1}^Th_s)$, and hence $\widehat P(0,T)=q(T)\exp(-\sum_{s=1}^Th_s)$.

For [deterministic calibration of an autoregressive short rate](../../../mathematical-finance.md#deterministic-calibration-of-an-autoregressive-short-rate), define

$$
d_T=\log q(T)-\log p(T),\qquad d_0=0,\qquad h_T=d_T-d_{T-1}\quad(T\geq1).
$$

All these quantities are finite. The telescoping sum $\sum_{s=1}^Th_s=d_T$ gives $\widehat P(0,T)=p(T)$. Explicitly,

$$
\boxed{\alpha_1=d_1,\qquad
\alpha_T=d_T-(1+\beta)d_{T-1}+\beta d_{T-2}\quad(T\geq2).}
$$

These constants fit every maturity simultaneously. Each successive maturity fixes $h_T$ uniquely, so the deterministic calibration is also unique with the prescribed $r_0$.

## 2

↑ **Parent:** [Paper 39](paper-39.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The square root is concave on $[0,\infty)$, and $\sqrt{S_T}$ is [integrable](../../../measure-theory.md#integrability) since $\mathbb E\sqrt{S_T}\leq\sqrt{\mathbb ES_T}$. For $t\leq T_1\leq T_2$, the [conditional Jensen inequality](../../../measure-theory.md#conditional-jensen-inequality) and the [martingale](../../../martingale.md) property give

$$
\mathbb E[\sqrt{S_{T_2}}\mid\mathcal F_{T_1}]
\leq\sqrt{\mathbb E[S_{T_2}\mid\mathcal F_{T_1}]}
=\sqrt{S_{T_1}}.
$$

Taking [conditional expectations](../../../measure-theory.md#conditional-expectation) with respect to $\mathcal F_t$ and using the [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation) yields

$$
\boxed{C(t,T_2)\leq C(t,T_1)\quad\text{almost surely}.}
$$

Thus the maturity curve for a [square-root stock claim](../../../mathematical-finance.md#square-root-stock-claim) is nonincreasing; it need not be strictly decreasing, as a constant stock gives equality. The inequality holds for every ordered pair of maturities. Under the usual right-continuous versions of the market processes, it gives the corresponding nonincreasing version of the maturity curve.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Solving the [geometric Brownian motion](../../../stochastic-calculus.md#geometric-brownian-motion) equation over $[t,T]$ gives

$$
S_T=S_t\exp\left(\sigma_0(W_T-W_t)-\frac12\sigma_0^2(T-t)\right).
$$

The [Brownian increment](../../../brownian-motion.md#brownian-increment) is independent of $\mathcal F_t$ and has a [normal distribution](../../../probability-theory.md#normal-distribution) with variance $T-t$. Its exponential [moment-generating function](../../../probability-theory.md#moment-generating-function) therefore gives

$$
C(t,T)=\sqrt{S_t}\,e^{-\sigma_0^2(T-t)/4}
\mathbb E\left[e^{\sigma_0(W_T-W_t)/2}\mid\mathcal F_t\right]
=\sqrt{S_t}\,e^{-\sigma_0^2(T-t)/8}.
$$

The required deterministic price function is

$$
\boxed{F(t,T,s,v)=\sqrt{s}\exp\left(-\frac18v^2(T-t)\right).}
$$

This includes $s=0$, $v=0$ and $t=T$. For $s>0$ and $t<T$, it is continuous and strictly decreasing in $v\geq0$, with range $(0,\sqrt{s}]$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $\tau=T-t>0$ and $I_{t,T}=\int_t^T\sigma_s^2ds$. The [stochastic exponential](../../../stochastic-calculus.md#doleans-dade-exponential) solution gives

$$
\sqrt{S_T}=\sqrt{S_t}\,M_{t,T}e^{-I_{t,T}/8},\qquad
M_{t,T}=\exp\left(\frac12\int_t^T\sigma_s\,dW_s-\frac18 I_{t,T}\right).
$$

Boundedness of the [predictable process](../../../martingale.md#predictable-process) $\sigma$ implies the [Novikov condition](../../../stochastic-calculus.md#novikov-s-condition) on every finite horizon, so this exponential has [conditional expectation](../../../measure-theory.md#conditional-expectation) $\mathbb E[M_{t,T}\mid\mathcal F_t]=1$. The pathwise bounds $a^2\tau\leq I_{t,T}\leq b^2\tau$ and positivity of $M_{t,T}$ give

$$
\sqrt{S_t}\,e^{-b^2\tau/8}
\leq C(t,T)\leq\sqrt{S_t}\,e^{-a^2\tau/8}.
$$

This proves the required bound in the independent-volatility case, and the exponential argument in fact does not need independence. In the usual filtration generated by [Brownian motion](../../../brownian-motion.md) and an independent volatility history, one can alternatively condition on the whole volatility path: the Brownian integral is then conditionally Gaussian with variance $I_{t,T}$. The result is

$$
C(t,T)=\sqrt{S_t}\,\mathbb E[e^{-I_{t,T}/8}\mid\mathcal F_t],
$$

the [conditional square-root price under independent volatility](../../../mathematical-finance.md#conditional-square-root-price-under-independent-volatility). The outer conditional expectation cannot in general be removed.

On $\{S_t>0\}$, these positive price bounds justify the unique [square-root stock implied volatility](../../../mathematical-finance.md#square-root-stock-implied-volatility)

$$
\Sigma(t,T)^2=-\frac8\tau\log\left(\frac{C(t,T)}{\sqrt{S_t}}\right),
\qquad\boxed{a\leq\Sigma(t,T)\leq b.}
$$

There is a genuine zero-price qualification: if $S_t=0$, the nonnegative stock is absorbed at zero and both claim prices are zero for every volatility parameter. The price equation then does not determine a unique $\Sigma$. One may set $\Sigma=a$ on that event to retain the bounds; identification by inversion requires $S_t>0$.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Fix the horizon $T$ and define the [half-volatility measure for a square-root stock claim](../../../mathematical-finance.md#half-volatility-measure-for-a-square-root-stock-claim) by

$$
Z_s=\exp\left(\frac12\int_0^s\sigma_u\,dW_u-\frac18\int_0^s\sigma_u^2du\right),\qquad
\frac{dQ}{dP}\bigg|_{\mathcal F_T}=Z_T.
$$

The [Novikov condition](../../../stochastic-calculus.md#novikov-s-condition) makes $Z$ a true [martingale](../../../martingale.md) with $\mathbb EZ_T=1$, and $Z_T>0$ makes $Q$ equivalent to $P$. The [Girsanov theorem](../../../stochastic-calculus.md#girsanov-theorem) identifies $W_s^Q=W_s-\frac12\int_0^s\sigma_u du$ as a [Brownian motion](../../../brownian-motion.md) under $Q$.

The exact factorization from the previous part is

$$
\sqrt{S_T}=\sqrt{S_t}\,\frac{Z_T}{Z_t}e^{-I_{t,T}/8}.
$$

Using the [Bayes formula for conditional expectation](../../../probability-theory.md#bayes-formula-for-conditional-expectation) therefore gives

$$
\boxed{C(t,T)=\sqrt{S_t}\,\mathbb E_Q[e^{-I_{t,T}/8}\mid\mathcal F_t].}
$$

The random integrated variance need not have any independence property under $Q$. Its pathwise bounds still imply $e^{-b^2\tau/8}\leq\mathbb E_Q[e^{-I_{t,T}/8}\mid\mathcal F_t]\leq e^{-a^2\tau/8}$. Inverting the same price function proves **$a\leq\Sigma(t,T)\leq b$ even for volatility adapted to the Brownian motion**, on the positive-price event. The zero-price convention is as above. The auxiliary measure here is not asserted to be an [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure) for the stock.

## 3

↑ **Parent:** [Paper 39](paper-39.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Backward induction first proves that the [Snell envelope](../../../martingale.md#snell-envelope) is [adapted](../../../stochastic-process.md#adapted-process) and [integrable](../../../measure-theory.md#integrability). At each step, $|U_t|\leq|Y_t|+\mathbb E[|U_{t+1}|\mid\mathcal F_t]$, so integrability follows from that of $Y_t$ and $U_{t+1}$. Its defining maximum immediately gives

$$
\mathbb E[U_{t+1}\mid\mathcal F_t]\leq U_t,
$$

which proves that **$U$ is a supermartingale**.

If $Y$ is a [submartingale](../../../martingale.md#submartingale), the sharper backward identity is

$$
\boxed{U_t=\mathbb E[Y_T\mid\mathcal F_t].}
$$

It holds at $T$. If it holds at $t+1$, the [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation) gives $\mathbb E[U_{t+1}\mid\mathcal F_t]=\mathbb E[Y_T\mid\mathcal F_t]$. Iterating the submartingale inequalities shows that this is at least $Y_t$, so the maximum chooses this continuation value. The displayed identity then makes $U$ a [martingale](../../../martingale.md).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $\nu$ be the common increment law. The [random walk](../../../markov-process.md#random-walk) has the [Markov property](../../../markov-process.md#markov-property), since $\xi_{t+1}$ is independent of $\mathcal F_t$ and $X_{t+1}=X_t+\xi_{t+1}$. Its [transition operator](../../../markov-process.md#transition-operator) is $Ph(x)=\int h(x+z)\nu(dz)$ wherever that integral exists.

Set $V(T,x)=f(x)$. For $1\leq t<T$, suppose the Borel function $V(t+1,\cdot)$ has been constructed and represents $U_{t+1}$. On the Borel set

$$
A_t=\left\{x:\int|V(t+1,x+z)|\nu(dz)<\infty\right\},
$$

define the [optimal stopping value function](../../../martingale.md#optimal-stopping-value-function) recursively by

$$
V(t,x)=\max\left\{f(x),\int V(t+1,x+z)\nu(dz)\right\}.
$$

Outside $A_t$, assign the finite Borel value $f(x)$. Measurability of integrals against a fixed probability law proves measurability of both the set and the function. Integrability of $U_{t+1}=V(t+1,X_t+\xi_{t+1})$ and independence imply $X_t\in A_t$ almost surely and

$$
\mathbb E[U_{t+1}\mid\mathcal F_t]
=\int V(t+1,X_t+z)\nu(dz).
$$

The Snell recursion thus proves $U_t=V(t,X_t)$ by induction.

At time zero the generated [sigma-algebra](../../../measure-theory.md#sigma-algebra) is trivial, so $U_0$ is deterministic. Since $X_0=0$, define $V(0,x)=U_0$ for all $x$, with

$$
U_0=\max\{f(0),\mathbb E[V(1,\xi_1)]\}
$$

when $T\geq1$. This supplies a globally finite deterministic representation without assuming integrability of rewards from every unvisited starting state. Hence

$$
\boxed{U_t=V(t,X_t)\quad(0\leq t\leq T).}
$$

With the additional statewise integrability normally used to define a value function for arbitrary starting states, one can instead use the Bellman maximum at time zero too. For $T=0$, the representation is simply $U_0=f(0)$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The key [convexity](../../../real-analysis.md#convex-function) calculation is that the random-walk [transition operator](../../../markov-process.md#transition-operator) preserves [convex functions](../../../real-analysis.md#convex-function). If $h$ is convex, then for $0<\theta<1$,

$$
Ph(\theta x+(1-\theta)y)
=\mathbb E[h(\theta(x+\xi)+(1-\theta)(y+\xi))]
\leq\theta Ph(x)+(1-\theta)Ph(y).
$$

The [pointwise maximum of convex functions](../../../real-analysis.md#pointwise-maximum-of-convex-functions) is convex as well: the convexity inequality holds for each candidate and is bounded above by the convex combination of the two endpoint maxima. Thus the Bellman recursion proves [convexity of a random-walk Snell value function](../../../martingale.md#convexity-of-a-random-walk-snell-value-function) by backward induction from $V(T,\cdot)=f$.

To ensure that the functions in this argument are genuinely finite, rather than silently imposing a growth bound on $f$, use [integrability of translated convex random-walk rewards](../../../martingale.md#integrability-of-translated-convex-random-walk-rewards). Write $Z_j$ for a sum of $j$ independent increments with the same law. For $j\leq T-1$, the assumptions give integrability of $f(Z_j)$ and $f(Z_{j+1})$. The [negative part of a finite convex function is Lipschitz](../../../real-analysis.md#negative-part-of-a-finite-convex-function-is-lipschitz), so translating $Z_j$ preserves integrability of the negative part. For the positive part and $x>0$, if the increment law is unbounded above, take an independent increment $\eta$ and $p=\mathbb P(\eta\geq x)>0$. On that event $Z_j+x$ lies between $Z_j$ and $Z_j+\eta$, so convexity gives

$$
p\,\mathbb E[f(Z_j+x)^+]
\leq p\,\mathbb E[f(Z_j)^+]+\mathbb E[f(Z_{j+1})^+]<\infty.
$$

If increments are bounded above by $M$, then $Z_j\leq jM$ and the same convexity argument between $Z_j$ and $jM+x$ bounds the positive part by $f(Z_j)^++f(jM+x)^+$. For $x<0$, use the corresponding lower-tail argument. Thus every translated reward $f(x+Z_j)$ is integrable for $j\leq T-1$.

For $t\geq1$, backward induction also gives the bound

$$
f(x)\leq V(t,x)\leq\sum_{j=0}^{T-t}\mathbb E[f(x+Z_j)^+]<\infty.
$$

It justifies every convolution in the Bellman recursion at these times, so the arbitrary assignments outside $A_t$ in the previous part are never needed when $f$ is convex. The displayed convexity calculation therefore proves that each $V(t,\cdot)$ for $t\geq1$ is a finite convex function. The chosen $V(0,\cdot)=U_0$ is constant and hence convex. This proves the requested conclusion for the deterministic representation under the finite-horizon assumptions.

There is a distinction between this representation and a value function for every possible starting point at time zero. Without translated integrability at the full horizon, the latter may take $+\infty$ at unused states. For example, with $T=1$, $f(x)=e^{x^2}$ and $\mathbb P(\xi_1=k)=c e^{-k^2-k}$ for $k=1,2,\ldots$, the observed reward is integrable, but $\mathbb E[f(x+\xi_1)]=c e^{x^2}\sum_{k\geq1}e^{(2x-1)k}$ is infinite for $x\geq1/2$. The constant time-zero extension avoids claiming a globally finite Bellman function under insufficient assumptions. If integrability is assumed for all times of an infinite random walk, the translated-reward argument with one extra time also makes the full time-zero Bellman function finite and convex.

## 4

↑ **Parent:** [Paper 39](paper-39.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

On a fixed horizon $T$, an [arbitrage](../../../mathematical-finance.md#arbitrage) is an [admissible trading strategy](../../../mathematical-finance.md#admissible-trading-strategy) that is [self-financing](../../../mathematical-finance.md#self-financing-portfolio), has $X_0=0$, and satisfies $X_T\geq0$ almost surely with $\mathbb P(X_T>0)>0$. Here admissibility means that wealth in units of the strictly positive riskless [numéraire](../../../mathematical-finance.md#numeraire) has a deterministic lower bound throughout the horizon. An [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure) $Q$ is equivalent to the physical measure on $\mathcal F_T$ and makes each discounted risky price $\widetilde S^i=S^i/B$ a [martingale](../../../martingale.md).

For a predictable, stochastically integrable risky holding vector $\pi$, the discounted self-financing identity is

$$
\widetilde X_t:=\frac{X_t}{B_t}
=\frac{X_0}{B_0}+\int_0^t\pi_s\cdot d\widetilde S_s.
$$

Indeed, since the riskless account is a [finite-variation process](../../../stochastic-calculus.md#finite-variation-process), its quadratic covariations vanish, and the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) for $X/B$, combined with $X=\phi B+\pi\cdot S$ and $dX=\phi\,dB+\pi\cdot dS$, gives $d(X/B)=\pi\cdot d(S/B)$.

Use two standard facts from [stochastic calculus](../../../stochastic-calculus.md): a stochastic integral against a continuous local martingale is a [local martingale](../../../martingale.md#local-martingale), and a local martingale bounded below by a deterministic constant is a [supermartingale](../../../martingale.md#supermartingale). The latter follows by adding the constant to make the process nonnegative, stopping at a localizing sequence, and applying the conditional [Fatou lemma](../../../measure-theory.md#fatou-s-lemma). Thus admissible discounted wealth is a $Q$-supermartingale, and an arbitrage would satisfy

$$
0\leq\mathbb E_Q[\widetilde X_T]\leq\widetilde X_0=0.
$$

It follows that $X_T=0$ $Q$-almost surely, hence also physically almost surely by equivalence, a contradiction. Therefore **an equivalent martingale measure rules out arbitrage among admissible self-financing strategies**. The lower-bound restriction is essential to this argument; stochastic integrals need not be true martingales for arbitrary unbounded holdings.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The holdings $\phi_t$ and $\pi_t^i$ are numbers of shares, so the marked-to-market [portfolio](../../../mathematical-finance.md#investment-portfolio) value is

$$
\boxed{X_t=\phi_tB_t+\pi_t\cdot S_t.}
$$

The stock prices are ex-dividend prices. Over the trading interval, existing holdings gain $\phi_t\,dB_t$ from the riskless account and $\pi_t\cdot dS_t$ from capital-price changes. In addition, $\pi_t^i$ shares of asset $i$ receive $\pi_t^iD_t^i\,dt$ in cash dividends. If this cash remains in the portfolio and changes of holdings are financed internally, the [self-financing portfolio](../../../mathematical-finance.md#self-financing-portfolio) equation is

$$
\boxed{dX_t=\phi_t\,dB_t+\pi_t\cdot dS_t+\pi_t\cdot D_t\,dt.}
$$

Rebalancing does not add a separate source of wealth: the cost of purchasing one holding is paid by selling another or by using the cash account. This is why one must specify the gains equation, rather than infer self-financing solely by differentiating the marked-to-market identity. The dividends are reinvested rather than withdrawn as [consumption](../../../mathematical-finance.md#consumption).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Use the discounted wealth $\widetilde X=X/B$ and the [discounted dividend gains](../../../mathematical-finance.md#discounted-dividend-gains)

$$
Y_t=\frac{S_t}{B_t}+\int_0^t\frac{D_s}{B_s}\,ds.
$$

The integral uses $ds$: the printed $dt$ inside an integral indexed by $s$ is a differential typo. Since $B$ is a positive [finite-variation process](../../../stochastic-calculus.md#finite-variation-process), the [Itô product rule](../../../stochastic-calculus.md#ito-product-rule) gives

$$
d\widetilde X_t
=\frac{dX_t}{B_t}-\frac{X_t}{B_t^2}\,dB_t
=\pi_t\cdot\left(\frac{dS_t}{B_t}-\frac{S_t}{B_t^2}\,dB_t+\frac{D_t}{B_t}\,dt\right)
=\pi_t\cdot dY_t.
$$

The bank-account terms cancel using $X_t=\phi_tB_t+\pi_t\cdot S_t$.

If $Y$ is a $Q$-[martingale](../../../martingale.md), discounted self-financing wealth is a $Q$-[local martingale](../../../martingale.md#local-martingale). The [admissible trading strategy](../../../mathematical-finance.md#admissible-trading-strategy) lower bound makes it a [supermartingale](../../../martingale.md#supermartingale), exactly as in the previous no-arbitrage proof. A zero-cost portfolio with nonnegative terminal wealth must therefore have terminal wealth zero $Q$-almost surely and, by equivalence, physically almost surely. Hence **an equivalent martingale measure for discounted dividend gains excludes arbitrage**. It is the gains process, not just the ex-dividend price ratio, that must have zero martingale drift.

## 5

↑ **Parent:** [Paper 39](paper-39.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Use the [Black-Scholes equation](../../../mathematical-finance.md#black-scholes-equation) with the claim's terminal condition $V(T,s)=g(s)$:

$$
V_t+rsV_s+\frac12\sigma^2s^2V_{ss}-rV=0.
$$

For $t<T$, the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) under the physical measure gives

$$
dV(t,S_t)=\left(rV(t,S_t)+(\mu-r)S_tV_s(t,S_t)\right)dt
+\sigma S_tV_s(t,S_t)\,dW_t.
$$

Choose the [delta hedge](../../../mathematical-finance.md#delta-hedge) and its bank-account holding by

$$
\boxed{\pi_t=V_s(t,S_t),\qquad
\phi_t=\frac{V(t,S_t)-S_tV_s(t,S_t)}{B_t}.}
$$

Their portfolio value is $V(t,S_t)$, and

$$
\phi_t\,dB_t+\pi_t\,dS_t
=\left(rV+(\mu-r)S_tV_s\right)dt+\sigma S_tV_s\,dW_t
=dV(t,S_t).
$$

Thus the portfolio is [self-financing](../../../mathematical-finance.md#self-financing-portfolio) and, with initial capital $V(0,S_0)$, has terminal wealth $g(S_T)$.

Localizing to compact stock-price intervals and times below $T$ justifies these stochastic integrals from the classical smoothness of $V$. The extension to maturity also follows from boundedness. Under the [Risk-neutral measure for the Black-Scholes model](../../../mathematical-finance.md#risk-neutral-measure-for-the-black-scholes-model), discounted $V(t,S_t)$ is a bounded [local martingale](../../../martingale.md#local-martingale), hence a true square-integrable [martingale](../../../martingale.md). Its quadratic variation has finite expectation, so the stock-integral coefficient is square integrable through $T$. Equivalence of measures preserves its almost-sure finiteness, and the physical drift integral is finite by [Cauchy-Schwarz](../../../probability-and-statistics.md#cauchy-schwarz-inequality). The terminal limit is $g(S_T)$.

Finally, $B_t=B_0e^{rt}$ is bounded away from zero on this finite horizon, and bounded $V$ makes $V(t,S_t)/B_t$ bounded below by a deterministic constant. The hedge is therefore an [admissible trading strategy](../../../mathematical-finance.md#admissible-trading-strategy). **The displayed holdings replicate the payoff admissibly**, even if the bounded payoff can be negative.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Set $\theta=(\mu-r)/\sigma$. The positive density

$$
Z_T=\exp\left(-\theta W_T-\frac12\theta^2T\right)
$$

has mean one, and the [Girsanov theorem](../../../stochastic-calculus.md#girsanov-theorem) makes $W_t^Q=W_t+\theta t$ a [Brownian motion](../../../brownian-motion.md) under the equivalent measure $Q$. Hence

$$
dS_t=S_t(r\,dt+\sigma\,dW_t^Q).
$$

The [Black-Scholes equation](../../../mathematical-finance.md#black-scholes-equation) makes $e^{-rt}V(t,S_t)$ a local martingale. Bounded $V$ on the finite horizon makes it a true martingale, so its terminal condition gives the [risk-neutral valuation](../../../mathematical-finance.md#risk-neutral-pricing)

$$
V(t,S_t)=e^{-r(T-t)}\mathbb E_Q[g(S_T)\mid\mathcal F_t].
$$

The [geometric Brownian motion](../../../stochastic-calculus.md#geometric-brownian-motion) solution under $Q$ is

$$
S_T=S_t\exp\left((r-\tfrac12\sigma^2)(T-t)+\sigma(W_T^Q-W_t^Q)\right).
$$

The Brownian increment is independent of $\mathcal F_t$ and equals $\sqrt{T-t}\,Z$ in distribution, where $Z$ has the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution). Therefore

$$
\boxed{V(t,s)=e^{-r(T-t)}\mathbb E\left[g\left(se^{a(t)+b(t)Z}\right)\right],\qquad
a(t)=(r-\tfrac12\sigma^2)(T-t),\quad b(t)=\sigma\sqrt{T-t}.}
$$

The expectation on the right is only an integral against the standard normal law; the physical drift $\mu$ has disappeared.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Let $L=\exp((r-\frac12\sigma^2)(T-t)+\sigma\sqrt{T-t}\,Z)$. Boundedness of $g'$ and integrability of the [lognormal distribution](../../../probability-theory.md#log-normal-distribution) variable $L$ justify differentiation under the expectation, by dominated convergence:

$$
V_s(t,s)=e^{-r(T-t)}\mathbb E[g'(sL)L].
$$

A differentiable increasing payoff has $g'\geq0$, and $L>0$. Thus the [delta hedge](../../../mathematical-finance.md#delta-hedge) has

$$
\boxed{\pi_t=e^{-r(T-t)}\mathbb E[g'(S_tL)L]\geq0.}
$$

Moreover $\mathbb EL=e^{r(T-t)}$, so $0\leq\pi_t\leq\|g'\|_\infty$. At maturity the delta is $g'(S_T)\geq0$. The [admissible trading strategy](../../../mathematical-finance.md#admissible-trading-strategy) already constructed therefore uses nonnegative stock holdings throughout replication. After maturity, liquidate the stock position and retain the proceeds in the bank account, so $\pi_t=0$ for $t>T$ if holdings are to be defined for all times.

## 6

↑ **Parent:** [Paper 39](paper-39.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Write $R=1+r$, $m=\mathbb E\xi_1$ and $c=\operatorname{Cov}(S_1,\xi_1)=\mathbb E[(S_1-\mu)(\xi_1-m)]$. The riskless gross return must be nonzero for the requested formulas; in the usual positive-bank-account model $R>0$. If $R=0$, the bank holding cannot affect the terminal payoff, and the later moment equation for pricing $B_0=1$ is impossible. We use the intended nondegenerate case $R\ne0$.

The claim and asset prices are square integrable. Centering separates the bias from the stochastic error:

$$
\mathbb E[(\xi_1-\phi R-\pi\cdot S_1)^2]
=(m-\phi R-\pi\cdot\mu)^2
+\operatorname{Var}(\xi_1)-2\pi^Tc+\pi^TV\pi.
$$

For fixed $\pi$, the unique minimizing bank holding removes the bias. The invertible [covariance matrix](../../../variance.md#covariance-matrix) $V$ is positive definite, and completing the square gives

$$
\pi^TV\pi-2\pi^Tc
=(\pi-V^{-1}c)^TV(\pi-V^{-1}c)-c^TV^{-1}c.
$$

Consequently the unique [one-period quadratic hedge](../../../mathematical-finance.md#one-period-quadratic-hedge) is

$$
\boxed{\pi^*=V^{-1}c,\qquad \phi^*=\frac{m-(\pi^*)^T\mu}{R}.}
$$

Its minimum expected squared error is $\operatorname{Var}(\xi_1)-c^TV^{-1}c$. This is a least-squares hedge, not necessarily exact [claim replication](../../../mathematical-finance.md#claim-replication).

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Put $h=S_0-\mu/R$. The initial capital of the [one-period quadratic hedge](../../../mathematical-finance.md#one-period-quadratic-hedge) is

$$
X_0^*=\phi^*+(\pi^*)^TS_0
=\frac{m}{R}+h^TV^{-1}c.
$$

Define the [minimum-norm one-period pricing weight](../../../mathematical-finance.md#minimum-norm-one-period-pricing-weight)

$$
\boxed{\rho^*=\frac1R+h^TV^{-1}(S_1-\mu).}
$$

It is square integrable, and $\mathbb E[(S_1-\mu)\xi_1]=c$, so

$$
\mathbb E[\rho^*\xi_1]=\frac{m}{R}+h^TV^{-1}c=X_0^*.
$$

The weight depends only on the asset prices and their first two moments, not on the claim. It can be negative, so this identity alone does not supply an [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure) or a positive [state-price density](../../../mathematical-finance.md#state-price-density).

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

The centered term in $\rho^*$ has zero mean, giving $\mathbb E\rho^*=1/R$ and hence $\mathbb E[\rho^*B_1]=1=B_0$. For the risky assets, symmetry of the [covariance matrix](../../../variance.md#covariance-matrix) gives

$$
\mathbb E[\rho^*S_1]
=\frac\mu R+\mathbb E[(S_1-\mu)(S_1-\mu)^T]V^{-1}h
=\frac\mu R+h=S_0.
$$

Therefore **$\rho^*$ reproduces every asset's initial price**.

For another square-integrable $\rho$ satisfying the price moment constraints, set $\delta=\rho-\rho^*$. The bank equation and $R\ne0$ give $\mathbb E\delta=0$, while the risky equations give $\mathbb E[\delta S_1]=0$. Since $\rho^*$ is an affine combination of $1$ and the coordinates of $S_1$,

$$
\mathbb E[\delta\rho^*]
=\frac1R\mathbb E\delta+h^TV^{-1}\mathbb E[\delta(S_1-\mu)]=0.
$$

The [Pythagorean theorem in an inner-product space](../../../linear-algebra.md#pythagorean-theorem-in-an-inner-product-space) now gives

$$
\boxed{\mathbb E[\rho^2]=\mathbb E[(\rho^*)^2]+\mathbb E[(\rho-\rho^*)^2]
\geq\mathbb E[(\rho^*)^2].}
$$

Equality holds exactly when $\rho=\rho^*$ almost surely. If a competing weight has infinite second moment, the inequality is immediate in the extended sense. The minimum itself is

$$
\mathbb E[(\rho^*)^2]=\frac1{R^2}+h^TV^{-1}h.
$$

Thus $\rho^*$ is the orthogonal projection of any feasible square-integrable pricing weight onto the linear span of the traded payoffs.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

Let $A=V^{1/2}$ be the symmetric positive square root of the [covariance matrix](../../../variance.md#covariance-matrix), and write $S_1=\mu+AZ$ with $Z$ having the [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution) $N_d(0,I)$. Bounded gradient makes $g$ globally Lipschitz, so $g(S_1)$ has at most linear growth and is square integrable. This also justifies the permitted [Gaussian integration by parts](../../../probability-theory.md#stein-s-lemma-probability) formula for each coordinate.

By the [chain rule](../../../calculus.md#chain-rule), $\nabla_z g(\mu+Az)=A^T\nabla g(\mu+Az)$. Applying Gaussian integration by parts gives

$$
c=\mathbb E[(S_1-\mu)g(S_1)]
=A\,\mathbb E[Zg(\mu+AZ)]
=AA^T\mathbb E[\nabla g(S_1)]
=V\mathbb E[\nabla g(S_1)].
$$

Thus the [Gaussian quadratic hedge](../../../mathematical-finance.md#gaussian-quadratic-hedge) holds $\pi^*=\mathbb E[\nabla g(S_1)]$. Substitution into its initial capital formula yields

$$
\boxed{X_0^*=\frac1{1+r}\mathbb E[g(S_1)]
+\left(S_0-\frac\mu{1+r}\right)\cdot\mathbb E[\nabla g(S_1)].}
$$

Only the hedge calculation is being used here; the Gaussian model need not possess a positive pricing weight for this least-squares identity.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
