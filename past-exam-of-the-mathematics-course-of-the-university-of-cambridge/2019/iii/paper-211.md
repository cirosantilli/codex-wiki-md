# Paper 211

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_211.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_211.pdf)

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
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [c](#2/c-2)
    - [Solution](#2/c-2/solution)
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
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)

## 1

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

If such $\rho$ existed, then integrability and $H\cdot X\geq0$ would give

$$
0=H\cdot\mathbb E[\rho X]
=\mathbb E[\rho(H\cdot X)].
$$

But $\rho>0$ almost surely and $H\cdot X$ is nonnegative and strictly positive with positive probability. Hence $\rho(H\cdot X)$ is nonnegative and nonzero with positive probability, so its expectation is strictly positive. This contradiction proves that **no such positive state-price density exists**.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $(h_k)$ be a bounded minimizing sequence. A subsequence converges to some $h_*$, and continuity gives $F(h_*)=f$. Since $F$ is smooth and $h_*$ is an unconstrained minimizer,

$$
0=\nabla F(h_*)
=-\mathbb E[Xe^{-h_*\cdot X}\zeta].
$$

Define

$$
\rho=\frac{e^{-h_*\cdot X}\zeta}{F(h_*)}.
$$

Then $\rho>0$, $\mathbb E\rho=1$, and

$$
\mathbb E[\rho X]
=-\frac{\nabla F(h_*)}{F(h_*)}=0.
$$

Thus the normalized exponential tilt is the required [state-price density](../../../mathematical-finance.md#state-price-density).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

We prove the contrapositive. Let

$$
N=\{h\in\mathbb R^n:h\cdot X=0\text{ almost surely}\}.
$$

The function $F$ is constant along $N$, so minimize it on $N^\perp$. Suppose there is no $H$ with $H\cdot X\geq0$ almost surely and strict inequality with positive probability. If a sequence $h_k\in N^\perp$ satisfies $\|h_k\|\to\infty$, pass to a subsequence with

$$
\frac{h_k}{\|h_k\|}\longrightarrow H\in N^\perp,
\qquad\|H\|=1.
$$

Because $H\notin N$ and there is no arbitrage direction, $\mathbb P(H\cdot X<0)>0$. On that event, $e^{-h_k\cdot X}\zeta\to\infty$, and [Fatou lemma](../../../measure-theory.md#fatou-s-lemma) gives $\liminf_kF(h_k)=\infty$. Hence every finite sublevel set of $F$ in $N^\perp$ is bounded. It is also closed, so $F$ attains its infimum there and has a bounded minimizing sequence. This contradicts the assumption. Therefore there is a unit vector $H$ satisfying

$$
\boxed{H\cdot X\geq0\text{ almost surely},
\qquad\mathbb P(H\cdot X>0)>0.}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For $c\in\{0,1\}$ set

$$
\zeta_c=\exp(cY-Y^2-\|X\|^2).
$$

The quadratic negative terms make

$$
F_c(h)=\mathbb E[e^{-h\cdot X}\zeta_c]
$$

everywhere finite and smooth. Existence of the assumed $\rho$ rules out the arbitrage direction in part (c) by part (a). Hence each $F_c$ has a bounded minimizing sequence, and part (b) supplies

$$
\rho_c=\frac{
\exp(-h_c\cdot X+cY-Y^2-\|X\|^2)}{F_c(h_c)}
$$

with $\mathbb E\rho_c=1$ and $\mathbb E(\rho_cX)=0$. Uniqueness forces $\rho_0=\rho_1$. Taking logarithms and cancelling the common quadratic terms gives

$$
Y=(h_1-h_0)\cdot X+\log F_1(h_1)-\log F_0(h_0).
$$

Thus

$$
\boxed{Y=a+b\cdot X}
$$

with $b=h_1-h_0$ and $a=\log F_1(h_1)-\log F_0(h_0)$. Since $Y$ was arbitrary, the one-period market is complete.

## 2

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For $\theta=p+iq$ with $0\leq p\leq1$,

$$
|e^{\theta\log S}|=S^p.
$$

The elementary inequality $x^p\leq1+x$ for $x>0$ gives

$$
\mathbb E|e^{\theta\log S}|
=\mathbb E[S^p]\leq1+\mathbb ES=2.
$$

Therefore the [Mellin transform](../../../analysis.md#mellin-transform) $M(\theta)=\mathbb E[S^\theta]$ is absolutely well-defined throughout the strip and

$$
\boxed{|M(\theta)|\leq2.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Here

$$
S^\theta=(1+t)^\theta e^{-t\theta X}.
$$

The [Laplace transform of an exponential distribution](../../../continuous-probability-distribution.md#laplace-transform-of-an-exponential-distribution) is $\mathbb E[e^{-sX}]=(1+s)^{-1}$ for $\operatorname{Re}s>-1$. Since $\operatorname{Re}(t\theta)\geq0$,

$$
\boxed{M(\theta)=\frac{(1+t)^\theta}{1+t\theta}.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

By the bound in part (a), [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem) applies. Conditional on $S$,

$$
\begin{aligned}
&\sqrt K\,\mathbb E_Y\left[
S^{(1+iY)/2}e^{-iY\log K/2}
\right]\\
&\qquad=\sqrt{KS}\,
\mathbb E_Y\exp\left(\frac{iY}{2}\log\frac SK\right)\\
&\qquad=\sqrt{KS}\,
\exp\left(-\frac12\left|\log\frac SK\right|\right)
=\min(S,K),
\end{aligned}
$$

where the [Characteristic function of the Cauchy distribution](../../../probability-theory.md#characteristic-function-of-the-cauchy-distribution) was used. Since $\mathbb ES=1$,

$$
\mathbb E[(S-K)^+]
=\mathbb E[S-\min(S,K)]
=\boxed{1-\sqrt K\,
\mathbb E\left[M\left(\frac{1+iY}{2}\right)
e^{-iY\log K/2}\right].}
$$

The formula expresses a [European call option](../../../mathematical-finance.md#european-call-option) value through complex moments of $S$. In an affine stochastic-volatility model such as the [Heston model](../../../mathematical-finance.md#heston-model), those moments are available from an explicit transform, so call prices reduce to a one-dimensional Fourier expectation or integral.

<h3 id="2/c-2">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c-2/solution">Solution</h4>

↑ **Parent:** [C](#2/c-2)

Condition on $S$ and use the characteristic function of a [standard normal distribution](../../../probability-theory.md#standard-normal-distribution):

$$
\mathbb E_Z[S^{iZ}\mid S]
=\mathbb E_Z[e^{iZ\log S}]
=e^{-(\log S)^2/2}
=G(S).
$$

The integrand has modulus one, so [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem) is immediate. Taking expectation over $S$ yields

$$
\boxed{\mathbb E[G(S)]=\mathbb E[M(iZ)].}
$$

## 3

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [local martingale deflator](../../../mathematical-finance.md#local-martingale-deflator) makes both $YB$ and $YS$ local martingales. Since the filtration is generated by $W$, the martingale representation theorem and the finite-variation drift forced by $YB$ give

$$
dY_t=-r_tY_tdt+\eta_t dW_t
=-Y_t(r_tdt+\lambda_t dW_t)
$$

for a continuous adapted $\lambda$, where $\eta=-Y\lambda$. Applying the [Itô product rule](../../../stochastic-calculus.md#ito-product-rule) to $YS$ gives drift

$$
Y_tS_t(\mu_t-r_t-\lambda_t\sigma_t)dt.
$$

It vanishes exactly when

$$
\boxed{\lambda_t=\frac{\mu_t-r_t}{\sigma_t}.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Set

$$
M_t=\mathbb E[Y_T\xi_T\mid\mathcal F_t],
\qquad V_t=\frac{M_t}{Y_t}.
$$

The boundedness of $\xi_T$ and positivity of the deflator make $M$ a nonnegative true martingale. By the [Brownian martingale representation theorem](../../../brownian-motion.md#brownian-martingale-representation-theorem), $dM_t=\eta_t dW_t$. A self-financing wealth process with stock holding $\pi_t$ satisfies

$$
dV_t=\{r_tV_t+\pi_tS_t(\mu_t-r_t)\}dt
+\pi_tS_t\sigma_t dW_t.
$$

The product $YV$ then has diffusion coefficient

$$
Y_t(\pi_tS_t\sigma_t-V_t\lambda_t).
$$

Choose

$$
\pi_t=\frac{\eta_t/Y_t+V_t\lambda_t}{S_t\sigma_t},
\qquad
\phi_t=\frac{V_t-\pi_tS_t}{B_t}.
$$

Then $Y_tV_t=M_t$, so $V_T=\xi_T$ and the strategy replicates the claim. It is admissible because $V=M/Y$ is nonnegative.

For any other admissible replicating wealth $\widetilde V$, the nonnegative local martingale $Y\widetilde V$ is a supermartingale. Hence

$$
\widetilde V_0\geq\mathbb E[Y_T\widetilde V_T]
=\mathbb E[Y_T\xi_T].
$$

The constructed strategy has

$$
\boxed{V_0=\phi_0B_0+\pi_0S_0
=\mathbb E[Y_T\xi_T],}
$$

so this is the minimal replication cost.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For constant coefficients, the density process $Y_tB_t/B_0$ is a true exponential martingale and defines the [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure) $Q$. Under $Q$,

$$
dS_t=rS_tdt+\sigma S_t dW_t^Q.
$$

The minimal value process is therefore

$$
V(t,s)=e^{-r(T-t)}
\mathbb E^Q[g(S_T)\mid S_t=s].
$$

The [Markov property](../../../markov-process.md#markov-property) and the lognormal transition law make this a deterministic function of $(t,s)$, and

$$
\boxed{V(t,S_t)=\phi_tB_t+\pi_tS_t.}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Apply [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $V(t,S_t)$. Its Brownian coefficient is

$$
\sigma S_t\frac{\partial V}{\partial s}(t,S_t).
$$

The self-financing portfolio's Brownian coefficient is $\pi_t\sigma S_t$. Since $S_t\sigma>0$, equality of the two value processes forces

$$
\boxed{\pi_t=\widetilde V(t,S_t),
\qquad
\widetilde V(t,s)=\frac{\partial V}{\partial s}(t,s).}
$$

Thus the stock holding is the claim's [option delta](../../../mathematical-finance.md#option-delta).

## 4

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For initial capital zero and a predictable strategy $H$, let $C_t^{0,H}$ denote consumption after the time-$t$ portfolio payoff and before choosing the next holdings. An [investment-consumption arbitrage](../../../mathematical-finance.md#investment-consumption-arbitrage) has

$$
C_t^{0,H}\geq0\quad\text{for every }t,
$$

with strictly positive consumption at some date with positive probability. A [terminal-consumption arbitrage](../../../mathematical-finance.md#terminal-consumption-arbitrage) is a finite-horizon such strategy whose consumption is zero before its terminal date $T$, while $C_T^{0,H}\geq0$ almost surely and $\mathbb P(C_T^{0,H}>0)>0$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

A [numéraire strategy](../../../mathematical-finance.md#numeraire-strategy) $\eta$ has zero consumption and strictly positive wealth

$$
N_t=X_t^{\nu,\eta}=\eta_{t+1}\cdot P_t>0
$$

at every date. Given an investment-consumption arbitrage $H$, retain its holdings and invest each nonnegative consumption $C_s^{0,H}$ in the numéraire. With

$$
A_t=\sum_{s=0}^t\frac{C_s^{0,H}}{N_s},
\qquad
K_t=H_t+A_{t-1}\eta_t,
$$

the self-financing identity for $\eta$ gives zero intermediate consumption for $K$. At a deterministic $T$ after a date at which positive consumption occurs with positive probability, liquidating gives

$$
C_T^{0,K}=C_T^{0,H}
+N_T\sum_{s=0}^{T-1}\frac{C_s^{0,H}}{N_s}\geq0.
$$

It is strictly positive with positive probability. Hence $K$ is a terminal-consumption arbitrage.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Suppose a numéraire strategy $\eta$ existed and write $N_t=\eta_{t+1}\cdot P_t=\eta_t\cdot P_t>0$, using zero consumption. Since $\eta_{t+1}$ is $\mathcal F_t$-measurable and $M_t=(-1)^tZ_tP_t$ is a martingale,

$$
\mathbb E[\eta_{t+1}\cdot M_{t+1}\mid\mathcal F_t]
=\eta_{t+1}\cdot M_t.
$$

Thus

$$
-(-1)^t\mathbb E[Z_{t+1}N_{t+1}\mid\mathcal F_t]
=(-1)^tZ_tN_t,
$$

or

$$
\mathbb E[Z_{t+1}N_{t+1}\mid\mathcal F_t]
=-Z_tN_t.
$$

The left side is nonnegative and the right side nonpositive, so $Z_tN_t=0$ almost surely. Strict positivity of $N_t$ implies $Z_t=0$ almost surely for every $t$, contradicting

$$
\mathbb P(Z_t=0\text{ for all }t)=0.
$$

Therefore **the market has no numéraire strategy**.

## 5

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

At maturity, $P_T^T=1$. If $P_t^T\leq0$ on an event $A\in\mathcal F_t$ of positive probability, buying one bond on $A$ has nonpositive cost and certain payoff $1$ on $A$ at $T$; any negative purchase cost can also be consumed or retained. This is an [arbitrage](../../../mathematical-finance.md#arbitrage). Therefore absence of arbitrage implies

$$
\boxed{P_t^T>0\quad\text{almost surely}.}
$$

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

The one-period [spot interest rate](../../../mathematical-finance.md#spot-interest-rate) is defined by

$$
1+r_t=\frac1{P_t^{t+1}},
$$

and the [bank account](../../../mathematical-finance.md#bank-account) by

$$
B_0=1,
\qquad
B_t=\prod_{s=0}^{t-1}(1+r_s).
$$

A probability measure $Q$ equivalent to the physical measure is a [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure) when every discounted [zero-coupon bond](../../../mathematical-finance.md#zero-coupon-bond) price

$$
\frac{P_t^T}{B_t},\qquad0\leq t\leq T,
$$

is a $Q$-martingale. Equivalently,

$$
P_t^T=B_t\mathbb E^Q[B_T^{-1}\mid\mathcal F_t].
$$

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

If $T\mapsto P_t^T$ is nonincreasing, then

$$
P_t^{t+1}\leq P_t^t=1,
$$

so $1+r_t=(P_t^{t+1})^{-1}\geq1$ and $r_t\geq0$.

Conversely, if every spot rate is nonnegative, then $B_{T+1}=B_T(1+r_T)\geq B_T$. Under a [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure),

$$
P_t^{T+1}
=B_t\mathbb E^Q[B_{T+1}^{-1}\mid\mathcal F_t]
\leq B_t\mathbb E^Q[B_T^{-1}\mid\mathcal F_t]
=P_t^T.
$$

Hence

$$
\boxed{T\mapsto P_t^T\text{ is nonincreasing}
\iff r_t\geq0\text{ for every }t.}
$$

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

Risk-neutral valuation gives

$$
P_t^T
=\mathbb E^Q\left[
\prod_{s=t}^{T-1}(1+r_s)^{-1}
\,\middle|\,\mathcal F_t\right].
$$

For $s\geq t$,

$$
1+r_s=(1+r_t)\prod_{j=t}^{s-1}\zeta_j.
$$

Therefore

$$
\prod_{s=t}^{T-1}(1+r_s)^{-1}
=(1+r_t)^{-(T-t)}
\prod_{j=t}^{T-2}\zeta_j^{-(T-1-j)}.
$$

The future $\zeta_j$ are independent and identically distributed under the stated model, so

$$
\boxed{
P_t^T=(1+r_t)^{-(T-t)}
\prod_{k=1}^{T-t-1}M(-k),}
$$

with an empty product equal to one.

## 6

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Apply the multidimensional [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $\xi_t=F(t,S_t,v_t)$. The stated PDE cancels its drift to $rFdt$, leaving

$$
\begin{aligned}
d\xi_t={}&r\xi_tdt
+\sqrt{v_t}\left(S_tF_S+c\rho F_v\right)dW_t\\
&+c\sqrt{v_t}\sqrt{1-\rho^2}F_v\,dZ_t.
\end{aligned}
$$

Consequently $e^{-rt}S_t$ and $e^{-rt}\xi_t$ are local martingales under the physical measure $P$. Thus $P$ itself is an [equivalent local martingale measure](../../../mathematical-finance.md#equivalent-local-martingale-measure) for the augmented market relative to the bank account. The continuous-time [fundamental theorem of asset pricing](../../../mathematical-finance.md#fundamental-theorem-of-asset-pricing) says that existence of such a measure for locally bounded prices implies no free lunch with vanishing risk, and hence no arbitrage. The terminal condition also gives $\xi_T=\sqrt{S_T}$ as required.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

For

$$
F(t,S,v)=S^{1/2}e^{A(t)v+B(t)},
$$

one has

$$
\frac{F_S}{F}=\frac1{2S},
\quad
\frac{F_{SS}}F=-\frac1{4S^2},
\quad
\frac{F_v}F=A,
\quad
\frac{F_{Sv}}F=\frac{A}{2S},
\quad
\frac{F_{vv}}F=A^2.
$$

Substitution into the PDE and collection of the coefficient of $v$ give the [Riccati differential equation](../../../analysis.md#riccati-equation)

$$
\boxed{
A'(t)-bA(t)-\frac18
+\frac{c\rho}{2}A(t)
+\frac{c^2}{2}A(t)^2=0,
\qquad A(T)=0.}
$$

The terminal condition also requires $B(T)=0$.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

The terms independent of $v$ in the substituted PDE satisfy

$$
B'(t)+\frac r2+aA(t)=r,
$$

so

$$
B'(t)=\frac r2-aA(t),
\qquad B(T)=0.
$$

Integrating backward from $T$ yields

$$
\boxed{
B(t)=-\frac12(T-t)r
+a\int_t^TA(s)ds.}
$$

Thus the requested constant is

$$
\boxed{k=a.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
