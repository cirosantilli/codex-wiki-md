# Paper 40

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_40.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_40.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [a](#2/a)
    - [1](#2/a/1)
      - [Solution](#2/a/1/solution)
    - [2](#2/a/2)
      - [Solution](#2/a/2/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
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

## 1

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Put $\mathcal L_rV(s)=\frac12\sigma^2s^2V''(s)+rsV'(s)$ and define the nonnegative reserve rate $a(s)=rV(s)-\mathcal L_rV(s)$. The [obstacle problem](../../../partial-differential-equation.md#obstacle-problem) gives $V\geq g$ and $a\geq0$. The [American-option superhedge with a funded reserve](../../../mathematical-finance.md#american-option-superhedge-with-a-funded-reserve) invests the local surplus in the bond rather than consuming it.

For initial wealth $x\geq V(S_0)$, set

$$
D_t=e^{rt}\left(x-V(S_0)+\int_0^te^{-ru}a(S_u)\,du\right),\qquad F_t=V(S_t)+D_t,
$$

and choose the [stock](../../../mathematical-finance.md#stock) and bond holdings

$$
\boxed{\pi_t=V'(S_t),\qquad \phi_t=\frac{F_t-\pi_tS_t}{B_t}.}
$$

Thus $D_t\geq0$ and $F_t\geq V(S_t)\geq g(S_t)$, pathwise at every time. The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) under the original drift gives

$$
dV(S_t)=V'(S_t)\,dS_t+\tfrac12\sigma^2S_t^2V''(S_t)\,dt,
\qquad dD_t=(rD_t+a(S_t))\,dt.
$$

Adding these equations yields

$$
\boxed{dF_t=\pi_t\,dS_t+r(F_t-\pi_tS_t)\,dt
=\pi_t\,dS_t+\phi_t\,dB_t.}
$$

This is a [self-financing strategy](../../../mathematical-finance.md#self-financing-portfolio), and its nonnegative wealth makes it an [admissible trading strategy](../../../mathematical-finance.md#admissible-trading-strategy). Continuity of the [stock](../../../mathematical-finance.md#stock) and local regularity of $V$ ensure local integrability of the holdings. The construction does not require $\mu=r$.

For a classical solution, the usual [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) applies directly. The [smooth fit](../../../martingale.md#smooth-pasting) solution below is $C^1$ and piecewise $C^2$, with locally absolutely continuous first derivative. The generalized [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) applies with its almost-everywhere second derivative; the absence of a derivative jump means no boundary [local time of a semimartingale](../../../stochastic-calculus.md#local-time-of-a-semimartingale) term. This is the usual regularity interpretation of the perpetual [American option](../../../mathematical-finance.md#american-option) obstacle equation.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Write $\alpha=2r/\sigma^2\in(0,1)$. In a continuation interval, the [Euler differential equation](../../../differential-equation.md#cauchy-euler-equation) has power solutions $s$ and $s^{-\alpha}$: substitution of $s^\beta$ gives $(\beta-1)(\beta+\alpha)=0$. A decreasing bounded value uses the second solution.

Let $b$ be the exercise boundary. Value matching and [smooth fit](../../../martingale.md#smooth-pasting) require $Ab^{-\alpha}=(1+b)^{-1}$ and $-\alpha Ab^{-\alpha-1}=-(1+b)^{-2}$. Dividing gives $b/(1+b)=\alpha$. Consequently

$$
\boxed{b=\frac\alpha{1-\alpha},\qquad
V(s)=\begin{cases}
(1+s)^{-1},&0<s\leq b,\\
\displaystyle\frac1{1+b}\left(\frac{s}{b}\right)^{-\alpha},&s>b.
\end{cases}}
$$

This is a [perpetual reciprocal-payoff American option](../../../mathematical-finance.md#perpetual-reciprocal-payoff-american-option).

To verify the obstacle inequality, observe that $s^\alpha/(1+s)$ increases up to $b$ and decreases afterwards, because its logarithmic derivative is $\alpha/s-1/(1+s)$. Therefore $V(s)\geq(1+s)^{-1}$ for $s>b$. In the continuation region $(\mathcal L_r-r)V=0$. In the exercise region,

$$
(\mathcal L_r-r)g(s)
=\frac{\sigma^2}{(1+s)^3}
\left((1-\alpha)s^2-\frac{3\alpha}2s-\frac\alpha2\right).
$$

The quadratic is convex. At the two endpoints of $[0,b]$ it equals $-\alpha/2$ and $-\alpha/[2(1-\alpha)]$, respectively, so it is negative throughout that interval. Thus the [obstacle problem](../../../partial-differential-equation.md#obstacle-problem) is satisfied on both regions, with value matching and [smooth fit](../../../martingale.md#smooth-pasting) at $b$. The second derivative has a jump at $b$; the equation is understood piecewise and in the generalized Itô sense described in part (a).

For optimality, use the [Risk-neutral measure for the Black-Scholes model](../../../mathematical-finance.md#risk-neutral-measure-for-the-black-scholes-model), under which $dS_t=rS_tdt+\sigma S_tdW_t^{\mathbb Q}$. The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) makes $e^{-rt}V(S_t)$ a nonnegative [supermartingale](../../../martingale.md#supermartingale), so every exercise time $\tau$ satisfies

$$
\mathbb E_{\mathbb Q}[e^{-r\tau}g(S_\tau)1_{\{\tau<\infty\}}]\leq V(S_0).
$$

Before hitting the exercise region, its drift vanishes. Since $0\leq V\leq1$, the stopped process is a bounded [martingale](../../../martingale.md). Apply the [optional sampling theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) at $\tau_*\wedge T$ and let $T\to\infty$. The contribution from $\{\tau_*>T\}$ is at most $e^{-rT}$, while the boundary value equals the payoff. Hence equality holds for

$$
\boxed{\tau_*=\inf\{t\geq0:S_t\leq b\}.}
$$

If $S_0\leq b$, exercise immediately; otherwise wait for the first down-crossing. If that time is infinite, the discounted payout is zero. This proves both the value and the [optimal stopping](../../../martingale.md#optimal-stopping) policy, and part (a) supplies its [superhedge](../../../mathematical-finance.md#superhedging).

<a id="1/b/image-perpetual-reciprocal-payoff-option-value-and-exercise-boundary-for-two-interest-to-variance-ratios"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-40-perpetual-boundary.png)

**[Figure 1](#1/b/image-perpetual-reciprocal-payoff-option-value-and-exercise-boundary-for-two-interest-to-variance-ratios). Perpetual reciprocal-payoff option value and exercise boundary for two interest-to-variance ratios**.

## 2

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/1">1</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/1/solution">Solution</h5>

↑ **Parent:** [1](#2/a/1)

Interpret positivity of $Y$ as strict positivity almost surely. Suppose the stated bounded positive pricing variable exists. For a vector $H$ satisfying the two sign restrictions,

$$
0\geq H\cdot p=\mathbb E[Y(H\cdot P)]\geq0.
$$

A nonnegative random variable with zero expectation vanishes almost surely. Since $Y>0$, this gives $H\cdot P=0$ almost surely and $H\cdot p=0$. The supplied nondegeneracy condition now yields $\boxed{H=0}$. This proves the direction from a [one-period martingale deflator](../../../mathematical-finance.md#one-period-martingale-deflator) to the separating-portfolio condition; no asset-pricing theorem has been invoked.

<h4 id="2/a/2">2</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/2/solution">Solution</h5>

↑ **Parent:** [2](#2/a/2)

A direct [exponential minimization construction of a bounded pricing kernel](../../../mathematical-finance.md#exponential-minimization-construction-of-a-bounded-pricing-kernel) proves the reverse implication without using a course theorem. Consider

$$
F(h)=\mathbb E[e^{-h\cdot P}]+h\cdot p,\qquad h\in\mathbb R^n.
$$

Boundedness of $P$ makes $F$ finite, continuous, and differentiable. On every bounded set of $h$, the exponential and its derivatives have deterministic bounds, so differentiation under expectation is justified.

We first prove [coercivity](../../../real-analysis.md#coercive-function): $F(h)\to\infty$ as $|h|\to\infty$. Otherwise there would be a sequence $h_j$ with $|h_j|\to\infty$ along which $F(h_j)$ stays bounded above. Pass to a subsequence with $h_j/|h_j|\to u$, $|u|=1$. There are two cases.

If $\mathbb P(u\cdot P<0)>0$, choose $a>0$ with $\delta=\mathbb P(u\cdot P\leq-a)>0$. The bound on $P$ gives $h_j\cdot P\leq-a|h_j|/2$ on this event for all large $j$. Therefore

$$
F(h_j)\geq\delta e^{a|h_j|/2}-|p|\,|h_j|\longrightarrow\infty.
$$

If instead $u\cdot P\geq0$ almost surely, the portfolio condition forces $u\cdot p>0$, since $u\ne0$. Hence $h_j\cdot p\to\infty$, and the nonnegative exponential term again forces $F(h_j)\to\infty$. Both cases contradict the chosen sequence.

A minimizing sequence is consequently bounded. It has a convergent subsequence, and continuity of $F$ gives a global minimizer $h_*$. At a minimizer each directional derivative vanishes, so

$$
0=\nabla F(h_*)=p-\mathbb E[Pe^{-h_*\cdot P}].
$$

Thus

$$
\boxed{Y=e^{-h_*\cdot P}>0,\qquad \mathbb E[PY]=p.}
$$

If $|P|\leq L$, then $e^{-|h_*|L}\leq Y\leq e^{|h_*|L}$: the constructed [pricing kernel](../../../mathematical-finance.md#state-price-density) is bounded and even bounded away from zero. The compactness, coercivity, and differentiation arguments above supply the needed proof rather than appealing to the [fundamental theorem of asset pricing](../../../mathematical-finance.md#fundamental-theorem-of-asset-pricing).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Use the positive variable $Y$ from part (a). Since $0\leq(S-B)^+\leq S$ and $(S-B)^+\geq S-B$,

$$
0\leq c=\mathbb E[Y(S-B)^+]\leq\mathbb E[YS]=s,
\qquad c\geq\mathbb E[Y(S-B)]=s-b.
$$

Combining these inequalities gives the [one-period call price bounds](../../../mathematical-finance.md#one-period-call-price-bounds)

$$
\boxed{(s-b)^+\leq c\leq s.}
$$

For the strict assertion, both $\{S>B\}$ and $\{S<B\}$ have positive probability. Positivity of $Y$ gives

$$
c=\mathbb E[Y(S-B)^+]>0,
\qquad c-(s-b)=\mathbb E[Y(B-S)^+]>0.
$$

If $s-b\geq0$, the second inequality is the required strict bound; if $s-b<0$, the first is. Hence $\boxed{c>(s-b)^+}$. The weighted expectations are finite because $P$ and $Y$ are bounded.

## 3

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [complete market](../../../mathematical-finance.md#complete-market) permits [claim replication](../../../mathematical-finance.md#claim-replication) for every finite maturity and every bounded claim measurable at that maturity: there are an initial capital and a predictable [self-financing portfolio](../../../mathematical-finance.md#self-financing-portfolio) whose terminal wealth equals the claim almost surely. In a finite-state market this is equivalent to replicating every terminal payoff, since all such payoffs are bounded. Trading is allowed dynamically in the existing $n$ assets; adding a new security is not part of the definition.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

We prove the stronger [finite branching bound in a complete market](../../../mathematical-finance.md#finite-branching-bound-in-a-complete-market): modulo null sets, $\mathcal F_t$ is generated by at most $n^t$ atoms. Here an atom is a positive-probability event which cannot be split into two positive-probability measurable pieces.

At time zero there is one atom because $\mathcal F_0$ is trivial. Suppose $\mathcal F_{t-1}$ has at most $n^{t-1}$ atoms, and fix one such atom $A$. Any [predictable process](../../../martingale.md#predictable-process) holdings over $(t-1,t]$ are constant on $A$, so the restriction to $A$ of every time-$t$ replicable payoff lies in

$$
\operatorname{span}\{P_t^1|_A,\ldots,P_t^n|_A\},
$$

a [vector space](../../../vector-space.md) of [dimension of a vector space](../../../vector-space.md#dimension-vector-space) at most $n$. If $A$ contained $n+1$ disjoint positive-probability $\mathcal F_t$ events, their indicators would have [linear independence](../../../vector-space.md#linear-independence) on $A$. [Market completeness](../../../mathematical-finance.md#complete-market) would replicate each indicator, contradicting that dimension bound.

For clarity, the absence of $n+1$ disjoint positive pieces implies that $A$ is a union of at most $n$ atoms: start with $A$ and repeatedly split any non-atom into two positive pieces. Each split increases the count by one. The process must stop before the count exceeds $n$, and at termination every piece is an atom. Thus each time-$(t-1)$ atom has at most $n$ successors. Induction gives at most $n^t$ atoms at time $t$.

Each disjoint positive-probability $\mathcal F_t$ event contains at least one distinct atom. Therefore

$$
\boxed{k\leq n^t.}
$$

The argument includes $t=0$ and uses the ability to replicate the indicator claims at every intermediate maturity.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Use the conditional second-moment matrix $V_t=\mathbb E[P_tP_t^\top\mid\mathcal F_{t-1}]$ from the PDF. By part (b), the filtration is finite-state at every finite time. On a time-$(t-1)$ atom let $p_1,\ldots,p_m$ be the successor price vectors and $q_1,\ldots,q_m>0$ their conditional probabilities. Then $m\leq n$ and

$$
V=\sum_{i=1}^m q_i p_i p_i^\top.
$$

Positive definiteness gives rank $n$, so $m\geq n$. Hence $m=n$, and the $n$ successor vectors have [linear independence](../../../vector-space.md#linear-independence).

We use the finite-horizon [fundamental theorem of asset pricing](../../../mathematical-finance.md#fundamental-theorem-of-asset-pricing) in deflator form: an arbitrage-free finite market admits a strictly positive adapted process $D$, with $D_0=1$, such that $DP$ is a [martingale](../../../martingale.md). Equivalently, on every step,

$$
\mathbb E[D_tP_t\mid\mathcal F_{t-1}]=D_{t-1}P_{t-1}.
$$

Fix a finite horizon containing the step in question. On the parent atom, write $d_i=D_t/D_{t-1}>0$ on successor $i$ and $p_0=P_{t-1}$. Then

$$
\sum_iq_i d_i p_i=p_0.
$$

The proposed values $z_i=p_i^\top V^{-1}p_0$ satisfy precisely the same equation:

$$
\sum_iq_i z_i p_i
=\left(\sum_iq_i p_i p_i^\top\right)V^{-1}p_0=p_0.
$$

Because the $p_i$ have [linear independence](../../../vector-space.md#linear-independence) and the $q_i$ are positive, this linear system has a unique solution. Thus $z_i=d_i>0$, proving

$$
\boxed{Z_t>0\quad\text{almost surely for every }t\geq1.}
$$

This is the [positive regression deflator in a complete finite market](../../../mathematical-finance.md#positive-regression-deflator-in-a-complete-finite-market). It also proves the suggested conclusion: with $Y_0=1$ and $Y_t=\prod_{u=1}^tZ_u$,

$$
\mathbb E[Y_tP_t\mid\mathcal F_{t-1}]
=Y_{t-1}\mathbb E[P_tP_t^\top\mid\mathcal F_{t-1}]V_t^{-1}P_{t-1}
=Y_{t-1}P_{t-1}.
$$

Hence $Y$ is a strictly positive [martingale deflator](../../../mathematical-finance.md#martingale-deflator). Finite-state structure makes these expectations integrable on each finite horizon. Positive definiteness alone would not ensure positivity of the regression factor; [market completeness](../../../mathematical-finance.md#complete-market) and the positive deflator are essential.

## 4

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For $S_0>0$, the [stochastic exponential](../../../stochastic-calculus.md#doleans-dade-exponential) solution stays strictly positive. Put $U_t=\sqrt{S_t}$. The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives

$$
\boxed{dU_t=\frac12U_t\sigma_t\,dW_t-\frac18U_t\sigma_t^2\,dt.}
$$

Thus $U$ is a nonnegative local [supermartingale](../../../martingale.md#supermartingale). To justify the true [supermartingale](../../../martingale.md#supermartingale) property, stop where $U$ or its stochastic integral exceeds successive bounds. The stopped [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives $\mathbb E[U_{T\wedge\tau_m}\mid\mathcal F_t]\leq U_{t\wedge\tau_m}$ for $T\geq t$. The conditional [Fatou lemma](../../../measure-theory.md#fatou-s-lemma) and $\tau_m\uparrow\infty$ yield

$$
\boxed{\mathbb E[U_T\mid\mathcal F_t]\leq U_t.}
$$

In particular $\mathbb EU_T\leq U_0<\infty$. The case $S_0=0$ is the identically zero process. This is the [square-root stock supermartingale](../../../martingale.md#square-root-stock-supermartingale).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The coefficient is $\boxed{k=1/8}$, but independence alone does not make the printed right-hand side $\mathcal F_t$-measurable. The future variance integral need not be known at time $t$. This is a genuine missing information assumption in the PDF.

The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) or explicit [stochastic exponential](../../../stochastic-calculus.md#doleans-dade-exponential) gives

$$
\frac{U_T}{U_t}
=\exp\left(\frac12\int_t^T\sigma_u\,dW_u
-\frac18\int_t^T\sigma_u^2\,du\right)
\exp\left(-\frac18\int_t^T\sigma_u^2\,du\right).
$$

If the volatility path is fixed at time zero and independent of $W$, conditioning on that path makes the first factor an exponential of a centered Gaussian variable with the compensating half-variance, so its conditional expectation is one. More generally, this conditioning works when enlarging the filtration by the entire independent volatility path preserves the Brownian property. For the usual joint filtration of Brownian history and independent volatility history, the valid [conditional square-root price under independent volatility](../../../mathematical-finance.md#conditional-square-root-price-under-independent-volatility) is

$$
\boxed{\mathbb E[U_T\mid\mathcal F_t]
=U_t\,\mathbb E\left[\exp\left(-\frac18\int_t^T\sigma_u^2du\right)\middle|\mathcal F_t\right].}
$$

When the integral is already $\mathcal F_t$-measurable, the outer conditional expectation can be removed, giving the intended printed formula. In particular this holds for deterministic volatility or an independent path disclosed initially.

For a counterexample to the unqualified printed assertion, take an independent fair Bernoulli variable $A\in\{0,1\}$, disclose it at time $1$, and let

$$
\sigma_u=A\min\{(u-1)^+,1\},\qquad S_0=1.
$$

With the filtration generated by the Brownian history and this disclosure, $W$ is Brownian and $\sigma$ is bounded, continuous, adapted, and independent of $W$. At $t=0,T=2$, the variance integral is $A/3$, while $\mathcal F_0$ is trivial. Direct Gaussian conditioning gives

$$
\mathbb E\sqrt{S_2}=\frac{1+e^{-1/24}}2,
$$

a constant. The proposed factor $e^{-A/24}$ is random, so cannot equal that conditional expectation. **The formula requires knowledge of future integrated variance; independence by itself is insufficient.**

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

This part's conditional-expectation representation is its own hypothesis; it does not need the incorrect unrestricted claim in part (b). Fix $T$, and write

$$
I_t(T)=\int_t^Tf_t(u)\,du,\qquad
\beta_t(T)=\int_t^TB_t(u)\,du,\qquad
M_t(T)=U_te^{-I_t(T)}.
$$

The assumed representation makes $M(T)$ a [martingale](../../../martingale.md). The [stochastic Fubini theorem](../../../stochastic-calculus.md#stochastic-fubini-theorem) gives

$$
dI_t(T)=\left(\int_t^TA_t(u)\,du-f_t(t)\right)dt+\beta_t(T)\,dW_t.
$$

Apply the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $e^{-I}$ and use the equation for $U$ from part (a), including the cross-variation. The result is

$$
\frac{dM_t(T)}{M_t(T)}
=\left[f_t(t)-\frac18\sigma_t^2-\int_t^TA_t(u)\,du
+\frac12\beta_t(T)^2-\frac12\sigma_t\beta_t(T)\right]dt
+\left(\frac12\sigma_t-\beta_t(T)\right)dW_t.
$$

Uniqueness of the continuous [semimartingale](../../../stochastic-calculus.md#semimartingale) decomposition makes the drift vanish. Initially this is a $dt\,d\mathbb P$ statement; the assumed continuity in time and maturity extends it to the continuous versions simultaneously. Let $T\downarrow t$ to obtain

$$
\boxed{f_t(t)=\frac18\sigma_t^2=k\sigma_t^2.}
$$

Substitute back and differentiate the maturity integrals using their continuous integrands:

$$
\boxed{A_t(T)=B_t(T)\left(\int_t^TB_t(u)\,du-\frac12\sigma_t\right).}
$$

This is the [forward drift restriction for square-root stock claims](../../../mathematical-finance.md#forward-drift-restriction-for-square-root-stock-claims). The $-\sigma_t/2$ term comes from the product cross-variation and must be retained. For the uninformative zero-[stock](../../../mathematical-finance.md#stock) case, the representation does not identify $f$; as usual a positive initial [stock](../../../mathematical-finance.md#stock) price is understood.

## 5

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Use a [telescoping replication of a stock-price sum](../../../mathematical-finance.md#telescoping-replication-of-a-stock-price-sum). Hold $T-t+1$ shares during interval $(t-1,t]$; at time $t$, sell one share and keep its proceeds in the bond. Start with $T$ shares and no cash, costing $TS_0$.

After the time-$t$ rebalance, the [stock](../../../mathematical-finance.md#stock) holdings are $T-t$ and the cash holdings are $\sum_{u=1}^tS_u$, so wealth is

$$
V_t=\sum_{u=1}^tS_u+(T-t)S_t.
$$

The sale of one share exactly funds the cash increase, making the strategy [self-financing](../../../mathematical-finance.md#self-financing-portfolio). Equivalently,

$$
\boxed{TS_0+\sum_{t=1}^T(T-t+1)(S_t-S_{t-1})
=\sum_{u=1}^TS_u.}
$$

At time $T$ there are no remaining shares, and the cash equals the claim. All [stock](../../../mathematical-finance.md#stock) positions over trading intervals are predictable.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

For every integer $m\in\{0,\ldots,N\}$,

$$
m+2\sum_{K=1}^N(m-K)^+
=m+2\sum_{K=1}^{m-1}(m-K)
=m+m(m-1)=m^2.
$$

Thus the [static replication on a finite terminal support](../../../mathematical-finance.md#static-replication-on-a-finite-terminal-support) consists of **one share and two calls of every listed strike**, held to maturity:

$$
\boxed{S_T^2=S_T+2\sum_{K=1}^N(S_T-K)^+.}
$$

The strike-$N$ call contributes zero at maturity but is harmless in this identity. The portfolio costs $S_0+2\sum_{K=1}^NC_0(K)$. No distributional assumption on the [stock](../../../mathematical-finance.md#stock) is needed beyond its stated terminal support.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

The pathwise identity $(S_t-S_{t-1})^2=S_t^2-S_{t-1}^2-2S_{t-1}(S_t-S_{t-1})$ telescopes to

$$
\sum_{t=1}^T(S_t-S_{t-1})^2
=S_T^2-S_0^2-2\sum_{t=1}^TS_{t-1}(S_t-S_{t-1}).
$$

This is the [discrete realized-variance replication identity](../../../mathematical-finance.md#discrete-realized-variance-replication-identity). Replicate $S_T^2$ using part (b). Add a [self-financing portfolio](../../../mathematical-finance.md#self-financing-portfolio) with initial wealth $-S_0^2$ and [stock](../../../mathematical-finance.md#stock) holdings $-2S_{t-1}$ during $(t-1,t]$.

To give the cash positions explicitly, let

$$
G_{t-1}=-S_0^2-2\sum_{u=1}^{t-1}S_{u-1}(S_u-S_{u-1}).
$$

The added portfolio holds $G_{t-1}+2S_{t-1}^2$ units of the bond over that interval. Its starting value is $G_{t-1}$ and its change is exactly $-2S_{t-1}(S_t-S_{t-1})$. The combined holdings are therefore

$$
\boxed{\text{stock: }1-2S_{t-1},\quad
\text{bond: }G_{t-1}+2S_{t-1}^2,\quad
\text{calls: }2\text{ of each strike}.}
$$

The terminal value equals the squared-increment sum by the telescoping identity. Its initial cost is

$$
\boxed{S_0+2\sum_{K=1}^NC_0(K)-S_0^2
=2\sum_{K=1}^NC_0(K)+S_0(1-S_0).}
$$

The dynamic [stock](../../../mathematical-finance.md#stock) hedge uses only prices known before each interval, while the calls remain static.

## 6

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Normalize $B_0=1$ and put $\widetilde S_t=e^{-rt}S_t$. Its dynamics are $d\widetilde S_t=\widetilde S_t\sigma(t,S_t)\,dW_t$. Bounded volatility makes this [stochastic exponential](../../../stochastic-calculus.md#doleans-dade-exponential) a true [martingale](../../../martingale.md) on each finite horizon, by the [Novikov condition](../../../stochastic-calculus.md#novikov-s-condition). It also gives a finite second moment: stopping the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) for $S^2$ and applying the [Gronwall inequality](../../../probability-and-statistics.md#gronwall-inequality) yields $\mathbb E S_T^2\leq S_0^2e^{(2r+L^2)T}$ when $\sigma\leq L$.

The discounted payoff $\xi=e^{-rT}(S_T-K)^+$ is thus square-integrable. Define the nonnegative [martingale](../../../martingale.md)

$$
M_t=\mathbb E[\xi\mid\mathcal F_t],\qquad M_0=C(T,K).
$$

The [Brownian martingale representation theorem](../../../brownian-motion.md#brownian-martingale-representation-theorem) says that every square-integrable martingale in the Brownian filtration has a representation $M_t=M_0+\int_0^th_u\,dW_u$ with predictable $h$ and $\mathbb E\int_0^Th_u^2du<\infty$. Since $\widetilde S>0$ and $\sigma>0$, choose

$$
\boxed{\pi_t=\frac{h_t}{\widetilde S_t\sigma(t,S_t)},\qquad
\phi_t=M_t-\pi_t\widetilde S_t.}
$$

Then discounted gains satisfy $dM_t=\pi_t\,d\widetilde S_t$. Consequently $X_t=B_tM_t=\phi_tB_t+\pi_tS_t$ is [self-financing](../../../mathematical-finance.md#self-financing-portfolio), nonnegative, and hence an [admissible trading strategy](../../../mathematical-finance.md#admissible-trading-strategy). At maturity $X_T=(S_T-K)^+$, proving [claim replication](../../../mathematical-finance.md#claim-replication) at cost $C(T,K)$.

For minimality, discounted wealth of any admissible [self-financing portfolio](../../../mathematical-finance.md#self-financing-portfolio) is a [local martingale](../../../martingale.md#local-martingale) bounded below, hence a [supermartingale](../../../martingale.md#supermartingale) by localization and the conditional [Fatou lemma](../../../measure-theory.md#fatou-s-lemma). Thus any such replication with initial wealth $x$ obeys

$$
x\geq\mathbb E[e^{-rT}X_T]=C(T,K).
$$

Together with the constructed portfolio, this proves

$$
\boxed{\text{minimal admissible replication cost}=C(T,K).}
$$

This is [Brownian representation replication in a local volatility market](../../../mathematical-finance.md#brownian-representation-replication-in-a-local-volatility-market). The given drift $r$ means that the original probability measure already serves as the [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure).

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Differentiating the [European call option](../../../mathematical-finance.md#european-call-option) price in strike gives, for $T>0$,

$$
C_K(T,K)=-e^{-rT}\int_K^\infty\psi(T,s)\,ds,
\qquad C_{KK}(T,K)=e^{-rT}\psi(T,K).
$$

The strike derivative uses dominated convergence; the second uses the continuous density. Also,

$$
\int_K^\infty s\psi(T,s)\,ds
=e^{rT}\bigl(C(T,K)-KC_K(T,K)\bigr).
$$

Differentiate the supplied time-integral identity and the discount factor. Continuity of the density supplies the diffusion-term derivative. For the tail first moment, continuity in time follows from continuous [stock](../../../mathematical-finance.md#stock) paths, locally uniformly bounded second moments, and the absence of an atom at $K$. Therefore

$$
\begin{aligned}
C_T&=-rC+e^{-rT}\left(r\int_K^\infty s\psi(T,s)\,ds
+\frac12K^2\sigma(T,K)^2\psi(T,K)\right)\\
&=-rKC_K+\frac12K^2\sigma(T,K)^2C_{KK}.
\end{aligned}
$$

Hence the [Dupire equation](../../../mathematical-finance.md#dupire-equation) is

$$
\boxed{C_T(T,K)=\frac12K^2\sigma(T,K)^2C_{KK}(T,K)-rKC_K(T,K).}
$$

Its initial condition is $C(0,K)=(S_0-K)^+$; natural strike boundaries are $C(T,0)=S_0$ and $C(T,K)\to0$ as $K\to\infty$. These are consistent with the discounted [stock](../../../mathematical-finance.md#stock) [martingale](../../../martingale.md) and integrable tails. Where $C_{KK}>0$, the same identity gives [local volatility recovery from call prices](../../../mathematical-finance.md#local-volatility-recovery-from-call-prices):

$$
\boxed{\sigma(T,K)^2=
\frac{2(C_T+rKC_K)}{K^2C_{KK}}.}
$$

The equation evolves in maturity and strike, unlike the backward option-value equation in calendar time and spot.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

The [Brownian martingale representation theorem](../../../brownian-motion.md#brownian-martingale-representation-theorem) argument in part (a) also replicates the bounded put payoff. The discounted [stock](../../../mathematical-finance.md#stock) is a true [martingale](../../../martingale.md), so the elementary terminal payoff identity yields [put-call parity](../../../mathematical-finance.md#put-call-parity)

$$
\boxed{P(T,K)=C(T,K)-S_0+Ke^{-rT}.}
$$

Set $H(T,K)=-S_0+Ke^{-rT}$. Then $H_T=-rKe^{-rT}$, $H_K=e^{-rT}$, and $H_{KK}=0$. Thus

$$
H_T=\frac12K^2\sigma(T,K)^2H_{KK}-rKH_K.
$$

Linearity of the [Dupire equation](../../../mathematical-finance.md#dupire-equation) and $P=C+H$ give

$$
\boxed{P_T(T,K)=\frac12K^2\sigma(T,K)^2P_{KK}(T,K)-rKP_K(T,K).}
$$

The initial payoff is $P(0,K)=(K-S_0)^+$, and $P(T,0)=0$. Therefore calls and puts obey the same maturity-strike differential equation, with their respective initial and boundary data.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
