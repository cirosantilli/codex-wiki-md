# Paper 211

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_211.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_211.pdf)

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
    - [i](#4/d/i)
      - [Solution](#4/d/i/solution)
    - [ii](#4/d/ii)
      - [Solution](#4/d/ii/solution)
    - [iii](#4/d/iii)
      - [Solution](#4/d/iii/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
  - [e](#5/e)
    - [Solution](#5/e/solution)
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

$X_t^{x,H}$ is the wealth delivered by the holdings chosen before time $t$, after receiving their time-$t$ dividends. The investor then chooses $H_{t+1}$, whose market value is $H_{t+1}\cdot P_t$, and consumes the remainder $C_t^{x,H}$. A [numéraire portfolio](../../../mathematical-finance.md#numeraire-portfolio) is a strategy $\eta$ with zero consumption and strictly positive wealth $N_t=X_t^{\nu,\eta}$ at every time, where $\nu=\eta_1\cdot P_0$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Write $V_t=X_t^{x,H}-C_t^{x,H}=H_{t+1}\cdot P_t>0$. Set $a_0=1$ and recursively

$$
a_t=a_{t-1}\frac{X_t^{x,H}}{V_t},
\qquad
\eta_{t+1}=a_tH_{t+1}.
$$

The factors are positive and adapted, so $\eta$ is previsible. For $t\geq1$,

$$
X_t^{\nu,\eta}=a_{t-1}X_t^{x,H}
=a_tV_t=\eta_{t+1}\cdot P_t,
$$

while the same identity at $t=0$ defines $\nu=\eta_1\cdot P_0$. Thus consumption is zero and wealth is strictly positive, so $\eta$ is a [numéraire portfolio](../../../mathematical-finance.md#numeraire-portfolio).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Put

$$
A_t=\sum_{s=0}^t\frac{C_s^{x,H}}{N_s},
\qquad A_{-1}=0,
$$

and define

$$
K_t=H_t+A_{t-1}\eta_t
\quad(t\geq1).
$$

Because the numéraire strategy is self-financing,

$$
X_t^{x,K}=X_t^{x,H}+A_{t-1}N_t.
$$

Moreover,

$$
\begin{aligned}
C_t^{x,K}
&=X_t^{x,H}+A_{t-1}N_t
-H_{t+1}\cdot P_t-A_t\eta_{t+1}\cdot P_t\\
&=C_t^{x,H}+N_t(A_{t-1}-A_t)=0.
\end{aligned}
$$

This also proves the required wealth formula.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Let

$$
D_t=\sum_{s=1}^t\frac{\delta_s}{N_s},
\qquad D_0=0,
$$

where the sum is componentwise, and set

$$
K_t=H_t+\eta_t(H_t\cdot D_{t-1}).
$$

Then

$$
X_t^{x,K}
=H_t\cdot(\delta_t+P_t)+N_tH_t\cdot D_{t-1}
=H_t\cdot\widetilde P_t
=\widetilde X_t^{x,H}.
$$

Also $K_{t+1}\cdot P_t=H_{t+1}\cdot\widetilde P_t$, so subtracting the new holdings value gives $C_t^{x,K}=\widetilde C_t^{x,H}$.

## 2

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The discrete-time [fundamental theorem of asset pricing](../../../mathematical-finance.md#fundamental-theorem-of-asset-pricing) supplies a strictly positive [martingale deflator](../../../mathematical-finance.md#martingale-deflator) $Y$. Since the maturity-$T$ bond pays one unit at $T$, its deflated price is a martingale:

$$
Y_tP_t^T=\mathbb E(Y_T\mid\mathcal F_t).
$$

Division by $Y_t>0$ gives the formula.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For the bond maturing one period later,

$$
\mathbb E(Y_t\mid\mathcal F_{t-1})
=Y_{t-1}P_{t-1}^t
=\frac{Y_{t-1}}{1+r_t}.
$$

If $r_t\geq0$, this is at most $Y_{t-1}$, which is exactly the [supermartingale](../../../martingale.md#supermartingale) property.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Buy one maturity-$(T-1)$ bond. When it pays one at $T-1$, use all proceeds to buy $1/P_{T-1}^T$ maturity-$T$ bonds. Short $1+f$ maturity-$T$ bonds. The terminal payoff is

$$
\frac1{P_{T-1}^T}-(1+f)=r_T-f.
$$

Its initial replication cost is

$$
\xi_0=P_0^{T-1}-(1+f)P_0^T,
$$

which vanishes for $f=P_0^{T-1}/P_0^T-1$.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

With $P_0^0=1$, the time-zero value of payment $r_t-s$ is

$$
P_0^{t-1}-(1+s)P_0^t.
$$

Summing over $t$ telescopes, so the swap value is

$$
1-P_0^T-s\sum_{t=1}^TP_0^t.
$$

The par swap rate is therefore

$$
\boxed{s=\frac{1-P_0^T}{\sum_{t=1}^TP_0^t}.}
$$

## 3

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A claim $\xi$ is replicated if some holdings $h\in\mathbb R^n$ satisfy $h\cdot P_1=\xi$ almost surely; its replication cost is $h\cdot P_0$. The market is [complete](../../../mathematical-finance.md#complete-market) when every claim in the specified integrability class can be replicated.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Every indicator random variable must lie in the linear span of the $n$ terminal asset prices. If the sigma-algebra had $n+1$ disjoint events of positive probability, their indicators would be linearly independent, yet completeness would place all of them in an at-most-$n$-dimensional space. Hence, modulo null events, the sample space has at most $n$ positive-probability atoms.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For every replicable claim $\xi=h\cdot P_1$,

$$
\mathbb E[(X-Y)\xi]
=h\cdot\mathbb E[(X-Y)P_1]=0.
$$

Completeness makes every bounded claim replicable. Taking increasing bounded truncations of $\operatorname{sgn}(X-Y)$, or using the finite-atom conclusion of part b directly, gives $\mathbb E|X-Y|=0$. Thus $X=Y$ almost surely.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The proposed variable satisfies

$$
\mathbb E(ZP_1)
=\mathbb E(P_1P_1^T)Q^{-1}P_0=P_0.
$$

No arbitrage and the [fundamental theorem of asset pricing](../../../mathematical-finance.md#fundamental-theorem-of-asset-pricing) provide a strictly positive one-period deflator $Y$ with $\mathbb E(YP_1)=P_0$. Part c makes such a deflator unique in a complete market, so $Z=Y>0$ almost surely.

## 4

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Localize when the predictable integrand first exceeds level $n$, just before that increment is taken. The resulting stopped integrand is bounded, so its [martingale transform](../../../martingale.md#martingale-transform) is a martingale by the stated result. The localization times increase to infinity because each finite collection of $H_t$ is finite almost surely. Hence $X$ is a [local martingale](../../../martingale.md#local-martingale).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

On $\{H_T\ne0,X_{T-1}\leq0\}$,

$$
H_T\cdot(M_T-M_{T-1})
=X_T-X_{T-1}\geq-X_{T-1}\geq0.
$$

Dividing by $\|H_T\|$ proves $\xi\geq0$ there; outside that event $\xi=0$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

If $X_{T-1}<0$, then $X_T\geq0$ forces $H_T\ne0$ and a strictly positive increment in the $H_T$ direction. If $X_{T-1}=0$, that directional increment is strictly positive exactly when $X_T>0$. These disjoint cases give

$$
\boxed{\mathbb P(\xi>0)
=\mathbb P(X_T>0,X_{T-1}=0)
+\mathbb P(X_{T-1}<0).}
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/i">i</h4>

↑ **Parent:** [D](#4/d)

<h5 id="4/d/i/solution">Solution</h5>

↑ **Parent:** [I](#4/d/i)

If $X_{T-1}=0$ almost surely, the definition of $T$ gives $\mathbb P(X_T>0)>0$. Part c then implies $\mathbb P(\xi>0)>0$.

<h4 id="4/d/ii">ii</h4>

↑ **Parent:** [D](#4/d)

<h5 id="4/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/d/ii)

If $\mathbb P(X_{T-1}<0)>0$, the second term in the identity of part c is positive, so $\mathbb P(\xi>0)>0$.

<h4 id="4/d/iii">iii</h4>

↑ **Parent:** [D](#4/d)

<h5 id="4/d/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/d/iii)

The assumptions of this case imply $X_{T-1}\geq0$ almost surely and $\mathbb P(X_{T-1}>0)>0$. This would satisfy the defining condition for $T$ one period earlier, contradicting the minimality of $T$. Thus the case is impossible.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

The one-step predictable integrand $\theta$ is bounded by one. If $M$ were a martingale, its transform $\xi=\theta\cdot(M_T-M_{T-1})$ would be an integrable mean-zero random variable. Parts b–d show instead that it is nonnegative almost surely and strictly positive with positive probability, so its expectation is positive. This contradiction proves that $M$ cannot be a martingale.

## 5

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

A predictable strategy $H$ is [self-financing](../../../mathematical-finance.md#self-financing-portfolio) when its wealth $X=H\cdot P$ satisfies

$$
dX_t=H_t\cdot dP_t.
$$

It is admissible when its wealth obeys the stipulated lower bound, here taken to be nonnegative. A strictly positive Itô process $Y$ is a [martingale deflator](../../../mathematical-finance.md#martingale-deflator) when every deflated asset price $YP^i$ is a [local martingale](../../../martingale.md#local-martingale).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

The product rule and self-financing identity show that $XY$ is the stochastic integral of $H$ against the vector of deflated prices $YP$, hence is a [local martingale](../../../martingale.md#local-martingale). It is nonnegative by admissibility and positivity of $Y$. Every nonnegative local martingale is a [supermartingale](../../../martingale.md#supermartingale), so

$$
\boxed{\mathbb E(X_TY_T)\leq X_0Y_0.}
$$

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

The definition of the concave conjugate gives the pointwise [Fenchel–Young inequality](../../../convex-optimization.md#fenchel-young-inequality)

$$
U(x)\leq\widehat U(y)+xy.
$$

Apply it to $(X_T,Y_T)$, take expectations, and use part b:

$$
\mathbb E U(X_T)
\leq\mathbb E\widehat U(Y_T)+\mathbb E(X_TY_T)
\leq\mathbb E\widehat U(Y_T)+X_0Y_0.
$$

If $U'(X_T)=Y_T$, the first inequality is equality; if $XY$ is a true martingale, the second is equality.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

Applying the [Itô product rule](../../../stochastic-calculus.md#ito-product-rule) to $YB$ makes its drift vanish automatically. For $YS$, the drift is

$$
YS(\mu-r-\lambda\sigma)\,dt.
$$

Thus both deflated prices are local martingales when

$$
\lambda=\frac{\mu-r}{\sigma}.
$$

Since self-financing gives $dX=\phi\,dB+\pi\,dS$, another application of the product rule, including $d[X,Y]$, cancels the drift and yields

$$
\boxed{d(X_tY_t)
=Y_t(\pi_tS_t\sigma-X_t\lambda)\,dW_t.}
$$

<h3 id="5/e">e</h3>

↑ **Parent:** [5](#5)

<h4 id="5/e/solution">Solution</h4>

↑ **Parent:** [E](#5/e)

Normalize $Y_0=1/X_0$. Solving its stochastic differential equation gives

$$
\log Y_T
=-\log X_0-\left(r+\frac{\lambda^2}{2}\right)T-\lambda W_T.
$$

For logarithmic utility, $\widehat U(y)=-\log y-1$. Part c and $\mathbb EW_T=0$ therefore give

$$
\mathbb E\log X_T
\leq\log X_0+\left(r+\frac{\lambda^2}{2}\right)T.
$$

If $\pi_t=X_t\lambda/(S_t\sigma)$, part d gives $d(XY)=0$. Hence $X_tY_t=X_0Y_0=1$, so $U'(X_T)=1/X_T=Y_T$ and both inequalities in part c are equalities.

## 6

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

The two-dimensional [Itô formula](../../../stochastic-calculus.md#ito-s-lemma), using $d[W^X,W^Z]_t=\rho\,dt$, gives the drift of $U(t,Z_t,X_t)$ as

$$
U_t+BU_z+\frac12C^2U_{zz}
+zC\rho U_{zx}
+\frac12z^2(U_{xx}-U_x).
$$

The PDE makes this zero, leaving only stochastic-integral terms. Thus $M_t=U(t,Z_t,X_t)$ is a [local martingale](../../../martingale.md#local-martingale).

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Substitute $U=e^{\theta x}V$. After dividing by $e^{\theta x}$, the PDE becomes

$$
V_t+(B+\theta\rho zC)V_z
+\frac12C^2V_{zz}
+\frac12\theta(\theta-1)z^2V=0,
$$

with terminal condition $V(T,z)=1$.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Let $\tau=T-t$ and set

$$
V(t,z)=\exp\{P(\tau)+Q(\tau)z+R(\tau)z^2\}.
$$

Then

$$
\frac{V_z}{V}=Q+2Rz,
\qquad
\frac{V_{zz}}V=2R+(Q+2Rz)^2,
\qquad
\frac{V_t}V=-(\dot P+\dot Qz+\dot Rz^2).
$$

For $B(z)=a-bz$ and $C(z)=c$, matching constant, linear, and quadratic coefficients gives

$$
\dot R
=2c^2R^2+2(\theta\rho c-b)R+\frac12\theta(\theta-1),
$$



$$
\dot Q
=2aR+(\theta\rho c-b)Q+2c^2QR,
$$

and

$$
\dot P=aQ+c^2R+\frac12c^2Q^2.
$$

The terminal condition becomes $P(0)=Q(0)=R(0)=0$. The first equation is a [Riccati equation](../../../analysis.md#riccati-equation); once it is solved, the second is linear in $Q$, followed by direct integration for $P$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
