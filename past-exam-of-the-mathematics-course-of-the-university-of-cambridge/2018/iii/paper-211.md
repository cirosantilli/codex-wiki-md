# Paper 211

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_211.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_211.pdf)

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

## 1

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For holdings $h\in\mathbb R^n$, let $V_0=h\cdot P_0$ and $V_1=h\cdot P_1$. Under the [investment-consumption arbitrage](../../../mathematical-finance.md#investment-consumption-arbitrage) convention used here, an [arbitrage](../../../mathematical-finance.md#arbitrage) satisfies

$$
\boxed{V_0\leq0,\quad V_1\geq0\ \text{a.s.},\quad V_0<0\ \text{or}\ \mathbb P(V_1>0)>0.}
$$

The initial [consumption](../../../mathematical-finance.md#consumption) is $-V_0$, and the terminal [consumption](../../../mathematical-finance.md#consumption) is $V_1$: there is a possible gain with no external funding and no negative [consumption](../../../mathematical-finance.md#consumption). A [pure-investment arbitrage](../../../mathematical-finance.md#pure-investment-arbitrage) additionally requires $V_0=0$. This convention is important because the last part distinguishes initial [consumption](../../../mathematical-finance.md#consumption) from pure investment.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

A [pricing kernel](../../../mathematical-finance.md#state-price-density) is a strictly positive [random variable](../../../random-variable.md) $R$ such that $RP_1^i$ is integrable and

$$
\boxed{P_0^i=\mathbb E[RP_1^i]\qquad(i=1,\ldots,n).}
$$

It is a one-period [state-price density](../../../mathematical-finance.md#state-price-density), converting a terminal payoff into its initial price. Strict positivity means $R>0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), not merely $R\geq0$. When cash has price $1$ at both dates, this identity forces $\mathbb ER=1$, so $d\mathbb Q=R\,d\mathbb P$ defines an [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For any holdings $h$, the [pricing kernel](../../../mathematical-finance.md#state-price-density) identity implies $V_0=\mathbb E[RV_1]$. If $V_1\geq0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), then $V_0\geq0$, so an [arbitrage](../../../mathematical-finance.md#arbitrage) cannot have $V_0<0$. If also $V_0=0$, then the nonnegative integrable [random variable](../../../random-variable.md) $RV_1$ has zero [expectation](../../../probability-theory.md#expected-value) and hence is zero [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Since $R>0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), $V_1=0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), ruling out a positive terminal gain. Therefore **a [pricing kernel](../../../mathematical-finance.md#state-price-density) rules out [arbitrage](../../../mathematical-finance.md#arbitrage).**

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Write $q_{15},q_{12},q_9$ for the state probabilities under an [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure). Since cash is constant and the [European put option](../../../mathematical-finance.md#european-put-option) pays only in the lowest state, the pricing equations are

$$
q_{15}+q_{12}+q_9=1,\qquad15q_{15}+12q_{12}+9q_9=10,\qquad2q_9=\xi_0.
$$

Their unique solution is $q_9=\xi_0/2$, $q_{15}=\xi_0/2-2/3$, $q_{12}=5/3-\xi_0$. Every physical state has positive [probability](../../../probability-theory.md#probability), so equivalence requires all three values to be strictly positive. Thus

$$
\boxed{\frac43<\xi_0<\frac53.}
$$

For each price in this open interval the [pricing kernel](../../../mathematical-finance.md#state-price-density) takes values $3q_{15},3q_{12},3q_9$ in the three equally likely states, proving absence of [arbitrage](../../../mathematical-finance.md#arbitrage).

The necessity, including the exclusion of endpoints, can also be checked directly. The three terminal payoff vectors of cash, the [stock](../../../mathematical-finance.md#stock) and the [European put option](../../../mathematical-finance.md#european-put-option) form the invertible matrix

$$
\begin{pmatrix}1&15&0\\1&12&0\\1&9&2\end{pmatrix},\qquad\det=-6.
$$

Each unit state payoff therefore has a [replicating strategy](../../../mathematical-finance.md#replicating-strategy), whose initial cost is the corresponding $q$. A zero or negative $q$ supplies an [arbitrage](../../../mathematical-finance.md#arbitrage), so the endpoints are genuinely excluded.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Write $(a,b,c)$ for holdings of cash, the [stock](../../../mathematical-finance.md#stock) and the [European put option](../../../mathematical-finance.md#european-put-option), and let $\gamma=-V_0$ be initial [consumption](../../../mathematical-finance.md#consumption). At the given price, $a=-10b-c-\gamma$, and the three terminal payoffs, in descending order of the [stock](../../../mathematical-finance.md#stock) price, are

$$
5b-c-\gamma,\qquad2b-c-\gamma,\qquad c-b-\gamma.
$$

Nonnegative terminal payoffs require $c+\gamma\leq2b$ and $c-\gamma\geq b$. Together with $\gamma\geq0$, these imply $b\geq2\gamma\geq0$. If $b=0$ they force $\gamma=c=a=0$, which is not an [arbitrage](../../../mathematical-finance.md#arbitrage). If $b>0$, the highest-state payoff is at least $3b>0$, so every such choice is an [arbitrage](../../../mathematical-finance.md#arbitrage). Consequently the complete set is

$$
\boxed{(a,b,c)=(-10b-c-\gamma,b,c),\quad b>0,\quad0\leq\gamma\leq b/2,\quad b+\gamma\leq c\leq2b-\gamma.}
$$

The [pure-investment arbitrages](../../../mathematical-finance.md#pure-investment-arbitrage) are exactly the choices $\gamma=0$:

$$
\boxed{(a,b,c)=(-10b-c,b,c),\quad b>0,\quad b\leq c\leq2b.}
$$

For example, $(a,b,c)=(-11,1,1)$ costs zero and pays $(4,1,0)$.

## 2

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $\tau_n\uparrow\infty$ be a [localizing sequence](../../../martingale.md#localizing-sequence) for the discrete-time [local martingale](../../../martingale.md#local-martingale) $X$. For $t\geq1$, the increment of the stopped [martingale](../../../martingale.md) is

$$
X_{t\wedge\tau_n}-X_{(t-1)\wedge\tau_n}=\mathbf1_{\{\tau_n\geq t\}}(X_t-X_{t-1}),
$$

and $\{\tau_n\geq t\}\in\mathcal F_{t-1}$. Thus, for any $A\in\mathcal F_{t-1}$,

$$
\mathbb E[\mathbf1_A\mathbf1_{\{\tau_n\geq t\}}(X_t-X_{t-1})]=0.
$$

The assumed integrability gives the dominating [random variable](../../../random-variable.md) $|X_t|+|X_{t-1}|$. The [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) now yields $\mathbb E[\mathbf1_A(X_t-X_{t-1})]=0$, or $\mathbb E[X_t\mid\mathcal F_{t-1}]=X_{t-1}$. Iterating the [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation) proves **an integrable discrete-time [local martingale](../../../martingale.md#local-martingale) is a true [martingale](../../../martingale.md).** The proof uses the discrete-time increment indicator; the conclusion does not extend to continuous time.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Under the standard [local martingale](../../../martingale.md#local-martingale) definition, $X_0$ is integrable. For a nonnegative $X$, the [Fatou lemma](../../../measure-theory.md#fatou-s-lemma) and a [localizing sequence](../../../martingale.md#localizing-sequence) give

$$
\mathbb EX_t\leq\liminf_n\mathbb EX_{t\wedge\tau_n}=\mathbb EX_0<\infty.
$$

Hence every $X_t$ is integrable, and part (a) applies. Therefore **a nonnegative discrete-time [local martingale](../../../martingale.md#local-martingale) is a true [martingale](../../../martingale.md).** This is stronger than the continuous-time [supermartingale](../../../martingale.md#supermartingale) conclusion.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Take an increasing [localizing sequence](../../../martingale.md#localizing-sequence) $\tau_n$ for $X$ and define the [stopping times](../../../martingale.md#stopping-time)

$$
R_n=\inf\{u\geq0:|K_{u+1}|>n\},\qquad T_n=\tau_n\wedge R_n\wedge n.
$$

The [predictable process](../../../martingale.md#predictable-process) condition $K_{u+1}\in\mathcal F_u$ makes $R_n$ a [stopping time](../../../martingale.md#stopping-time). For each fixed finite time range, the finitely many coefficients $K_1,\ldots,K_t$ are finite [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence); hence $T_n\uparrow\infty$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence).

The stopped [martingale transform](../../../martingale.md#martingale-transform) can be written

$$
M_{t\wedge T_n}=\sum_{s=1}^tK_s\mathbf1_{\{R_n\geq s\}}\mathbf1_{\{n\geq s\}}\bigl(X_{s\wedge\tau_n}-X_{(s-1)\wedge\tau_n}\bigr).
$$

Its coefficient is $\mathcal F_{s-1}$-measurable and bounded in absolute value by $n$. Each summand is consequently integrable with zero [conditional expectation](../../../measure-theory.md#conditional-expectation) given $\mathcal F_{s-1}$, since $X^{\tau_n}$ is a true [martingale](../../../martingale.md). Thus $M^{T_n}$ is a true [martingale](../../../martingale.md) and

$$
\boxed{M=K\mathbin\cdot X\ \text{is a local martingale}.}
$$

The original PDF fixes $M_0=0$; the TeX extraction omits this equality.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

For fixed integers $s\leq t$, $A_s=\{\tau=s\}$ belongs to $\mathcal F_s$ and $X_s=0$ there. The [supermartingale](../../../martingale.md#supermartingale) property and nonnegativity imply

$$
0\leq\mathbb E[\mathbf1_{A_s}X_t]\leq\mathbb E[\mathbf1_{A_s}X_s]=0.
$$

Therefore $X_t=0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) on $A_s$. Taking the finite union over $s\leq t$ gives $X_t=0$ on $\{\tau\leq t\}$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence); taking the countable intersection over all integer $t$ makes the assertion simultaneous at every time. Thus **zero is absorbing for a nonnegative [supermartingale](../../../martingale.md#supermartingale) in discrete time.**

## 3

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Assume the innovations are [independent](../../../random-variable.md#independent-random-variables) of the previous history and have finite [exponential moments](../../../probability-theory.md#exponential-moment) at every real argument, as required by the finite-valued affine definition. Conditioning on $X_{t-1}=x$ gives

$$
\log\mathbb E[e^{\theta X_t}\mid X_{t-1}=x]=a\theta x+b\theta+\psi(\theta).
$$

Hence the [autoregressive process of order one](../../../time-series.md#autoregressive-process-of-order-one) is an [affine process](../../../markov-process.md#affine-process), with

$$
\boxed{A(\theta)=a\theta,\qquad B(\theta)=b\theta+\psi(\theta).}
$$

Here and in the remaining parts, an [affine process](../../../markov-process.md#affine-process) uses a time-homogeneous [Markov process](../../../markov-process.md): the one-step transform is the same at every time. The displayed definition at time $1$ alone would not determine later transitions of an arbitrary time-inhomogeneous [Markov process](../../../markov-process.md).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Use the [time-homogeneous Markov property](../../../markov-process.md#time-homogeneous-markov-property) and define backward effective parameters by

$$
q_t=\theta_t,\qquad q_j=\theta_j+A(q_{j+1})\quad(j=t-1,\ldots,1).
$$

Conditioning the last exponential factor on $\mathcal F_{t-1}$ replaces $\theta_tX_t$ by $A(q_t)X_{t-1}+B(q_t)$. Repeating the [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation) combines this with the preceding exponent, then with each earlier exponent. The last remaining conditional transform is at time $1$, so

$$
\boxed{A_t(\theta_1,\ldots,\theta_t)=A(q_1),\qquad B_t(\theta_1,\ldots,\theta_t)=\sum_{j=1}^t B(q_j).}
$$

These are finite because the one-step [affine process](../../../markov-process.md#affine-process) transforms are finite at every real parameter. The argument establishes the entire [joint affine transform](../../../markov-process.md#joint-affine-transform), including when the coefficients $\theta_j$ have different signs.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Iterating the [autoregressive process of order one](../../../time-series.md#autoregressive-process-of-order-one) gives

$$
X_j=a^jx+b\sum_{\ell=0}^{j-1}a^\ell+\sum_{r=1}^ja^{j-r}\xi_r.
$$

For $q_r=\sum_{j=r}^t\theta_ja^{j-r}$, regrouping the sum of the exponents gives

$$
\sum_{j=1}^t\theta_jX_j=x\sum_{j=1}^t\theta_ja^j+b\sum_{r=1}^tq_r+\sum_{r=1}^tq_r\xi_r.
$$

The [independent](../../../random-variable.md#independent-random-variables) innovations factorize the [moment-generating function](../../../probability-theory.md#moment-generating-function). Consequently

$$
\boxed{A_t=\sum_{j=1}^t\theta_ja^j,\qquad B_t=\sum_{r=1}^t\bigl(bq_r+\psi(q_r)\bigr),\qquad q_r=\sum_{j=r}^t\theta_ja^{j-r}.}
$$

Finite sums avoid a division by $a-1$, so these formulas include $a=0$ and $a=1$; zeroth powers in these sums are $1$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

A unit-face-value [zero-coupon bond](../../../mathematical-finance.md#zero-coupon-bond) pays $1$ at maturity. The [martingale deflator](../../../mathematical-finance.md#martingale-deflator) pricing identity is

$$
P_{t,T}=\frac{\mathbb E[Y_T\mid\mathcal F_t]}{Y_t}=\mathbb E\!\left[\exp\!\left(\sum_{j=t+1}^TX_j\right)\middle|\mathcal F_t\right].
$$

Use the [affine process](../../../markov-process.md#affine-process) [Markov property](../../../markov-process.md#markov-property) with respect to the market [filtration](../../../stochastic-process.md#filtration-probability-theory); if that [filtration](../../../stochastic-process.md#filtration-probability-theory) contains extra predictive information, the natural [Markov property](../../../markov-process.md#markov-property) alone would not suffice. Part (b), with every future coefficient equal to $1$, gives the exponential-affine form. More explicitly, the [exponential-affine bond pricing](../../../mathematical-finance.md#exponential-affine-bond-pricing) recursion is

$$
\boxed{\alpha(0)=\beta(0)=0,\quad\alpha(n+1)=A(1+\alpha(n)),\quad\beta(n+1)=\beta(n)+B(1+\alpha(n)).}
$$

Indeed, conditioning the first future step in an $(n+1)$-step horizon transforms $e^{(1+\alpha(n))X_{t+1}+\beta(n)}$ into $e^{A(1+\alpha(n))X_t+B(1+\alpha(n))+\beta(n)}$. Therefore

$$
\boxed{P_{t,T}=\exp\bigl(\alpha(T-t)X_t+\beta(T-t)\bigr).}
$$

This uses the true [martingale deflator](../../../mathematical-finance.md#martingale-deflator) pricing identity; a merely local [martingale deflator](../../../mathematical-finance.md#martingale-deflator) would not by itself justify replacing prices by conditional terminal [expectations](../../../probability-theory.md#expected-value).

## 4

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Since the initial value and increments are integers, $m=S_T-K$ is an integer. If $m\leq-1$, all three [positive parts](../../../function.md#positive-part-of-a-real-valued-function) in the second difference are zero. If $m\geq1$, the second difference is $(m-1)-2m+(m+1)=0$, including $m=1$. At $m=0$ it equals $0-0+1=1$. Thus

$$
\boxed{(S_T-K-1)^+-2(S_T-K)^++(S_T-K+1)^+=\mathbf1_{\{S_T=K\}}.}
$$

The original PDF has the first term $(S_T-K-1)^+$; the TeX's $(S_T-K+K)^+$ is an extraction error. This [discrete call-price curvature](../../../mathematical-finance.md#discrete-call-price-curvature) identity isolates an individual integer state.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For an integer $m$ and $d\in\{-1,0,1\}$, verify the single-step identity

$$
(m+d)^+-m^+=f(m)d+\frac12\mathbf1_{\{m=0\}}d^2.
$$

If $m\geq1$, the [positive part](../../../function.md#positive-part-of-a-real-valued-function) is linear across the step and $f(m)=1$; if $m\leq-1$, it remains zero and $f(m)=0$. At $m=0$, $d^+=(d+d^2)/2$, which is checked for the three permitted values of $d$.

Apply this with $m=S_{t-1}-K$ and $d=S_t-S_{t-1}$, and telescope over $t$. The result is the [discrete Tanaka formula](../../../stochastic-calculus.md#discrete-tanaka-formula)

$$
\boxed{(S_T-K)^+=(S_0-K)^++\sum_{t=1}^Tf(S_{t-1}-K)\Delta S_t+\frac12\sum_{t=1}^T\mathbf1_{\{S_{t-1}=K\}}(\Delta S_t)^2.}
$$

The first sum is a [martingale transform](../../../martingale.md#martingale-transform); the second records the correction at the kink of the [positive part](../../../function.md#positive-part-of-a-real-valued-function). The algebraic identity itself needs only the integer values and permitted increments, not the [martingale](../../../martingale.md) property.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Taking [expectations](../../../probability-theory.md#expected-value) in the single-step [discrete Tanaka formula](../../../stochastic-calculus.md#discrete-tanaka-formula), the [martingale transform](../../../martingale.md#martingale-transform) term vanishes because $f$ is bounded and $\mathcal F_T$-measurable. Hence

$$
C(T+1,K)-C(T,K)=\frac12\mathbb E[\mathbf1_{\{S_T=K\}}(S_{T+1}-S_T)^2].
$$

At a state with $p_K=\mathbb P(S_T=K)>0$, the [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation) gives $\mathbb E[S_{T+1}\mid S_T=K]=K$, so the conditional second [moment](../../../probability-theory.md#moment) of the increment is $\sigma^2(T,K)$. Part (a) gives $p_K=C(T,K+1)-2C(T,K)+C(T,K-1)$. Combining these identities yields the [discrete Dupire equation](../../../mathematical-finance.md#discrete-dupire-equation)

$$
\boxed{C(T+1,K)-C(T,K)=\frac12\sigma^2(T,K)\bigl(C(T,K+1)-2C(T,K)+C(T,K-1)\bigr).}
$$

**The conditional [variance](../../../variance.md) needs a positive-probability conditioning state.** The bound $|K-S_0|\leq T$ does not guarantee $p_K>0$. If $p_K=0$, both the [call-price curvature](../../../mathematical-finance.md#discrete-call-price-curvature) and the time increment above are zero; the equation can be extended by assigning an arbitrary finite value to $\sigma^2(T,K)$ at such a state, but its conditional [variance](../../../variance.md) is not determined there.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Let $p_K=C(T,K+1)-2C(T,K)+C(T,K-1)>0$ and $D_K=C(T+1,K)-C(T,K)$. Given $S_T=K$, the next value is one of $K-1,K,K+1$. The [martingale](../../../martingale.md) property makes its upward and downward conditional probabilities equal; their sum is the conditional [variance](../../../variance.md) of the increment, $\sigma^2(T,K)=2D_K/p_K$. Thus

$$
\boxed{\mathbb P(S_{T+1}=H\mid S_T=K)=\begin{cases}D_K/p_K,&H=K-1\text{ or }K+1,\\1-2D_K/p_K,&H=K,\\0,&\text{otherwise}.\end{cases}}
$$

The [discrete Dupire equation](../../../mathematical-finance.md#discrete-dupire-equation) therefore recovers all positive-probability one-step conditional transitions from the [European call option](../../../mathematical-finance.md#european-call-option) price surface. No [Markov property](../../../markov-process.md#markov-property) is required: these are conditional probabilities given the current value, not necessarily given the whole past.

**Recovery is impossible at a zero-probability state.** For example, $S_t\equiv S_0$ satisfies every stated assumption, but at $T\geq1$ a different integer $K$ can satisfy $|K-S_0|\leq T$ while $p_K=0$. Its conditional transitions can be specified arbitrarily without altering $C$. Thus the literal all-states claim needs the positive-probability qualification.

## 5

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

For a fixed realization $\xi=a$ and $\operatorname{Re}z>1$, direct integration gives

$$
\begin{aligned}
\int_{-\infty}^{\infty}(e^a-e^k)^+z(z-1)e^{(z-1)k}\,dk
&=z(z-1)\int_{-\infty}^a(e^a-e^k)e^{(z-1)k}\,dk\\
&=z(z-1)\left(\frac{e^{za}}{z-1}-\frac{e^{za}}z\right)=e^{za}.
\end{aligned}
$$

To interchange the integral and [expectation](../../../probability-theory.md#expected-value), write $x=\operatorname{Re}z>1$ and estimate

$$
\mathbb E\int_{-\infty}^{\infty}\left|(e^\xi-e^k)^+z(z-1)e^{(z-1)k}\right|dk
=\frac{|z(z-1)|}{x(x-1)}\mathbb Ee^{x\xi}<\infty.
$$

The [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem) now proves the [Mellin transform of call prices](../../../analysis.md#mellin-transform-of-call-prices) identity

$$
\boxed{M(z)=\int_{-\infty}^{\infty}C(k)z(z-1)e^{(z-1)k}\,dk\qquad(\operatorname{Re}z>1).}
$$

The required [exponential moment](../../../probability-theory.md#exponential-moment) is $\mathbb Ee^{x\xi}<\infty$ at the chosen real part; the assertion for every $x>1$ presupposes these [exponential moments](../../../probability-theory.md#exponential-moment) for every such $x$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Set $z=x_0+iy$. Since $|M(z)|\leq\mathbb Ee^{x_0\xi}$ and $|z(z-1)|^{-1}$ is integrable over $y\in\mathbb R$, the proposed contour integral is absolutely convergent. The same bound justifies the [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem) when substituting $M(z)=\mathbb Ee^{z\xi}$:

$$
\begin{aligned}
\frac1{2\pi i}\int_{x_0-i\infty}^{x_0+i\infty}\frac{M(z)}{z(z-1)e^{(z-1)k}}\,dz
&=e^k\mathbb E\!\left[\frac1{2\pi i}\int_{x_0-i\infty}^{x_0+i\infty}\frac{e^{z(\xi-k)}}{z(z-1)}\,dz\right]\\
&=e^k\mathbb E(e^{\xi-k}-1)^+=C(k).
\end{aligned}
$$

The last equality uses the contour identity provided in the original PDF. Consequently

$$
\boxed{C(k)=\frac1{2\pi i}\int_{x_0-i\infty}^{x_0+i\infty}\frac{M(z)}{f(z,k)}\,dz\qquad(x_0>1).}
$$

This is [contour inversion for call prices](../../../mathematical-finance.md#contour-inversion-for-call-prices). The supplied TeX corrupts the permitted identity into a reciprocal and drops the imaginary units from its endpoints; the PDF has $(e^a-1)^+$ and the vertical contour used above.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Assume the usual positive initial [stock](../../../mathematical-finance.md#stock) price and strike, so the logarithm is defined, and interpret $U$ as a classical solution of the displayed [partial differential equation](../../../partial-differential-equation.md). For a fixed complex $z$, put $F_t(z)=S_t^zU(t,\sigma_t,z)$, defining $S_t^z=\exp(z\log S_t)$. The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) for the two [Brownian motions](../../../brownian-motion.md) with [correlation coefficient](../../../variance.md#pearson-correlation-coefficient) $\rho$ gives

$$
\begin{aligned}
dF_t(z)=S_t^z\bigg(&U_t+A(\sigma_t)U_\sigma+\frac12B(\sigma_t)^2U_{\sigma\sigma}+\frac12\sigma_t^2z(z-1)U+z\sigma_tB(\sigma_t)\rho U_\sigma\bigg)dt\\
&+S_t^z\bigl(z\sigma_tU\,dW_t^S+B(\sigma_t)U_\sigma\,dW_t^\sigma\bigr).
\end{aligned}
$$

The [partial differential equation](../../../partial-differential-equation.md) cancels the entire [drift](../../../stochastic-calculus.md#drift-coefficient). By the permission to treat the resulting [local martingales](../../../martingale.md#local-martingale) as true [martingales](../../../martingale.md), and the terminal condition, $F_t(z)=\mathbb E[S_T^z\mid\mathcal F_t]$.

The bounded [spot volatility](../../../mathematical-finance.md#spot-volatility) ensures $\mathbb ES_T^{x_0}<\infty$: the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) for a real power and localization bound its [moment](../../../probability-theory.md#moment) by $S_0^{x_0}\exp(x_0(x_0-1)\|\sigma\|_\infty^2T/2)$. Rewrite the proposed integrand as

$$
\frac{S_tU(t,\sigma_t,z)}{f(z,\log(K/S_t))}=\frac{K^{1-z}F_t(z)}{z(z-1)}.
$$

Now $|F_t(x_0+iy)|\leq\mathbb E[S_T^{x_0}\mid\mathcal F_t]$, an integrable bound independent of $y$. Conditional [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem) and part (b) therefore imply

$$
\boxed{C_t=\mathbb E[(S_T-K)^+\mid\mathcal F_t].}
$$

This route justifies the contour exchange without assuming bounds on $U$ uniform in all complex $z$. Cash is constant, $S$ is a true [martingale](../../../martingale.md) under the stated allowance, and the displayed $C$ is a true [martingale](../../../martingale.md). The original measure is thus an [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure) for all three assets. The [fundamental theorem of asset pricing](../../../mathematical-finance.md#fundamental-theorem-of-asset-pricing) gives **the market has no [arbitrage](../../../mathematical-finance.md#arbitrage) under the usual admissible trading convention.**

## 6

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Use positive initial asset prices and the usual augmentation of the [natural Brownian filtration](../../../brownian-motion.md#natural-brownian-filtration). Define the [market price of risk](../../../mathematical-finance.md#market-price-of-risk)

$$
\boxed{\lambda_t=\frac{\mu_t-r_t}{\sigma_t}.}
$$

Continuity and strict positivity of $\sigma$ imply $\int_0^T\lambda_t^2dt<\infty$ on every finite horizon [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), because each path has a positive minimum of $\sigma$ there. Hence the strictly positive [stochastic exponential](../../../stochastic-calculus.md#doleans-dade-exponential)

$$
\boxed{Y_t=\exp\!\left(-\int_0^tr_sds-\int_0^t\lambda_s\,dW_s-\frac12\int_0^t\lambda_s^2ds\right)}
$$

is defined and has $Y_0=1$ and $dY_t=-Y_t(r_tdt+\lambda_tdW_t)$. The [Itô product rule](../../../stochastic-calculus.md#ito-product-rule) gives

$$
d(Y_tB_t)=-Y_tB_t\lambda_t\,dW_t,\qquad d(Y_tS_t)=Y_tS_t(\sigma_t-\lambda_t)\,dW_t,
$$

so it is a [local martingale deflator](../../../mathematical-finance.md#local-martingale-deflator).

For uniqueness, let $\widetilde Y$ be any normalized strictly positive [local martingale deflator](../../../mathematical-finance.md#local-martingale-deflator). The [Brownian martingale representation theorem](../../../brownian-motion.md#brownian-martingale-representation-theorem) makes $B\widetilde Y$ a continuous [local martingale](../../../martingale.md#local-martingale) with a [Brownian motion](../../../brownian-motion.md) integral representation. Dividing by $B$ therefore gives $d\widetilde Y=-r\widetilde Ydt+\eta dW$. The vanishing [drift](../../../stochastic-calculus.md#drift-coefficient) of $S\widetilde Y$ requires $\widetilde Y(\mu-r)+\eta\sigma=0$, so $\eta=-\widetilde Y\lambda$. This scalar linear [stochastic differential equation](../../../stochastic-calculus.md#stochastic-differential-equation) has exactly the exponential solution above, proving **the normalized [local martingale deflator](../../../mathematical-finance.md#local-martingale-deflator) is unique.**

The assumptions do not make $\lambda$ deterministically bounded: $\sigma$ need not be bounded away from zero uniformly over outcomes. Thus a true [martingale](../../../martingale.md) density or [Novikov condition](../../../stochastic-calculus.md#novikov-s-condition) is not inferred here; the required conclusion is local.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Let $\theta_t$ and $\eta_t$ be the [predictable](../../../martingale.md#predictable-process) holdings of the [stock](../../../mathematical-finance.md#stock) and the [bank account](../../../mathematical-finance.md#bank-account). With no [consumption](../../../mathematical-finance.md#consumption), the [self-financing portfolio](../../../mathematical-finance.md#self-financing-portfolio) has $X=\theta S+\eta B$ and $dX=\theta dS+\eta dB$. The [Itô product rule](../../../stochastic-calculus.md#ito-product-rule), together with the dynamics from part (a), gives

$$
\begin{aligned}
d(X_tY_t)
&=\bigl(Y_t\theta_tS_t\mu_t+Y_t\eta_tB_tr_t-r_tX_tY_t-Y_t\theta_tS_t\sigma_t\lambda_t\bigr)dt\\
&\quad+Y_t(\theta_tS_t\sigma_t-X_t\lambda_t)\,dW_t\\
&=Y_t(\theta_tS_t\sigma_t-X_t\lambda_t)\,dW_t.
\end{aligned}
$$

The [drift](../../../stochastic-calculus.md#drift-coefficient) vanishes because $X=\theta S+\eta B$ and $\sigma\lambda=\mu-r$. Thus $XY$ is a [local martingale](../../../martingale.md#local-martingale). It is nonnegative by the assumed nonnegative wealth and strict positivity of $Y$, and hence

$$
\boxed{XY\ \text{is a supermartingale}.}
$$

For example, this last fact follows directly from [Conditional Fatou lemma](../../../measure-theory.md#conditional-fatou-lemma) applied to a [localizing sequence](../../../martingale.md#localizing-sequence); the initial capital is assumed finite. As usual, holdings must be integrable against the asset [semimartingales](../../../stochastic-calculus.md#semimartingale) for the [self-financing portfolio](../../../mathematical-finance.md#self-financing-portfolio) equation to be defined.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Fix the maturity horizon. Since $YB$ is a nonnegative [local martingale](../../../martingale.md#local-martingale) and $r$ is bounded, $\mathbb EY_T<\infty$: $B_T\geq B_0e^{-\|r\|_\infty T}$ and $\mathbb E(Y_TB_T)\leq B_0$. The bounded nonnegative payoff thus makes $Y_T\xi_T$ integrable. Set

$$
N_t=\mathbb E[Y_T\xi_T\mid\mathcal F_t],\qquad X_t=\frac{N_t}{Y_t}.
$$

The [Brownian martingale representation theorem](../../../brownian-motion.md#brownian-martingale-representation-theorem) yields $N_t=N_0+\int_0^t\zeta_s\,dW_s$, using its locally [square-integrable](../../../measure-theory.md#square-integrable-function) version for an integrable terminal [random variable](../../../random-variable.md). The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) for $N/Y$ gives

$$
dX_t=\bigl(r_tX_t+\lambda_t(\zeta_t/Y_t+\lambda_tX_t)\bigr)dt+(\zeta_t/Y_t+\lambda_tX_t)\,dW_t.
$$

Choose the [replicating strategy](../../../mathematical-finance.md#replicating-strategy)

$$
\boxed{\theta_t=\frac{\zeta_t/Y_t+\lambda_tX_t}{S_t\sigma_t},\qquad\eta_t=\frac{X_t-\theta_tS_t}{B_t}.}
$$

Its [self-financing portfolio](../../../mathematical-finance.md#self-financing-portfolio) equation has exactly the displayed [drift](../../../stochastic-calculus.md#drift-coefficient) and diffusion, because $\mu-r=\sigma\lambda$. All coefficients are locally integrable after stopping; the holdings are [predictable](../../../martingale.md#predictable-process) in the augmented [natural Brownian filtration](../../../brownian-motion.md#natural-brownian-filtration). This construction has $X_t\geq0$ and $X_T=\xi_T$, so it is an admissible [replicating strategy](../../../mathematical-finance.md#replicating-strategy) under the question's nonnegative-wealth convention.

For any other nonnegative [self-financing portfolio](../../../mathematical-finance.md#self-financing-portfolio) $\widehat X$ replicating the same payoff, part (b) implies $\widehat X_0\geq\mathbb E[Y_T\xi_T]$. The constructed strategy attains equality, since $Y_0=1$ and $N_0=\mathbb E[Y_T\xi_T]$ in the augmented [natural Brownian filtration](../../../brownian-motion.md#natural-brownian-filtration). Hence

$$
\boxed{\text{minimal initial cost}=\mathbb E[Y_T\xi_T].}
$$

This is [deflator-based claim replication](../../../mathematical-finance.md#deflator-based-claim-replication); it does not require upgrading the [local martingale deflator](../../../mathematical-finance.md#local-martingale-deflator) to a true [martingale](../../../martingale.md) density.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

With constant coefficients, $\lambda=(\mu-r)/\sigma$ is constant, so the [stochastic exponential](../../../stochastic-calculus.md#doleans-dade-exponential) $Z_t=e^{rt}Y_t$ is a true [martingale](../../../martingale.md). Under its [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure) $\mathbb Q$, the [stock](../../../mathematical-finance.md#stock) follows the [Black-Scholes model](../../../mathematical-finance.md#black-scholes-model) $dS_t=S_t(rdt+\sigma dW_t^{\mathbb Q})$. The Gaussian exponential [moment](../../../probability-theory.md#moment) gives the value of the [power option](../../../mathematical-finance.md#power-option)

$$
V_t=e^{-r(T-t)}\mathbb E_{\mathbb Q}[\sqrt{S_T}\mid\mathcal F_t]=\sqrt{S_t}\exp\!\left(-\left(\frac r2+\frac{\sigma^2}8\right)(T-t)\right).
$$

The [option delta](../../../mathematical-finance.md#option-delta) is $\partial_sV=V/(2s)$, so the [replicating strategy](../../../mathematical-finance.md#replicating-strategy) holds

$$
\boxed{\theta_t=\frac{V_t}{2S_t},\qquad\eta_t=\frac{V_t}{2B_t},\qquad V_0=\sqrt{S_0}\exp\!\left(-\left(\frac r2+\frac{\sigma^2}8\right)T\right).}
$$

Half the wealth value is in the [stock](../../../mathematical-finance.md#stock) and half in the [bank account](../../../mathematical-finance.md#bank-account), with continuous rebalancing. To check the [self-financing portfolio](../../../mathematical-finance.md#self-financing-portfolio) property under the original measure, the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives $dV_t=\frac12(r+\mu)V_tdt+\frac12\sigma V_tdW_t=\theta_tdS_t+\eta_tdB_t$. Also $V_T=\sqrt{S_T}$ and $V_t>0$.

The payoff is unbounded, so the bounded-payoff restriction of part (c) is not invoked automatically; the [Black-Scholes model](../../../mathematical-finance.md#black-scholes-model) has the necessary finite Gaussian [moments](../../../probability-theory.md#moment), and the explicit strategy attains $V_0=\mathbb E[Y_T\sqrt{S_T}]$. The [supermartingale](../../../martingale.md#supermartingale) bound from part (b) therefore proves its minimality. The cost is independent of the physical [drift](../../../stochastic-calculus.md#drift-coefficient) $\mu$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
