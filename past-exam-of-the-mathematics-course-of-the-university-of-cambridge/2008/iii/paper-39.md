# Paper 39

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper39.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper39.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
  - [v](#1/v)
    - [Solution](#1/v/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
  - [iii](#5/iii)
    - [Solution](#5/iii/solution)
- [6](#6)
  - [i](#6/i)
    - [Solution](#6/i/solution)
  - [ii](#6/ii)
    - [Solution](#6/ii/solution)

## 1

↑ **Parent:** [Paper 39](paper-39.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

A one-period [arbitrage](../../../mathematical-finance.md#arbitrage) is a [portfolio](../../../mathematical-finance.md#investment-portfolio) of initial-information-measurable holdings $(h_B,h_S)$ with value $V_t=h_BB_t+h_SS_t$ such that

$$
\boxed{V_0=0,\qquad V_1\geq0\text{ almost surely},\qquad\mathbb P(V_1>0)>0.}
$$

The holdings are fixed during the period, so this is a [self-financing strategy](../../../mathematical-finance.md#self-financing-portfolio). A [portfolio](../../../mathematical-finance.md#investment-portfolio) costing a negative amount with nonnegative terminal value also gives an [arbitrage](../../../mathematical-finance.md#arbitrage): invest its initial surplus in the strictly positive [bank account](../../../mathematical-finance.md#bank-account) to obtain a zero-cost [portfolio](../../../mathematical-finance.md#investment-portfolio) with a strict gain. The same definition applies when further traded assets are added.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

An [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure) is a [probability measure](../../../probability-theory.md#probability-measure) $Q$ equivalent to the objective measure $P$, meaning the two have exactly the same null events, under which the discounted stock $\widetilde S_t=S_t/B_t$ is a [martingale](../../../martingale.md). In this one-period model the condition is

$$
\boxed{\mathbb E_Q[S_1/B_1\mid\mathcal F_0]=S_0/B_0,\qquad Q\sim P.}
$$

The discounted [bank account](../../../mathematical-finance.md#bank-account) is identically one. [Integrability](../../../measure-theory.md#integrability) of the discounted stock is part of the [martingale](../../../martingale.md) condition. In an augmented market the discounted price of every additional asset must satisfy the same condition.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Suppose $Q$ is an [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure) and a zero-cost [self-financing strategy](../../../mathematical-finance.md#self-financing-portfolio) has holdings $(h_B,h_S)$. Its discounted terminal value has [conditional expectation](../../../measure-theory.md#conditional-expectation)

$$
\mathbb E_Q[V_1/B_1\mid\mathcal F_0]=h_B+h_S\mathbb E_Q[S_1/B_1\mid\mathcal F_0]=h_B+h_SS_0/B_0=V_0/B_0=0.
$$

If it were an [arbitrage](../../../mathematical-finance.md#arbitrage), $V_1/B_1$ would be nonnegative because $B_1>0$. Equivalence implies that it is strictly positive on an event of positive $Q$-probability. A nonnegative [random variable](../../../random-variable.md) with zero [conditional expectation](../../../measure-theory.md#conditional-expectation) must be zero almost surely, a contradiction. Thus $\boxed{\text{an equivalent martingale measure excludes arbitrage}}$. The calculation uses the usual integrable one-period strategies, and also works conditionally for finite initial-information-measurable holdings.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

The [European call option](../../../mathematical-finance.md#european-call-option) pays one in the state $S_1=5$ and zero in the other two states. Short one call, buy one third of a stock, and borrow one half unit of cash. Writing the option quote as $c=1/2$, the holdings and initial value are

$$
\boxed{(h_B,h_S,h_C)=(-1/2,1/3,-1),\qquad V_0=-1/2+1-c=0.}
$$

The terminal value is $-1/2+S_1/3-(S_1-4)^+$. At stock prices $5,3,2$ it is respectively

$$
\boxed{(1/6,\ 1/2,\ 1/6).}
$$

It is strictly positive in every state, so this [portfolio](../../../mathematical-finance.md#investment-portfolio) is an [arbitrage](../../../mathematical-finance.md#arbitrage).

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

Let $c$ be the initial call price. Write the risk-neutral [probabilities](../../../probability-theory.md#probability) of stock prices $5,3,2$ as $q_5,q_3,q_2$. The stock's [martingale](../../../martingale.md) equation and the normalization give $q_2=2q_5$ and $q_3=1-3q_5$. The call pays only in the first state, so its [martingale](../../../martingale.md) equation is $q_5=c$. Thus

$$
(q_5,q_3,q_2)=(c,1-3c,2c).
$$

All three objective [probabilities](../../../probability-theory.md#probability) are positive. This defines an [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure) precisely when $0<c<1/3$, and part (iii) proves that every such price excludes [arbitrage](../../../mathematical-finance.md#arbitrage).

To prove necessity without appealing to an existence theorem, consider the other prices explicitly. If $c\leq0$, buy one call and hold $-c$ units of cash. Its initial value is zero and terminal value is $(S_1-4)^+-c$, nonnegative and positive with positive [probability](../../../probability-theory.md#probability). If $c\geq1/3$, take holdings $(h_B,h_S,h_C)=(c-1,1/3,-1)$. The initial value is $c-1+1-c=0$ and terminal values at $5,3,2$ are $(c-1/3,c,c-1/3)$. They are nonnegative and the middle-state value is strictly positive. This includes the endpoint $c=1/3$. Consequently

$$
\boxed{\text{the arbitrage-free call prices are exactly }c\in(0,1/3).}
$$

## 2

↑ **Parent:** [Paper 39](paper-39.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

A [complete market](../../../mathematical-finance.md#complete-market) is one in which every [contingent claim](../../../mathematical-finance.md#contingent-claim) in the pricing class can be replicated: for each finite maturity $T$ and terminal $\mathcal F_T$-measurable payoff $H$, there are an initial value and an admissible [self-financing strategy](../../../mathematical-finance.md#self-financing-portfolio) whose terminal value is $H$ almost surely. It is enough for the [complete market](../../../mathematical-finance.md#complete-market) characterization to include all claims with bounded discounted payoffs. Thus **every such payoff is attainable by trading the existing assets**, rather than needing an additional independent security.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Suppose $Q_1,Q_2$ are [equivalent martingale measures](../../../mathematical-finance.md#risk-neutral-measure). Fix a finite maturity $T$ and an event $E\in\mathcal F_T$. Because the market is a [complete market](../../../mathematical-finance.md#complete-market), replicate the claim $H=B_T\mathbf1_E$, whose discounted payoff is bounded. For a [self-financing strategy](../../../mathematical-finance.md#self-financing-portfolio), the discounted value satisfies

$$
\widetilde V_{t+1}-\widetilde V_t=h^S_t(\widetilde S_{t+1}-\widetilde S_t),\qquad\widetilde S=S/B.
$$

Under either pricing measure its conditional mean increment is zero, since $h^S_t$ is known at time $t$ and the discounted stock is a [martingale](../../../martingale.md). In the standard admissible discrete-time pricing class these finite-horizon values are integrable; a constant lower bound on discounted wealth also gives [integrability](../../../measure-theory.md#integrability) successively from the conditional increment formula. Therefore replication and taking [expectations](../../../probability-theory.md#expected-value) give

$$
\frac{V_0}{B_0}=\mathbb E_{Q_j}[H/B_T]=Q_j(E),\qquad j=1,2.
$$

The replicating [portfolio](../../../mathematical-finance.md#investment-portfolio) and its initial cost are the same for both measures, so $Q_1(E)=Q_2(E)$. Since $E$ was arbitrary, the measures agree on $\mathcal F_T$, for every finite $T$, and hence on the [sigma-algebra](../../../measure-theory.md#sigma-algebra) generated by the market [filtration](../../../stochastic-process.md#filtration-probability-theory). Thus $\boxed{\text{the equivalent martingale measure is unique}}$. This is the measure version of [complete markets have unique state-price densities](../../../mathematical-finance.md#complete-markets-have-unique-state-price-densities).

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Let $Q$ be the unique [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure). The [risk-neutral pricing](../../../mathematical-finance.md#risk-neutral-pricing) formula is

$$
C(T,K)=B_0\mathbb E_Q\left[\frac{(S_T-K)^+}{B_T}\right]=B_0\mathbb E_Q[(M_T-K/B_T)^+],\qquad M_t=S_t/B_t.
$$

For the usual nonnegative strike $K$ and maturities $u\geq t$, the monotonic [bank account](../../../mathematical-finance.md#bank-account) gives $K/B_u\leq K/B_t$. Therefore

$$
\begin{aligned}\mathbb E_Q[(M_u-K/B_u)^+\mid\mathcal F_t]&\geq\mathbb E_Q[(M_u-K/B_t)^+\mid\mathcal F_t]\\&\geq(\mathbb E_Q[M_u\mid\mathcal F_t]-K/B_t)^+\\&=(M_t-K/B_t)^+.
\end{aligned}
$$

The second inequality follows directly since the [conditional expectation](../../../measure-theory.md#conditional-expectation) of a [positive part](../../../function.md#positive-part-of-a-real-valued-function) is at least both zero and the [conditional expectation](../../../measure-theory.md#conditional-expectation) of its argument; it is also conditional [Jensen's inequality](../../../real-analysis.md#jensen-s-inequality). Taking [expectations](../../../probability-theory.md#expected-value) proves $C(u,K)\geq C(t,K)$, the [maturity monotonicity of calls with nonnegative strikes](../../../mathematical-finance.md#maturity-monotonicity-of-calls-with-nonnegative-strikes).

If $K_1\leq K_2$, then $(S_T-K_1)^+\geq(S_T-K_2)^+$ pointwise; positive discounting and [expectation](../../../probability-theory.md#expected-value) prove [monotonicity of a European call price in strike](../../../mathematical-finance.md#monotonicity-of-a-european-call-price-in-strike). For $0\leq a\leq1$, the pointwise inequality

$$
(S_T-aK_1-(1-a)K_2)^+\leq a(S_T-K_1)^++(1-a)(S_T-K_2)^+
$$

gives [convexity of a European call price in strike](../../../mathematical-finance.md#convexity-of-a-european-call-price-in-strike) after the same operations. Hence

$$
\boxed{C(T,K)\text{ is nondecreasing in }T,\text{ nonincreasing and convex in }K.}
$$

The maturity assertion uses $K\geq0$; it need not hold for a negative strike. For example, in the deterministic [complete market](../../../mathematical-finance.md#complete-market) $S_t=B_t=e^{rt}$ with $r>0$, a negative-strike call has price $1-Ke^{-rT}$, which decreases with $T$. The monotonicity assertions are non-strict, as equality can occur.

## 3

↑ **Parent:** [Paper 39](paper-39.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Relative to a [filtration](../../../stochastic-process.md#filtration-probability-theory) $(\mathcal F_t)$, a [supermartingale](../../../martingale.md#supermartingale) is an [adapted process](../../../stochastic-process.md#adapted-process) $U_t$ with $\mathbb E|U_t|<\infty$ for every $t$ and

$$
\boxed{\mathbb E[U_{t+1}\mid\mathcal F_t]\leq U_t\quad\text{almost surely for every }t.}
$$

By the [tower property](../../../measure-theory.md#law-of-total-expectation) this also gives $\mathbb E[U_u\mid\mathcal F_t]\leq U_t$ for every $u\geq t$.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

For a [stopping time](../../../martingale.md#stopping-time) $\tau$, $U_{t\wedge\tau}$ is adapted: split according to $\{\tau=j\}$ for $j<t$ and $\{\tau\geq t\}$, all events belonging to $\mathcal F_t$. It is integrable because $|U_{t\wedge\tau}|\leq\sum_{j=0}^t|U_j|$. Moreover,

$$
U_{(t+1)\wedge\tau}-U_{t\wedge\tau}=\mathbf1_{\{\tau>t\}}(U_{t+1}-U_t).
$$

The indicator is $\mathcal F_t$-measurable, so conditioning and the [supermartingale](../../../martingale.md#supermartingale) property give

$$
\mathbb E[U_{(t+1)\wedge\tau}-U_{t\wedge\tau}\mid\mathcal F_t]=\mathbf1_{\{\tau>t\}}(\mathbb E[U_{t+1}\mid\mathcal F_t]-U_t)\leq0.
$$

Thus $\boxed{(U_{t\wedge\tau})_t\text{ is a supermartingale}}$. This proves [stopping preserves supermartingales in discrete time](../../../martingale.md#stopping-preserves-supermartingales-in-discrete-time) without assuming $\tau$ itself bounded or integrable.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Use the tree's natural [filtration](../../../stochastic-process.md#filtration-probability-theory). The [stopping times](../../../martingale.md#stopping-time) take values in the process horizon $\{0,1,2\}$. Construct a dominating [supermartingale](../../../martingale.md#supermartingale) $Y$ by backward comparison, the finite-horizon [Snell envelope](../../../martingale.md#snell-envelope). At time two put $Y_2=\xi_2$. At time one the continuation values are

$$
\mathbb E[\xi_2\mid\xi_1=11]=\frac23\,13+\frac13\,10=12,\qquad\mathbb E[\xi_2\mid\xi_1=7]=\frac12\,8+\frac12\,4=6.
$$

Compare these with immediate rewards $11$ and $7$ to obtain $Y_1=12$ on the upper branch and $Y_1=7$ on the lower branch. Finally set

$$
Y_0=\max\{8,\mathbb EY_1\}=\max\left\{8,\frac25\,12+\frac35\,7\right\}=9.
$$

These definitions explicitly give $Y_t\geq\xi_t$, $Y_0=\mathbb EY_1$, and $Y_1\geq\mathbb E[Y_2\mid\mathcal F_1]$. Thus $Y$ is a [supermartingale](../../../martingale.md#supermartingale). By part (ii), its [stopped process](../../../martingale.md#stopped-process) is a [supermartingale](../../../martingale.md#supermartingale), so for every allowed $\tau$,

$$
\boxed{\mathbb E\xi_\tau\leq\mathbb EY_\tau=\mathbb EY_{2\wedge\tau}\leq Y_0=9.}
$$

The reward process itself need not be a [supermartingale](../../../martingale.md#supermartingale); the constructed majorant is what proves the bound.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

Continue at time zero. At time one stop on the lower branch and continue on the upper branch:

$$
\boxed{\tau_0=\begin{cases}1,&\xi_1=7,\\2,&\xi_1=11.\end{cases}}
$$

This is a [stopping time](../../../martingale.md#stopping-time) since the branch decision is [measurable](../../../measure-theory.md#measurability) at time one. Its expected reward is

$$
\boxed{\mathbb E\xi_{\tau_0}=\frac35\,7+\frac25\left(\frac23\,13+\frac13\,10\right)=9.}
$$

It therefore attains the upper bound in part (iii).

## 4

↑ **Parent:** [Paper 39](paper-39.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Use the usual [Black-Scholes model](../../../mathematical-finance.md#black-scholes-model) with $\sigma>0$ and the [filtration](../../../stochastic-process.md#filtration-probability-theory) generated by $W$. Set

$$
\boxed{\lambda=\frac{\mu-r}{\sigma},\qquad Z_t=\exp\left(-\lambda W_t-\frac12\lambda^2t\right).}
$$

For $u>t$, [independence](../../../random-variable.md#independent-random-variables) and the [Gaussian distribution](../../../probability-theory.md#normal-distribution) [exponential moment](../../../probability-theory.md#exponential-moment) formula give $\mathbb E_P[Z_u/Z_t\mid\mathcal F_t]=1$. Thus $Z$ is a strictly positive [martingale](../../../martingale.md) of mean one, defining an equivalent measure $Q$ on every finite horizon by $dQ/dP|_{\mathcal F_t}=Z_t$.

To verify the measure change directly, put $\widehat W_t=W_t+\lambda t$. For any real $a$ and $h=u-t$,

$$
\begin{aligned}\mathbb E_Q[e^{ia(\widehat W_u-\widehat W_t)}\mid\mathcal F_t]&=\mathbb E_P[(Z_u/Z_t)e^{ia(W_u-W_t+\lambda h)}\mid\mathcal F_t]\\&=e^{ia\lambda h-\lambda^2h/2}\exp\left(\tfrac12(-\lambda+ia)^2h\right)\\&=e^{-a^2h/2}.
\end{aligned}
$$

The conditional [characteristic function](../../../probability-theory.md#characteristic-function) is that of $N(0,h)$ and does not depend on past information. Therefore $\widehat W$ has independent increments with [Gaussian distribution](../../../probability-theory.md#normal-distribution) and continuous paths, and is a [Brownian motion](../../../brownian-motion.md) under $Q$. Substituting $dW=d\widehat W-\lambda dt$ gives $dS_t=S_t(rdt+\sigma d\widehat W_t)$. Hence $S_t/B_t$ is a [geometric Brownian motion](../../../stochastic-calculus.md#geometric-brownian-motion) that is a [martingale](../../../martingale.md) and $Q$ is an [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure).

The form is also forced. By the [Brownian martingale representation theorem](../../../brownian-motion.md#brownian-martingale-representation-theorem), any [density process](../../../measure-theory.md#density-process) that is a [martingale](../../../martingale.md) has $dZ_t=a_t\,dW_t$. The [change of measure](../../../measure-theory.md#change-of-measure) identity makes $Z_tS_t/B_t$ a [local martingale](../../../martingale.md#local-martingale) under $P$. Its drift, calculated by [Itô formula](../../../stochastic-calculus.md#ito-s-lemma), is $(S_t/B_t)[Z_t(\mu-r)+\sigma a_t]dt$, which must vanish. Thus $a_t=-\lambda Z_t$. Solving $dZ_t=-\lambda Z_t\,dW_t$ with $Z_0=1$ gives exactly the displayed [stochastic exponential](../../../stochastic-calculus.md#doleans-dade-exponential). Equivalence here is on each finite horizon, as usual for Black-Scholes pricing.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Let $\Phi$ denote the standard [normal distribution](../../../probability-theory.md#normal-distribution) [cumulative distribution function](../../../probability-theory.md#cumulative-distribution-function), and $\phi$ its density. Put $\tau=T-t$. For $K>0$ and $t<T$, define

$$
d_1=\frac{\log(S_t/K)+(r+\sigma^2/2)\tau}{\sigma\sqrt\tau},\qquad d_2=d_1-\sigma\sqrt\tau.
$$

Under the [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure), conditional on $\mathcal F_t$,

$$
S_T=S_t\exp\bigl((r-\sigma^2/2)\tau+\sigma\sqrt\tau\,Z\bigr),\qquad Z\sim N(0,1).
$$

Thus $Q(S_T<K\mid\mathcal F_t)=\Phi(-d_2)$. The identity $e^{az}\phi(z)=e^{a^2/2}\phi(z-a)$ for the standard [Gaussian distribution](../../../probability-theory.md#normal-distribution) [probability density function](../../../continuous-probability-distribution.md#probability-density-function) gives

$$
\mathbb E_Q[S_T\mathbf1_{\{S_T\geq K\}}\mid\mathcal F_t]=S_te^{r\tau}\Phi(d_1).
$$

Split the payout according to whether the stock exceeds the floor and discount. The [risk-neutral pricing](../../../mathematical-finance.md#risk-neutral-pricing) process is

$$
\boxed{\xi_t=V(t,S_t)=S_t\Phi(d_1)+Ke^{-r(T-t)}\Phi(-d_2),\qquad \xi_T=\max(K,S_T).}
$$

Its discounted value is $\mathbb E_Q[\xi_T/B_T\mid\mathcal F_t]$, a true [martingale](../../../martingale.md). Thus adding this asset preserves the [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure) and gives no [arbitrage](../../../mathematical-finance.md#arbitrage). This is the [guaranteed terminal stock floor in the Black-Scholes model](../../../mathematical-finance.md#guaranteed-terminal-stock-floor-in-the-black-scholes-model). For $K\leq0$, positivity of the stock makes the claim simply $S_T$, and the price is $\xi_t=S_t$.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Let $\phi$ denote the standard [Gaussian distribution](../../../probability-theory.md#normal-distribution) [probability density function](../../../continuous-probability-distribution.md#probability-density-function). Directly from the definitions, $S\phi(d_1)=Ke^{-r\tau}\phi(d_2)$. Differentiating the price in part (ii), the terms involving [derivatives](../../../calculus.md#derivative) of $d_1,d_2$ cancel, yielding $V_S=\Phi(d_1)$. Therefore, in units of the two traded assets, the [replicating strategy](../../../mathematical-finance.md#replicating-strategy) is

$$
\boxed{h^S_t=\Phi(d_1),\qquad h^B_t=\frac{Ke^{-r(T-t)}\Phi(-d_2)}{B_t}\qquad(t<T).}
$$

Its value is $h^B_tB_t+h^S_tS_t=V(t,S_t)$. To check self-financing explicitly, [differentiation](../../../calculus.md#differentiation) also gives

$$
V_{SS}=\frac{\phi(d_1)}{S\sigma\sqrt\tau},\qquad V_t=-\frac{S\sigma\phi(d_1)}{2\sqrt\tau}+rKe^{-r\tau}\Phi(-d_2).
$$

Hence $V_t+rSV_S+\tfrac12\sigma^2S^2V_{SS}=rV$. Applying [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) under the physical measure gives

$$
dV=[rV+(\mu-r)SV_S]dt+\sigma SV_SdW=h^B_t\,dB_t+h^S_t\,dS_t.
$$

Thus the holdings form a [self-financing strategy](../../../mathematical-finance.md#self-financing-portfolio) and their terminal value is the required payout. Holdings at the single maturity instant can be assigned by their limiting values; the continuous-time trading gains do not depend on that assignment. If $\pi_t$ denotes wealth fractions instead, the stock fraction is $S_t\Phi(d_1)/V(t,S_t)$ and the bank fraction is $Ke^{-r\tau}\Phi(-d_2)/V(t,S_t)$. For $K\leq0$, hold one stock and no bank-account units.

## 5

↑ **Parent:** [Paper 39](paper-39.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

Let $Q$ be the given [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure), and write $B_t=B_0e^{rt}$. Take $V$ to be classical on $t<T$ and continuous at its prescribed terminal value. By [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) and the [pricing equation for a local volatility model](../../../mathematical-finance.md#pricing-equation-for-a-local-volatility-model),

$$
\begin{aligned}
dV(t,S_t)&=\left[V_t+rS_tV_S+\tfrac12\sigma(S_t)^2S_t^2V_{SS}\right]dt+\sigma(S_t)S_tV_S\,d\widehat W_t\\
&=rV(t,S_t)dt+\sigma(S_t)S_tV_S\,d\widehat W_t,
\end{aligned}
$$

so

$$
d\left(\frac{\xi_t}{B_t}\right)=\frac{\sigma(S_t)S_tV_S(t,S_t)}{B_t}\,d\widehat W_t.
$$

The discounted added asset is a [local martingale](../../../martingale.md#local-martingale), as is $S_t/B_t$, while $B_t/B_t=1$. Consequently $Q$ is an [equivalent local martingale measure](../../../mathematical-finance.md#equivalent-local-martingale-measure) for all three assets.

Here is the [arbitrage](../../../mathematical-finance.md#arbitrage) argument, including the usual [admissible trading strategy](../../../mathematical-finance.md#admissible-trading-strategy) condition. If $X$ is the discounted wealth of a [self-financing strategy](../../../mathematical-finance.md#self-financing-portfolio), it is a [stochastic integral](../../../stochastic-calculus.md#stochastic-integral) against the discounted asset prices, plus its initial value, and hence a [local martingale](../../../martingale.md#local-martingale). Assume $X_t\geq-c$ for a fixed $c$, as required for an [admissible trading strategy](../../../mathematical-finance.md#admissible-trading-strategy). For a localizing sequence $\tau_n$, the [stopped process](../../../martingale.md#stopped-process) $X^{\tau_n}$ is a [martingale](../../../martingale.md). Apply the conditional [Fatou lemma](../../../measure-theory.md#fatou-s-lemma) to $X_{t\wedge\tau_n}+c\geq0$: for $s\leq t$, continuity and the stopped [martingale](../../../martingale.md) identity give $\mathbb E_Q[X_t+c\mid\mathcal F_s]\leq X_s+c$. Thus $X$ is a [supermartingale](../../../martingale.md#supermartingale). An [arbitrage](../../../mathematical-finance.md#arbitrage) would have $X_0=0$, $X_T\geq0$ and positive [probability](../../../probability-theory.md#probability) of $X_T>0$. Equivalence of $P,Q$ makes that [probability](../../../probability-theory.md#probability) positive under $Q$, contradicting $\mathbb E_Q[X_T]\leq0$. Therefore **the augmented market has no admissible [arbitrage](../../../mathematical-finance.md#arbitrage)**.

Nonnegativity of $V$ gives the needed price process, but does not by itself make its discounted [local martingale](../../../martingale.md#local-martingale) a true [martingale](../../../martingale.md). If $V$ is bounded, the latter follows by bounded [localization](../../../commutative-algebra.md#localization-of-a-ring), and its price is also $B_t\mathbb E_Q[g(S_T)/B_T\mid\mathcal F_t]$. The [arbitrage](../../../mathematical-finance.md#arbitrage) proof above applies to the stated nonnegative classical solution without assuming that additional bound.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

The [delta replication from a local-volatility pricing equation](../../../mathematical-finance.md#delta-replication-from-a-local-volatility-pricing-equation) uses the asset-unit holdings

$$
\boxed{h^S_t=V_S(t,S_t),\qquad h^B_t=\frac{V(t,S_t)-S_tV_S(t,S_t)}{B_t}.}
$$

Their wealth is exactly $V(t,S_t)$. Moreover,

$$
h^B_t\,dB_t+h^S_t\,dS_t=rV(t,S_t)dt+\sigma(S_t)S_tV_S(t,S_t)d\widehat W_t=dV(t,S_t),
$$

where the final equality is the calculation in part (i). Thus the holdings are a [self-financing strategy](../../../mathematical-finance.md#self-financing-portfolio) with terminal wealth $g(S_T)$, proving replication. Since $V\geq0$, this [replicating strategy](../../../mathematical-finance.md#replicating-strategy) has nonnegative wealth and is an [admissible trading strategy](../../../mathematical-finance.md#admissible-trading-strategy). The equality of trading gains is unchanged by replacing the drift with its physical-measure value: the stock drift in [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) and in the stock holding changes by the same amount. If $\pi_t$ denotes wealth fractions, then, wherever $V>0$, its stock fraction is $S_tV_S/V$ and its bank fraction is $1-S_tV_S/V$.

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

The [diffusion coefficient](../../../brownian-motion.md#diffusion-coefficient) becomes $S\sigma(S)=\sqrt S$, so the stock is a [driftless square-root diffusion](../../../stochastic-calculus.md#driftless-square-root-diffusion), with zero taken as an absorbing boundary. Substitution of $V(t,S)=e^{A(t)S+B(t)}$ into the [pricing equation for a local volatility model](../../../mathematical-finance.md#pricing-equation-for-a-local-volatility-model) gives

$$
A'(t)S+B'(t)+\tfrac12A(t)^2S=0.
$$

Equating the constant and linear terms and imposing the terminal payoff gives

$$
A'+\tfrac12A^2=0,\quad B'=0,\quad A(1)=1,\quad B(1)=0.
$$

Thus $1/A(t)=(1+t)/2$ and $B(t)=0$, and the price is

$$
\boxed{\xi_t=V(t,S_t)=\exp\left(\frac{2S_t}{1+t}\right),\qquad 0\leq t\leq1.}
$$

This is the [exponential claim in a driftless square-root model](../../../mathematical-finance.md#exponential-claim-in-a-driftless-square-root-model). At the absorbing boundary its value is $1$, matching the payoff at zero.

The payoff in this part is unbounded, unlike the payoff assumed in part (i), so it is useful to verify that the proposed price is a finite [conditional expectation](../../../measure-theory.md#conditional-expectation). For $h>0$, starting from stock value $s$, define

$$
F(v,x)=\exp\left(-\frac{ux}{1+u(h-v)/2}\right),\qquad 0\leq v\leq h,\quad u\geq0.
$$

Then $F_v+\tfrac12xF_{xx}=0$, $F(h,x)=e^{-ux}$, and $0\leq F\leq1$. By [Itô formula](../../../stochastic-calculus.md#ito-s-lemma), $F(v,S_v)$ is a bounded [local martingale](../../../martingale.md#local-martingale), hence a true [martingale](../../../martingale.md). It follows that

$$
\mathbb E_s[e^{-uS_h}]=\exp\left(-\frac{su}{1+uh/2}\right).
$$

This is also the [Laplace transform](../../../analysis.md#laplace-transform) of a sum of $N$ independent variables with [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) of rate $2/h$, where $N$ has [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) of mean $2s/h$ and is independent of the summands: its transform is $\exp[(2s/h)((2/h)/(2/h+u)-1)]$. Uniqueness of the [Laplace transform](../../../analysis.md#laplace-transform) therefore gives the [compound Poisson transition law of a driftless square-root diffusion](../../../stochastic-calculus.md#compound-poisson-transition-law-of-a-driftless-square-root-diffusion). The [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) jump has [exponential moment](../../../probability-theory.md#exponential-moment) $\mathbb E[e^{Y}]=(2/h)/(2/h-1)$ whenever $h<2$. Summing over the [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) yields

$$
\mathbb E_s[e^{S_h}]=\exp\left[\frac{2s}{h}\left(\frac{2/h}{2/h-1}-1\right)\right]=\exp\left(\frac{s}{1-h/2}\right).
$$

For the remaining horizon $h=1-t\leq1$, this is finite and, by the [Markov property](../../../markov-process.md#markov-property), is precisely $\mathbb E_Q[e^{S_1}\mid\mathcal F_t]=e^{2S_t/(1+t)}$. Thus the displayed process is indeed the [risk-neutral pricing](../../../mathematical-finance.md#risk-neutral-pricing) value and a true [martingale](../../../martingale.md). The [replicating strategy](../../../mathematical-finance.md#replicating-strategy) from part (ii) has $h^S_t=[2/(1+t)]V(t,S_t)$ and $h^B_t=[1-2S_t/(1+t)]V(t,S_t)/B_t$.

## 6

↑ **Parent:** [Paper 39](paper-39.md)

<h3 id="6/i">i</h3>

↑ **Parent:** [6](#6)

<h4 id="6/i/solution">Solution</h4>

↑ **Parent:** [I](#6/i)

Let $Q$ denote the given unique [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure). A [zero-coupon bond](../../../mathematical-finance.md#zero-coupon-bond) paying one at $T$ has [risk-neutral pricing](../../../mathematical-finance.md#risk-neutral-pricing) value

$$
P_t(T)=\mathbb E_Q\left[\exp\left(-\int_t^Tr_sds\right)\middle|\mathcal F_t\right].
$$

Write $h=T-t$. Split the integrated [short rate](../../../mathematical-finance.md#short-rate) into its known and future parts:

$$
\int_t^Tr_sds=\int_t^Tg(s)ds+\sigma h\widehat W_t+\sigma\int_t^T(\widehat W_s-\widehat W_t)ds.
$$

By integrating the future [Brownian motion](../../../brownian-motion.md) increments in the opposite order, the last integral equals $\int_t^T(T-u)d\widehat W_u$. It is independent of $\mathcal F_t$ and is a [Gaussian random variable](../../../probability-theory.md#gaussian-random-variable) of mean zero and [variance](../../../variance.md)

$$
\int_t^T(T-u)^2du=\frac{h^3}{3}.
$$

The [Gaussian](../../../probability-theory.md#normal-distribution) [exponential moment](../../../probability-theory.md#exponential-moment) formula $\mathbb E[e^{aZ}]=e^{a^2\operatorname{Var}(Z)/2}$ for centered $Z$ therefore gives the bond price in this [Gaussian short-rate model with a deterministic shift](../../../mathematical-finance.md#gaussian-short-rate-model-with-a-deterministic-shift):

$$
\boxed{P_t(T)=\exp\left[-\int_t^Tg(s)ds-\sigma(T-t)\widehat W_t+\frac{\sigma^2(T-t)^3}{6}\right].}
$$

The [instantaneous forward rate](../../../mathematical-finance.md#instantaneous-forward-rate) is the negative maturity [derivative](../../../calculus.md#derivative) of the logarithm of the bond price. Consequently

$$
\boxed{f_t(T)=g(T)+\sigma\widehat W_t-\frac{\sigma^2}{2}(T-t)^2.}
$$

In particular, $P_t(t)=1$ and $f_t(t)=g(t)+\sigma\widehat W_t=r_t$, as required. The [derivative](../../../calculus.md#derivative) formula is pointwise for continuous $g$ and almost everywhere for locally integrable $g$.

<h3 id="6/ii">ii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6/ii)

Let $F_0(T)$ be the observed initial [instantaneous forward rate](../../../mathematical-finance.md#instantaneous-forward-rate) curve. Since $\widehat W_0=0$, part (i) gives $f_0(T)=g(T)-\sigma^2T^2/2$. Thus the [forward-curve calibration of a shifted Brownian short rate](../../../mathematical-finance.md#forward-curve-calibration-of-a-shifted-brownian-short-rate) is achieved by the deterministic choice

$$
\boxed{g(T)=F_0(T)+\frac{\sigma^2T^2}{2}.}
$$

Substitution gives $f_0(T)=F_0(T)$ at every maturity where the curve is defined classically. It also reproduces the corresponding initial [zero-coupon bond](../../../mathematical-finance.md#zero-coupon-bond) curve:

$$
P_0(T)=\exp\left[-\int_0^TF_0(s)ds-\frac{\sigma^2T^3}{6}+\frac{\sigma^2T^3}{6}\right]=\exp\left[-\int_0^TF_0(s)ds\right].
$$

There is no shape restriction on the initial curve beyond the regularity needed to define these integrals and forward [derivatives](../../../calculus.md#derivative); for continuous curves the match is pointwise, and for locally integrable curves the forward identity has its almost-everywhere interpretation.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
