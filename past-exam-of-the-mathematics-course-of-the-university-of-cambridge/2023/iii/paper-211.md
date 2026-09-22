# Paper 211

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_211.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_211.pdf)

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
  - [e](#2/e)
    - [Solution](#2/e/solution)
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

## 1

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A portfolio $H\in\mathbb R^n$ is an [arbitrage](../../../mathematical-finance.md#arbitrage) when $H\cdot P_0\leq0$, $H\cdot P_1\geq0$ almost surely, and at least one inequality supplies a strict gain: either $H\cdot P_0<0$ or $\mathbb P(H\cdot P_1>0)>0$. It is a [terminal-consumption arbitrage](../../../mathematical-finance.md#terminal-consumption-arbitrage) when $H\cdot P_0=0$, $H\cdot P_1\geq0$ almost surely, and the terminal inequality is strict with positive probability.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

A [numéraire portfolio](../../../mathematical-finance.md#numeraire-portfolio) $\eta$ satisfies $\eta\cdot P_0>0$ and $\eta\cdot P_1>0$ almost surely. If an arbitrage $H$ already has zero initial cost, it is a terminal-consumption arbitrage. Otherwise $H\cdot P_0<0$; set

$$
\widetilde H=H-\frac{H\cdot P_0}{\eta\cdot P_0}\eta.
$$

Then $\widetilde H\cdot P_0=0$, while its terminal payoff is the nonnegative payoff of $H$ plus a strictly positive multiple of $\eta\cdot P_1$. Hence it is strictly positive almost surely and is a terminal-consumption arbitrage.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

If $A=\operatorname{Im}V=\mathbb R^n$, the symmetric covariance matrix $V$ is positive definite. For every nonzero $H$, the scalar $H\cdot P_1$ is normal with variance $H^TVH>0$, so it has positive probability of being negative. It cannot be an arbitrage payoff. The zero portfolio provides no strict gain, proving absence of arbitrage.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For a numéraire portfolio $\eta$, the normal random variable $\eta\cdot P_1$ is strictly positive almost surely. A nondegenerate normal variable has support on all of $\mathbb R$, so it must be degenerate: $\eta^TV\eta=0$, equivalently $V\eta=0$. Thus $\eta\cdot P_1=\eta\cdot\mu>0$ deterministically. The scaled portfolio

$$
B=\frac{\eta}{\eta\cdot\mu}
$$

has terminal value $B\cdot P_1=1$ almost surely and therefore replicates a risk-free bond.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Let $d=\mu-(1+r)P_0$. Since $V$ is symmetric, $A=\operatorname{Im}V=(\ker V)^\perp$. If $d\in A$, every $H\in\ker V$ satisfies

$$
H\cdot\mu=(1+r)H\cdot P_0.
$$

Any $H\notin\ker V$ has a nondegenerate normal terminal value and cannot be nonnegative almost surely. Any $H\in\ker V$ has the displayed deterministic relation, which excludes an arbitrage because $1+r=(\eta\cdot\mu)/(\eta\cdot P_0)>0$.

Conversely, if $d\notin A$, choose $h\in\ker V$ with $h\cdot d>0$. The zero-cost portfolio

$$
H=h-\frac{h\cdot P_0}{\eta\cdot P_0}\eta
$$

has deterministic terminal payoff

$$
H\cdot P_1=h\cdot\mu-(1+r)h\cdot P_0=h\cdot d>0.
$$

It is a terminal-consumption arbitrage. Thus no arbitrage is equivalent to $d\in A$, the [Arbitrage in a one-period Gaussian market](../../../mathematical-finance.md#arbitrage-in-a-one-period-gaussian-market) criterion.

## 2

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A [one-period martingale deflator](../../../mathematical-finance.md#one-period-martingale-deflator) is a pair $Y_0>0$, $Y_1>0$ such that

$$
\mathbb E[Y_1P_1]=Y_0P_0.
$$

If $Y^0,Y^1$ are deflators and $\varepsilon_0,\varepsilon_1>0$, their positive linear combination is strictly positive and

$$
\mathbb E[(\varepsilon_0Y_1^0+\varepsilon_1Y_1^1)P_1]
=(\varepsilon_0Y_0^0+\varepsilon_1Y_0^1)P_0.
$$

It is therefore another martingale deflator.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The one-period [fundamental theorem of asset pricing](../../../mathematical-finance.md#fundamental-theorem-of-asset-pricing), applied as a separating-hyperplane theorem to the cone of attainable payoffs, gives the superhedging duality

$$
\inf\{H\cdot P_0:H\cdot P_1\geq\xi_1\}
=\sup_Y\frac{\mathbb E[\xi_1Y_1]}{Y_0},
$$

where the supremum is over martingale deflators. The assumed strict inequalities make the right side strictly below $\xi_0$. Hence some $H$ satisfies $H\cdot P_0\leq\xi_0$ and $H\cdot P_1\geq\xi_1$ almost surely.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Apply part b with initial capital $\xi_0+\varepsilon$ and let $\varepsilon\downarrow0$. The finite-dimensional attainable space is closed, so a limit portfolio $H$ satisfies $H\cdot P_0\leq\xi_0$ and $H\cdot P_1\geq\xi_1$. Let $\bar Y$ be a deflator for which equality holds. Then

$$
0\leq\mathbb E[\bar Y_1(H\cdot P_1-\xi_1)]
=\bar Y_0(H\cdot P_0-\xi_0)\leq0.
$$

Strict positivity of $\bar Y_1$ forces $H\cdot P_1=\xi_1$ almost surely, and the middle identity then gives $H\cdot P_0=\xi_0$.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

By definition of the concave conjugate, $u(x)\leq\widehat u(y)+xy$ for all $x,y>0$. Put $x=H\cdot P_1$ and $y=Y_1$, take expectations, and use the deflator identity:

$$
\mathbb E[u(H\cdot P_1)]
\leq\mathbb E[\widehat u(Y_1)]
+\mathbb E[Y_1H\cdot P_1]
=\mathbb E[\widehat u(Y_1)]+X_0Y_0.
$$

The maximizing condition in the definition of $\widehat u$ is $u'(x)=y$, so equality holds when $u'(H\cdot P_1)=Y_1$ almost surely. This is [utility duality with martingale deflators](../../../utility-function.md#utility-duality-with-martingale-deflators).

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

For every deflator $Y$ and $\varepsilon\geq0$, $Y^*+\varepsilon Y$ is a deflator. Minimality and right differentiation at zero give

$$
\mathbb E[\widehat u'(Y_1^*)Y_1]+X_0Y_0\geq0.
$$

Taking $Y=Y^*$ and varying the positive scalar multiple $(1+\varepsilon)Y^*$ in both directions around one gives equality.

Set $\xi_1=-\widehat u'(Y_1^*)$ and $\xi_0=X_0$. The preceding inequality says

$$
\mathbb E[\xi_1Y_1]\leq X_0Y_0
$$

for every deflator, with equality at $Y^*$. Part c produces $H^*$ with $H^*\cdot P_0=X_0$ and $H^*\cdot P_1=\xi_1$. The inverse relation between conjugate derivatives gives $u'(\xi_1)=Y_1^*$, so equality holds in part d:

$$
\boxed{\mathbb E[u(H^*\cdot P_1)]
=\mathbb E[\widehat u(Y_1^*)]+X_0Y_0^*.}
$$

## 3

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The bond pays one at maturity. If $\tau=\inf\{t<T:P_t^T\leq0\}$ had positive probability of being finite, buy one bond at $\tau$. A negative price supplies immediate consumption and a positive terminal payoff; a zero price supplies a free positive terminal payoff. Trading only on the stopping event gives an arbitrage. Therefore $P_t^T>0$ almost surely for every $t<T$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For $K_1<K_2$, the lower-strike payoff dominates:

$$
(S_T-K_1)^+\geq(S_T-K_2)^+.
$$

If $C_t^{T,K_1}<C_t^{T,K_2}$, buy the cheaper lower-strike call and sell the higher-strike call. This gives positive initial consumption and a nonnegative terminal payoff, an arbitrage. Hence the [monotonicity of a European call price in strike](../../../mathematical-finance.md#monotonicity-of-a-european-call-price-in-strike) gives $C_t^{T,K_1}\geq C_t^{T,K_2}$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

First, no arbitrage implies the lower bound

$$
C_t^{T+1,K}\geq S_t-KP_t^{T+1}:
$$

otherwise buy the call and $K$ maturity-$(T+1)$ bonds and short one non-dividend-paying stock; the initial receipt is positive and the terminal payoff is nonnegative. At time $T$, the assumption $P_T^{T+1}\leq1$ therefore gives $C_T^{T+1,K}\geq(S_T-K)^+$.

If $C_t^{T,K}>C_t^{T+1,K}$, sell the shorter call and buy the longer one. At time $T$, the longer call's no-arbitrage value covers the shorter call's payoff, with a strictly positive initial receipt. This is impossible, so $T\mapsto C_t^{T,K}$ is nondecreasing.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Order the support as $K_1<\cdots<K_N$ and put

$$
s_i=\frac{g(K_i)-g(K_{i-1})}{K_i-K_{i-1}}.
$$

On the finite support,

$$
g(S_T)=g(K_1)+\sum_{i=2}^Ns_i
\{(S_T-K_{i-1})^+-(S_T-K_i)^+\}.
$$

This follows by telescoping: at $S_T=K_j$, only terms through $j$ survive and reconstruct successive increments of $g$. The [static replication on a finite terminal support](../../../mathematical-finance.md#static-replication-on-a-finite-terminal-support) therefore has no-arbitrage price

$$
\boxed{\pi_t=g(K_1)P_t^T+
\sum_{i=2}^N
\frac{g(K_i)-g(K_{i-1})}{K_i-K_{i-1}}
(C_t^{T,K_{i-1}}-C_t^{T,K_i}).}
$$

## 4

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let $B_t=e^{rt}$ and let $\psi_t$ be the bank-account holding. Then $X_t=\psi_tB_t+\theta_tS_t$. The [self-financing portfolio](../../../mathematical-finance.md#self-financing-portfolio) condition gives

$$
\boxed{dX_t=\psi_t\,dB_t+\theta_t\,dS_t
=r(X_t-\theta_tS_t)\,dt+\theta_t\,dS_t.}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Set

$$
\lambda=\frac{\mu-r}{\sigma},
\qquad
\frac{dQ}{dP}
=\exp\left(-\lambda W_T-\frac12\lambda^2T\right).
$$

By the [Girsanov theorem](../../../stochastic-calculus.md#girsanov-theorem), $W_t^Q=W_t+\lambda t$ is Brownian motion under $Q$. Consequently

$$
dS_t=rS_t\,dt+\sigma S_t\,dW_t^Q,
$$

so discounted stock price is a martingale and $Q$ is the [Risk-neutral measure for the Black-Scholes model](../../../mathematical-finance.md#risk-neutral-measure-for-the-black-scholes-model).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Define the risk-neutral claim value

$$
V(t,s)=e^{-r(T-t)}
\int_{\mathbb R}g\left(
s e^{(r-\sigma^2/2)(T-t)+\sigma\sqrt{T-t}\,z}
\right)\phi(z)\,dz.
$$

Then $V(0,S_0)=x$, $V(T,s)=g(s)$, and the [Black-Scholes equation](../../../mathematical-finance.md#black-scholes-equation) holds. Differentiation under the integral gives the delta

$$
\partial_sV(t,s)=e^{-r\tau}
\mathbb E\left[
g'(se^{(r-\sigma^2/2)\tau+\sigma\sqrt\tau Z})
e^{(r-\sigma^2/2)\tau+\sigma\sqrt\tau Z}
\right],
\qquad \tau=T-t.
$$

A Gaussian shift $Z\mapsto Z+\sigma\sqrt\tau$ rewrites this as

$$
\partial_sV(t,s)=
\int_{\mathbb R}
g'(se^{(r+\sigma^2/2)\tau+\sigma\sqrt\tau z})\phi(z)\,dz,
$$

which is exactly the stated $\theta_t$ at $s=S_t$.

Apply [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $V(t,S_t)$. The PDE gives

$$
dV(t,S_t)=r\{V-\theta_tS_t\}\,dt+\theta_t\,dS_t.
$$

This is the same wealth equation as part a, with the same initial value $x$. Uniqueness therefore gives $X_t^{x,\theta}=V(t,S_t)$ and hence

$$
\boxed{X_T^{x,\theta}=V(T,S_T)=g(S_T).}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
