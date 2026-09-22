# Paper 211

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_211.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_211.pdf)

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
  - [f](#1/f)
    - [Solution](#1/f/solution)
  - [g](#1/g)
    - [Solution](#1/g/solution)
  - [h](#1/h)
    - [Solution](#1/h/solution)
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
  - [e](#3/e)
    - [Solution](#3/e/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)

## 1

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

An [arbitrage](../../../mathematical-finance.md#arbitrage) is a finite-horizon previsible strategy with no positive initial cost, nonnegative cash flows at every date, and a strictly positive cash flow with positive probability at some date, after liquidation. Equivalently, one may require zero initial value and a nonnegative terminal gain that is positive with positive probability, after retaining intermediate cash flows in a cash account.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

A [martingale deflator](../../../mathematical-finance.md#martingale-deflator) is a strictly positive adapted process $Y$ such that every deflated cum-dividend asset gain has zero conditional drift:

$$
\mathbb E\!\left[Y_t(P_t+\delta_t)\mid\mathcal F_{t-1}\right]
=Y_{t-1}P_{t-1}.
$$

Using the definitions of $\pi^H$ and $\xi^H$,

$$
Z_t-Z_{t-1}
=H_t\mathbin\cdot
\left[Y_t(P_t+\delta_t)-Y_{t-1}P_{t-1}\right].
$$

The holdings $H_t$ are $\mathcal F_{t-1}$-measurable, so the right side is a [martingale transform](../../../martingale.md#martingale-transform) of the deflated asset-gain local martingale. Hence $Z$ is a [local martingale](../../../martingale.md#local-martingale).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The [fundamental theorem of asset pricing](../../../mathematical-finance.md#fundamental-theorem-of-asset-pricing) says, in this discrete-time formulation, that the market has no arbitrage if and only if it admits a strictly positive [martingale deflator](../../../mathematical-finance.md#martingale-deflator). Under a chosen positive numeraire this is equivalent to the existence of an equivalent martingale measure for numeraire-discounted gains.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Let $Y$ be a martingale deflator for the original arbitrage-free market. Part b shows that

$$
\pi_t^HY_t+\sum_{s=1}^t\xi_s^HY_s
$$

is a local martingale. Thus $Y$ also deflates the gains of the added asset whose price and dividend are $(\pi^H,\xi^H)$. It already deflates the original $n$ assets, so it is a martingale deflator for the enlarged market. The [fundamental theorem of asset pricing](../../../mathematical-finance.md#fundamental-theorem-of-asset-pricing) implies that the enlarged market has no arbitrage. This expresses the fact that adding a dynamically replicated asset cannot create an arbitrage.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

The strategy $\eta$ is a [self-financing portfolio](../../../mathematical-finance.md#self-financing-portfolio) because $\xi_t^\eta=0$, and its price is known one period in advance. Suppose its price first became nonpositive. On the event, known immediately before that date, that the next price is nonpositive while the current price is positive, an investor can short or buy the self-financing portfolio with the sign that gives no downside, finance the position at the current date, and close it at the known next price. This gives a nonnegative gain and a strictly positive gain whenever the price changes sign or reaches zero from a positive value.

More formally, stopping and scaling $\eta$ on the first such predictable event constructs an arbitrage. Since the market has no arbitrage and $\pi_0^\eta>0$, induction over dates gives

$$
\boxed{\pi_t^\eta>0\qquad(t\geq0).}
$$

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

Normalize the self-financing strategy $\eta$ by defining

$$
L_t=\frac{\eta_t}{\pi_{t-1}^\eta}.
$$

Part e makes this well-defined, and

$$
\pi_t^L=\frac{\eta_{t+1}\cdot P_t}{\pi_t^\eta}=1.
$$

Moreover,

$$
\xi_t^L
=\frac{\eta_t\cdot(P_t+\delta_t)}{\pi_{t-1}^\eta}-1
=\frac{\pi_t^\eta}{\pi_{t-1}^\eta}-1.
$$

Both $K$ and $L$ have constant unit price and predictable dividends. Their difference has zero price and predictable dividend $\xi^K-\xi^L$. If that dividend were nonzero with positive probability, taking its known sign would produce an arbitrage. Therefore $\xi^K=\xi^L$, proving

$$
\boxed{\xi_t^K=\frac{\pi_t^\eta}{\pi_{t-1}^\eta}-1.}
$$

<h3 id="1/g">g</h3>

↑ **Parent:** [1](#1)

<h4 id="1/g/solution">Solution</h4>

↑ **Parent:** [G](#1/g)

Assume condition (1). Given an adapted cash-flow process $X_1,\ldots,X_T$, construct the holdings backwards. Set $H_{T+1}=0$. Once $H_{t+1}$ is known, the random variable

$$
X_t+H_{t+1}\cdot P_t
$$

is $\mathcal F_t$-measurable. Condition (1) supplies an $\mathcal F_{t-1}$-measurable $H_t$ satisfying

$$
H_t\cdot(P_t+\delta_t)
=X_t+H_{t+1}\cdot P_t.
$$

Hence $\xi_t^H=X_t$ for every $t\leq T$, and setting later holdings to zero proves condition (2).

Conversely, let $X_T$ be any $\mathcal F_T$-measurable random variable and apply condition (2) to the adapted process with cash flow $X_T$ at $T$ and zero cash flow earlier. Since $H_{T+1}=0$,

$$
X_T=\xi_T^H=H_T\cdot(P_T+\delta_T),
$$

where $H_T$ is $\mathcal F_{T-1}$-measurable. This is condition (1). The conditions are therefore equivalent and describe [market completeness](../../../mathematical-finance.md#complete-market).

<h3 id="1/h">h</h3>

↑ **Parent:** [1](#1)

<h4 id="1/h/solution">Solution</h4>

↑ **Parent:** [H](#1/h)

Let $Y$ and $\widetilde Y$ be normalized martingale deflators. For any date $T$ and bounded $\mathcal F_T$-measurable $X_T$, condition g supplies a strategy whose only prescribed cash flow is $X_T$ at $T$. Applying the martingale identity from part b gives

$$
\mathbb E[Y_TX_T]=\pi_0^H
=\mathbb E[\widetilde Y_TX_T].
$$

Thus $\mathbb E[(Y_T-\widetilde Y_T)X_T]=0$ for every bounded $\mathcal F_T$-measurable $X_T$. Taking indicators, or the sign of the difference, shows $Y_T=\widetilde Y_T$ almost surely. Since $T$ was arbitrary, the normalized martingale deflator is unique.

## 2

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A [T-forward measure](../../../mathematical-finance.md#t-forward-measure) is a probability measure $Q^T$, equivalent to the physical measure, under which prices expressed in units of the positive maturity-$T$ bond are martingales. Equivalently, every attainable payoff $X_T$ has time-$t$ price

$$
\pi_t=B_t^T\mathbb E_{Q^T}[X_T\mid\mathcal F_t].
$$

The zero-coupon bond is the [numéraire](../../../mathematical-finance.md#numeraire).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The forward contract initiated at $t$ has payoff $S_T-F_t^T$ and zero value. Pricing under the [T-forward measure](../../../mathematical-finance.md#t-forward-measure) gives

$$
0=B_t^T\mathbb E_{Q^T}[S_T-F_t^T\mid\mathcal F_t].
$$

Because $F_t^T$ is $\mathcal F_t$-measurable and $B_t^T>0$,

$$
F_t^T=\mathbb E_{Q^T}[S_T\mid\mathcal F_t].
$$

The [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation) therefore makes $(F_t^T)_{t<T}$ a $Q^T$-martingale.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

If $K_1\leq K_2$, then pointwise

$$
(S_T-K_1)^+\geq(S_T-K_2)^+.
$$

The positive pricing formula under the [T-forward measure](../../../mathematical-finance.md#t-forward-measure) gives

$$
C_t^{T,K}=B_t^T\mathbb E_{Q^T}[(S_T-K)^+\mid\mathcal F_t].
$$

**Therefore $C_t^{T,K_1}\geq C_t^{T,K_2}$, so the call price is non-increasing in strike.**

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Define the piecewise-linear function

$$
h(s)=g(0)+g'(0)s+
\sum_{i=1}^N\bigl(g'(K_i)-g'(K_{i-1})\bigr)(s-K_i)^+.
$$

On $[K_j,K_{j+1})$, its slope is $g'(K_j)$. Since $g$ is [convex](../../../real-analysis.md#convex-function), $g'$ is nondecreasing and hence $h'(s)\leq g'(s)$ wherever the derivatives exist. As $h(0)=g(0)$, integration gives $h(s)\leq g(s)$ for every $s\geq0$.

Positive no-arbitrage pricing, the forward identity $\mathbb E_{Q^T}[S_T\mid\mathcal F_t]=F_t^T$, and the call-price formula now give

$$
\boxed{\pi_t\geq B_t^T\bigl(g(0)+g'(0)F_t^T\bigr)
\bigl(g'(K_i)-g'(K_{i-1})\bigr)C_t^{T,K_i}.}
$$

## 3

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The cash-discounted stock is a positive [continuous local martingale](../../../martingale.md#continuous-local-martingale), because its dynamics contain no drift. Applying [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $\pi_t=U(t,v_t,S_t)$, the displayed partial differential equation cancels its drift exactly, leaving another local martingale. Since $U$ is bounded, $\pi$ is in fact a true martingale.

Thus the physical measure itself is an [equivalent local martingale measure](../../../mathematical-finance.md#equivalent-local-martingale-measure) relative to cash for all three traded assets. The continuous-time [fundamental theorem of asset pricing](../../../mathematical-finance.md#fundamental-theorem-of-asset-pricing) rules out arbitrage, more precisely no free lunch with vanishing risk, in the usual admissible class.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The bounded local martingale $\pi$ is a true martingale. Its terminal condition is $\pi_T=U(T,v_T,S_T)=g(S_T)$, so

$$
\pi_0=\mathbb E[\pi_T]=\mathbb E[g(S_T)].
$$

This is also the [Feynman-Kac formula](../../../stochastic-calculus.md#feynman-kac-formula) for the displayed backward equation.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The explicit [stochastic exponential](../../../stochastic-calculus.md#doleans-dade-exponential) solutions satisfy

$$
S_T=\widetilde S_T
\exp\left\{-\frac12(1-\rho^2)Y_T
+\sqrt{1-\rho^2}\int_0^T\sqrt{v_t}\,dW_t^\perp\right\}.
$$

Conditionally on the path generated by $W$, the last stochastic integral is a centered [Gaussian random variable](../../../probability-theory.md#gaussian-random-variable) with variance $Y_T$, because $W^\perp$ is independent of $W$. The conditional expectation of $g(S_T)$ is therefore

$$
G\bigl(\widetilde S_T,(1-\rho^2)Y_T\bigr).
$$

Taking expectations and using part b proves the result.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Integrating the variance equation gives

$$
\int_0^T\sqrt{v_t}\,dW_t
=\frac1\gamma(v_T-v_0-\alpha T+\beta Y_T).
$$

The [Doléans-Dade exponential](../../../stochastic-calculus.md#doleans-dade-exponential) solution of $d\widetilde S_t=\rho\widetilde S_t\sqrt{v_t}\,dW_t$ is

$$
\widetilde S_T
=S_0\exp\left\{
\rho\int_0^T\sqrt{v_t}\,dW_t
-\frac12\rho^2Y_T\right\}.
$$

Substitution yields

$$
\boxed{\widetilde S_T
=S_0\exp\left\{
\frac\rho\gamma(v_T-v_0-\alpha T+\beta Y_T)
-\frac12\rho^2Y_T\right\}.}
$$

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

The pair $(v_t,Y_t)$ is a [Markov diffusion](../../../stochastic-calculus.md#markov-diffusion) with infinitesimal generator

$$
\mathcal L
=(\alpha-\beta v)\partial_v
+\frac12\gamma^2v\,\partial_{vv}
+v\,\partial_y.
$$

Part d shows that the terminal condition in the equation for $\widetilde U$ is exactly

$$
G\bigl(\widetilde S_T,(1-\rho^2)Y_T\bigr)
$$

when evaluated at $(v_T,Y_T)$. The [Feynman-Kac formula](../../../stochastic-calculus.md#feynman-kac-formula) applied to the displayed backward equation therefore gives

$$
\widetilde U(0,v_0,0)
=\mathbb E\!\left[
G\bigl(\widetilde S_T,(1-\rho^2)Y_T\bigr)\right].
$$

Part c identifies the right side with $\pi_0$.

## 4

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Define

$$
\Delta A_t=U_{t-1}-\mathbb E[U_t\mid\mathcal F_{t-1}],
\qquad
\Delta M_t=U_t-\mathbb E[U_t\mid\mathcal F_{t-1}]
$$

for $t\geq1$, with $A_0=M_0=0$. The supermartingale property makes $\Delta A_t\geq0$, and it is $\mathcal F_{t-1}$-measurable, so $A$ is previsible and nondecreasing. The increments of $M$ have conditional mean zero, so $M$ is a martingale. Finally,

$$
\Delta U_t=\Delta M_t-\Delta A_t,
$$

and summation gives the [Doob decomposition in discrete time](../../../martingale.md#doob-decomposition-theorem)

$$
\boxed{U_t=U_0+M_t-A_t.}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The recursion makes $U$ a [supermartingale](../../../martingale.md#supermartingale) and gives $U_t\geq Z_t$ at every date. The [optional sampling theorem for a supermartingale](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) for the bounded stopping time $\tau$ therefore gives

$$
\boxed{\mathbb E Z_\tau\leq\mathbb E U_\tau\leq U_0.}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Take the first entry into the stopping region:

$$
\tau^*=\inf\{t\leq T:U_t=Z_t\}.
$$

This set is nonempty because $U_T=Z_T$. Before $\tau^*$, the recursion has

$$
U_t=\mathbb E[U_{t+1}\mid\mathcal F_t],
$$

so the stopped process $U_{t\wedge\tau^*}$ is a martingale. Optional sampling and $U_{\tau^*}=Z_{\tau^*}$ give

$$
U_0=\mathbb E U_{\tau^*}=\mathbb E Z_{\tau^*}.
$$

**Thus $\tau^*$ is an [optimal stopping time](../../../martingale.md#optimal-stopping-time).**

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

For every stopping time $\tau$, the martingale case of the [optional sampling theorem for a supermartingale](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) gives $\mathbb EX_\tau=X_0=0$. Hence

$$
\mathbb E(Z_\tau+X_\tau)=\mathbb EZ_\tau.
$$

Use the optimal stopping time from part c and the pathwise inequality

$$
\max_{0\leq t\leq T}(Z_t+X_t)
\geq Z_{\tau^*}+X_{\tau^*}.
$$

Taking expectations gives

$$
\boxed{\mathbb E\max_{0\leq t\leq T}(Z_t+X_t)
\geq\mathbb EZ_{\tau^*}=U_0.}
$$

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Let $U=U_0+M-A$ be its [Doob decomposition in discrete time](../../../martingale.md#doob-decomposition-theorem) and choose the martingale

$$
X_t^*=-M_t.
$$

Since $Z_t\leq U_t$ and $A_t\geq0$,

$$
Z_t+X_t^*
\leq U_t-M_t
=U_0-A_t
\leq U_0.
$$

For the first optimal stopping time $\tau^*$, the [complementarity for the Snell envelope compensator](../../../martingale.md#complementarity-for-the-snell-envelope-compensator) implies $A_{\tau^*}=0$: all compensator increments before $\tau^*$ vanish. Since $Z_{\tau^*}=U_{\tau^*}$,

$$
Z_{\tau^*}+X_{\tau^*}^*=U_0.
$$

Therefore

$$
\max_{0\leq t\leq T}(Z_t+X_t^*)=U_0
$$

pathwise, and taking expectations proves the asserted equality.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
