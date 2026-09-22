# Paper 211

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_211.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_211.pdf)

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

The [natural filtration](../../../stochastic-process.md#natural-filtration) of $S$ is the [natural Brownian filtration](../../../brownian-motion.md#natural-brownian-filtration): since $\sigma>0$, the equation $W_t=(\log(S_t/S_0)-\mu t)/\sigma$ recovers the entire [Brownian motion](../../../brownian-motion.md) history from the [stock](../../../mathematical-finance.md#stock) history. For $s<t$, [independent increments](../../../stochastic-process.md#independent-increments) and the [moment-generating function of a normal distribution](../../../probability-theory.md#moment-generating-function-of-a-normal-distribution) give

$$
\mathbb E[S_t\mid\mathcal F_s^S]
=S_s\mathbb E e^{\mu(t-s)+\sigma(W_t-W_s)}
=S_s e^{(\mu+\sigma^2/2)(t-s)}.
$$

All these [expectations](../../../probability-theory.md#expected-value) are finite. Since $S_s>0$, the [martingale](../../../martingale.md) identity holds for every $s<t$ exactly when the last exponential equals one. **The required logarithmic drift is**

$$
\boxed{\mu=-\frac{\sigma^2}{2}.}
$$

This is the distinction between the [drift](../../../stochastic-calculus.md#drift-coefficient) of $\log S$ and the [drift](../../../stochastic-calculus.md#drift-coefficient) of $S$: here the latter is zero.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Write $h=T-t$. Conditional on $\mathcal F_t^S$, [independent increments](../../../stochastic-process.md#independent-increments) of the [Brownian motion](../../../brownian-motion.md) give

$$
S_T=S_t\exp\{-\sigma^2h/2+\sigma\sqrt h\,Y\},
\qquad Y\sim N(0,1),
$$

where $Y$ has the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution) and is [independent](../../../random-variable.md#independent-random-variables) of $\mathcal F_t^S$. Factoring $S_t$ out of the positive part identifies the [normalized Black-Scholes call function](../../../mathematical-finance.md#normalized-black-scholes-call-function):

$$
\mathbb E[(S_T-K)^+\mid\mathcal F_t^S]
=S_t F(\sigma^2h,K/S_t)=C_t.
$$

The [European call option](../../../mathematical-finance.md#european-call-option) payoff is [integrable](../../../measure-theory.md#integrability), because $0\leq(S_T-K)^+\leq S_T$ and $\mathbb E S_T=S_0$. The [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation) therefore proves that $C$ is a true [martingale](../../../martingale.md). At $t=T$, the boundary value $F(0,m)=(1-m)^+$ gives $C_T=(S_T-K)^+$. **The answer is the conditional payoff martingale**

$$
\boxed{C_t=\mathbb E[(S_T-K)^+\mid\mathcal F_t^S].}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

First work with the [filtration](../../../stochastic-process.md#filtration-probability-theory) $\mathcal G_t=\mathcal F_t^W\vee\sigma(\mathbf1_{\{u\leq\tau\}}:0\leq u\leq t)$, which records the [Brownian motion](../../../brownian-motion.md) and whether [default](../../../mathematical-finance.md#credit-default) has occurred. On $\{s>\tau\}$ all subsequent [defaultable stock](../../../mathematical-finance.md#defaultable-stock) prices vanish. On $\{s\leq\tau\}$, the [memoryless property](../../../continuous-probability-distribution.md#memorylessness-of-the-exponential-distribution) of the [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) gives survival from $s$ to $t$ with [conditional probability](../../../probability-theory.md#conditional-probability) $e^{-\lambda(t-s)}$. The residual survival event is [independent](../../../random-variable.md#independent-random-variables) of the future [independent increments](../../../stochastic-process.md#independent-increments) of the [Brownian motion](../../../brownian-motion.md). Thus, for deterministic $s<t$,

$$
\mathbb E[\widehat S_t\mid\mathcal G_s]
=\mathbf1_{\{s\leq\tau\}}e^{\lambda t}
   e^{-\lambda(t-s)}\mathbb E[S_t\mid\mathcal F_s^W]
=\mathbf1_{\{s\leq\tau\}}e^{\lambda s}S_s
=\widehat S_s.
$$

Also $\mathbb E\widehat S_t=e^{\lambda t}e^{-\lambda t}S_0=S_0$, so this is a true [martingale](../../../martingale.md), with no localization needed. Its [natural filtration](../../../stochastic-process.md#natural-filtration) is contained in $\mathcal G$; applying the [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation) to the displayed identity yields **the requested natural-filtration martingale property**:

$$
\boxed{\mathbb E[\widehat S_t\mid\mathcal F_s^{\widehat S}]=\widehat S_s.}
$$

The printed convention keeps the [stock](../../../mathematical-finance.md#stock) alive at $t=\tau$. It is a left-continuous convention at that one random time. Replacing it by $\mathbf1_{\{t<\tau\}}$ gives the usual [càdlàg](../../../calculus.md#cadlag) [zero-recovery default model](../../../mathematical-finance.md#zero-recovery-default-model); since $\mathbb P(\tau=t)=0$ at each fixed $t$, the fixed-time [martingale](../../../martingale.md) calculations above are unchanged.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

A [martingale](../../../martingale.md) with the specified terminal value must equal its [conditional expectation](../../../measure-theory.md#conditional-expectation). If $\widehat S_t=0$, [default](../../../mathematical-finance.md#credit-default) has already occurred and the terminal [European call option](../../../mathematical-finance.md#european-call-option) payoff is zero. If $\widehat S_t>0$, put $h=T-t$. Conditional on survival to $T$,

$$
\widehat S_T=\widehat S_t e^{\lambda h}
  \exp\{-\sigma^2h/2+\sigma\sqrt h\,Y\},
$$

where $Y$ has the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution); the [conditional probability](../../../probability-theory.md#conditional-probability) of this survival is $e^{-\lambda h}$. The [conditional expectation](../../../measure-theory.md#conditional-expectation) of the payoff in the enlarged [filtration](../../../stochastic-process.md#filtration-probability-theory) used in part (c) is consequently

$$
e^{-\lambda h}\widehat S_t e^{\lambda h}
 F\left(\sigma^2h,\frac{Ke^{-\lambda h}}{\widehat S_t}\right).
$$

This expression is already measurable with respect to the [natural filtration](../../../stochastic-process.md#natural-filtration) of $\widehat S$, so the [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation) gives the same value there. **The survival factor cancels the compensating growth factor**:

$$
\boxed{\widehat C_t=
\begin{cases}
\widehat S_t F\!\left(\sigma^2(T-t),\dfrac{Ke^{-\lambda(T-t)}}{\widehat S_t}\right),&\widehat S_t>0,\\
0,&\widehat S_t=0.
\end{cases}}
$$

The separate zero branch avoids division by zero. At $t=T$ it gives the required payoff, using $F(0,m)=(1-m)^+$; [integrability](../../../measure-theory.md#integrability) follows from $(\widehat S_T-K)^+\leq\widehat S_T$.

## 2

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [short rate](../../../mathematical-finance.md#short-rate) is the limiting [instantaneous forward rate](../../../mathematical-finance.md#instantaneous-forward-rate) at the present maturity. The continuously compounded [zero-coupon bond](../../../mathematical-finance.md#zero-coupon-bond) price is obtained by integrating the [instantaneous forward rate](../../../mathematical-finance.md#instantaneous-forward-rate) curve in its maturity variable. **Both requested relations are**

$$
\boxed{r_t=f(t,t),\qquad
P(t,T)=\exp\!\left(-\int_t^T f(t,u)\,du\right).}
$$

In particular $P(T,T)=1$, and $f(t,T)=-\partial_T\log P(t,T)$. The [short rate](../../../mathematical-finance.md#short-rate) here is instantaneous, rather than the one-period rate used in a discrete-time [bank account](../../../mathematical-finance.md#bank-account).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For fixed maturity $T$, define $b_t^T=\int_t^T\sigma(t,u)\,du$ and $I_t^T=\int_t^T f(t,u)\,du$. The [stochastic Fubini theorem](../../../stochastic-calculus.md#stochastic-fubini-theorem) and the moving lower endpoint give

$$
dI_t^T=
\left[-r_t+\int_t^T\sigma(t,u)\int_t^u\sigma(t,v)\,dv\,du\right]dt
+b_t^T\,dW_t
=\left[-r_t+\frac12(b_t^T)^2\right]dt+b_t^T\,dW_t.
$$

The factor $1/2$ is the integral over one of the two triangles in the square $[t,T]^2$. Applying the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $P(t,T)=e^{-I_t^T}$, its quadratic-variation correction cancels that factor:

$$
\frac{dP(t,T)}{P(t,T)}=r_t\,dt-b_t^T\,dW_t.
$$

Set $D_t=e^{-\int_0^t r_sds}$, the reciprocal of the [continuous-time bank account](../../../mathematical-finance.md#continuous-time-bank-account). The [Itô product rule](../../../stochastic-calculus.md#ito-product-rule) then gives

$$
D_tP(t,T)=P(0,T)\exp\!\left[-\int_0^t b_s^T\,dW_s-\frac12\int_0^t(b_s^T)^2ds\right].
$$

If $|\sigma|\leq M$, then $|b_t^T|\leq MT$ on this finite horizon. The [Novikov condition](../../../stochastic-calculus.md#novikov-s-condition) holds, so this [stochastic exponential](../../../stochastic-calculus.md#doleans-dade-exponential) is a true [martingale](../../../martingale.md), not merely a [local martingale](../../../martingale.md#local-martingale). **The discounted price is therefore**

$$
\boxed{D_tP(t,T)\text{ is a }\mathbb Q\text{-martingale}.}
$$

The authoritative PDF discounts to $t$ in this part. The TeX transcription's upper endpoint $T$ would include future [short rates](../../../mathematical-finance.md#short-rate) and is incorrect here.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Since $P(T,T)=1$, part (b) shows that the [density process](../../../measure-theory.md#density-process) of the [T-forward measure](../../../mathematical-finance.md#t-forward-measure) is

$$
L_t^T=\mathbb E^{\mathbb Q}\!\left[\frac{D_T}{P(0,T)}\,\middle|\,\mathcal F_t\right]
=\frac{D_tP(t,T)}{P(0,T)}
=\mathcal E\!\left(-\int_0^\cdot b_s^T\,dW_s\right)_t.
$$

Its terminal [expectation](../../../probability-theory.md#expected-value) is one and it is strictly positive, so the stated [Radon-Nikodym derivative](../../../measure-theory.md#radon-nikodym-derivative) defines an [equivalent probability measure](../../../measure-theory.md#equivalent-probability-measure). By the [Girsanov theorem](../../../stochastic-calculus.md#girsanov-theorem),

$$
W_t^T=W_t+\int_0^t b_s^T\,ds
$$

is a [Brownian motion](../../../brownian-motion.md) under $\mathbb Q_T$. Substitution of $dW_t=dW_t^T-b_t^Tdt$ cancels the entire [instantaneous forward rate](../../../mathematical-finance.md#instantaneous-forward-rate) drift:

$$
df(t,T)=\sigma(t,T)\,dW_t^T.
$$

Because the integrand is deterministic and bounded, its [Itô integral](../../../stochastic-calculus.md#ito-integral) is square-integrable on $[0,T]$. With the usual fixed initial [instantaneous forward rate](../../../mathematical-finance.md#instantaneous-forward-rate) curve, **the requested true martingale is**

$$
\boxed{f(t,T)=f(0,T)+\int_0^t\sigma(s,T)\,dW_s^T.}
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Use the [Radon-Nikodym derivative](../../../measure-theory.md#radon-nikodym-derivative) at $T_1$ and the [discounted bond price martingale](../../../mathematical-finance.md#discounted-bond-price-martingale) from part (b):

$$
\mathbb E^{\mathbb Q_{T_1}}P(T_1,T_2)
=\frac{\mathbb E^{\mathbb Q}[D_{T_1}P(T_1,T_2)]}{P(0,T_1)}
=\frac{P(0,T_2)}{P(0,T_1)}.
$$

For the [variance](../../../variance.md), put $b_t^i=\int_t^{T_i}\sigma(t,u)du$ and $d_t=b_t^2-b_t^1=\int_{T_1}^{T_2}\sigma(t,u)du$, for $t\leq T_1$. The ratio $R_t=P(t,T_2)/P(t,T_1)$ has, by the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma),

$$
d\log R_t=-\frac12\big((b_t^2)^2-(b_t^1)^2\big)dt-d_t\,dW_t.
$$

Under the [T-forward measure](../../../mathematical-finance.md#t-forward-measure) $\mathbb Q_{T_1}$, $dW_t=dW_t^{T_1}-b_t^1dt$, so its drift becomes $-d_t^2/2$. Since $R_{T_1}=P(T_1,T_2)$,

$$
\log P(T_1,T_2)=\log\frac{P(0,T_2)}{P(0,T_1)}
-\frac12\int_0^{T_1}d_t^2dt-\int_0^{T_1}d_t\,dW_t^{T_1}.
$$

The first two terms are deterministic; the [Itô isometry](../../../stochastic-calculus.md#ito-isometry) supplies the [variance](../../../variance.md) of the last. **The two requested answers are**

$$
\boxed{\mathbb E^{\mathbb Q_{T_1}}P(T_1,T_2)=\frac{P(0,T_2)}{P(0,T_1)},\qquad
\operatorname{Var}^{\mathbb Q_{T_1}}\log P(T_1,T_2)
=\int_0^{T_1}\left(\int_{T_1}^{T_2}\sigma(t,u)\,du\right)^2dt.}
$$

In fact the terminal [zero-coupon bond](../../../mathematical-finance.md#zero-coupon-bond) price has a [log-normal distribution](../../../probability-theory.md#log-normal-distribution) under this [forward measure](../../../mathematical-finance.md#forward-measure), with the deterministic negative half-variance correction ensuring the displayed mean.

## 3

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Choose any strictly positive [pricing kernel](../../../mathematical-finance.md#state-price-density) $Z\in\mathcal Z$. The assumed componentwise [expectations](../../../probability-theory.md#expected-value) and the [linearity of expectation](../../../probability-theory.md#linearity-of-expectation) give

$$
\mathbb E[Z(H\cdot P)]=H\cdot\mathbb E[ZP]=H\cdot p\leq0.
$$

The integrand is nonnegative, so its [expectation](../../../probability-theory.md#expected-value) is also nonnegative and hence zero. A nonnegative [random variable](../../../random-variable.md) with zero [expectation](../../../probability-theory.md#expected-value) vanishes [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Since $Z>0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), this forces $H\cdot P=0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). **Both conclusions follow**:

$$
\boxed{H\cdot p=0,\qquad H\cdot P=0\quad\text{almost surely}.}
$$

The strict positivity of the [pricing kernel](../../../mathematical-finance.md#state-price-density) is essential: a kernel allowed to vanish could miss a positive payoff on its zero set. No normalization $\mathbb EZ=1$ is assumed in this abstract market; that normalization follows only if a unit-priced unit-payoff cash asset is included.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For fixed $\gamma$, [differentiation under the integral sign](../../../analysis.md#differentiation-under-the-integral-sign) is justified by bounded $P$ and $X$. At the unconstrained [minimizer](../../../analysis.md#global-minimizer) $H_\gamma$, the first-order condition is

$$
p\,e^{\gamma(H_\gamma\cdot p-x)}
=\mathbb E\!\left[P e^{\gamma(X-H_\gamma\cdot P)}\right].
$$

Define the strictly positive, bounded [pricing kernel](../../../mathematical-finance.md#state-price-density)

$$
Z_\gamma=\frac{e^{\gamma(X-H_\gamma\cdot P)}}{e^{\gamma(H_\gamma\cdot p-x)}}.
$$

The first-order condition says $\mathbb E[Z_\gamma P]=p$, so $Z_\gamma\in\mathcal Z$. When taking the requested [partial derivative](../../../calculus.md#partial-derivative), hold $H$ fixed and only afterwards set $H=H_\gamma$. Writing $A_\gamma=H_\gamma\cdot p-x$, we obtain

$$
\begin{aligned}
\left.\partial_\gamma F_\gamma(H)\right|_{H=H_\gamma}
&=e^{\gamma A_\gamma}\left[A_\gamma+
\mathbb E\{Z_\gamma(X-H_\gamma\cdot P)\}\right]\\
&=e^{\gamma A_\gamma}\big[\mathbb E(Z_\gamma X)-x\big].
\end{aligned}
$$

The assumed dual bound applies to this particular [pricing kernel](../../../mathematical-finance.md#state-price-density). **Thus**

$$
\boxed{\left.\partial_\gamma F_\gamma(H)\right|_{H=H_\gamma}\leq0.}
$$

No derivative of the map $\gamma\mapsto H_\gamma$ is needed; confusing a [partial derivative](../../../calculus.md#partial-derivative) with a derivative along the minimizing path would add an unnecessary hypothesis.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let $M=\sup_{\gamma>1}F_\gamma(H_\gamma)<\infty$. Choose $\gamma_j\to\infty$. Boundedness of the [minimizers](../../../analysis.md#global-minimizer) and the [Bolzano-Weierstrass theorem](../../../real-analysis.md#bolzano-weierstrass-theorem) yield a [subsequence](../../../real-analysis.md#subsequence), still indexed by $j$, with $H_{\gamma_j}\to H^*\in\mathbb R^n$. Each $H_{\gamma_j}$ is deterministic, hence so is $H^*$. The first exponential term gives

$$
H_{\gamma_j}\cdot p-x\leq\frac{\log M}{\gamma_j},
$$

and passing to the limit gives $H^*\cdot p\leq x$.

To obtain the [superhedging](../../../mathematical-finance.md#superhedging) inequality, suppose instead that $\mathbb P(X>H^*\cdot P)>0$. There is then an $\varepsilon>0$ such that the event $E=\{X-H^*\cdot P\geq\varepsilon\}$ has positive [probability](../../../probability-theory.md#probability). Let $\|P\|\leq B$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). For all sufficiently large $j$,

$$
|(H_{\gamma_j}-H^*)\cdot P|\leq B\|H_{\gamma_j}-H^*\|\leq\varepsilon/2.
$$

Consequently $X-H_{\gamma_j}\cdot P\geq\varepsilon/2$ on $E$, giving

$$
M\geq F_{\gamma_j}(H_{\gamma_j})
\geq\mathbb P(E)e^{\gamma_j\varepsilon/2}\longrightarrow\infty,
$$

a contradiction. **The limiting portfolio meets both constraints**:

$$
\boxed{H^*\cdot p\leq x,\qquad H^*\cdot P\geq X\quad\text{almost surely}.}
$$

Bounded $P$ is used precisely to turn convergence of deterministic holdings into a uniform bound on the payoff error.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Let $h$ be the [stock](../../../mathematical-finance.md#stock) holding and let $c$ be the initial cost, so the cash holding is $b=c-10h$. Terminal [portfolio](../../../mathematical-finance.md#investment-portfolio) wealth at [stock](../../../mathematical-finance.md#stock) price $s$ is $c+h(s-10)$. Dominating the [European call option](../../../mathematical-finance.md#european-call-option) payoff at the three possible prices gives

$$
c-h\geq0,\qquad c\geq0,\qquad c+h\geq1.
$$

Adding the two endpoint inequalities yields $2c\geq1$. Equality is attained by $h=1/2$ and $c=1/2$, which imply $b=-9/2$. The corresponding terminal wealth is $0,1/2,1$ at $s=9,10,11$, respectively, compared with the required payoff $0,0,1$. **The cheapest super-replication strategy is**

$$
\boxed{\text{hold }\frac12\text{ share and }-\frac92\text{ units of cash};\qquad c_{\min}=\frac12.}
$$

The middle-state excess shows why this is [superhedging](../../../mathematical-finance.md#superhedging) rather than exact [claim replication](../../../mathematical-finance.md#claim-replication). The endpoint bound proves global minimality, without relying on the physical state [probabilities](../../../probability-theory.md#probability).

## 4

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

**A complete market can replicate every contingent claim in its specified payoff class**: for every terminal $\mathcal F_T$-measurable payoff $X$, there is an admissible [self-financing portfolio](../../../mathematical-finance.md#self-financing-portfolio) whose terminal wealth equals $X$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Equivalently, in an arbitrage-free finite-state discrete-time model the [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure) is unique. In notation,

$$
\boxed{\forall X\text{ in the claim class},\quad\exists\text{ self-financing }\theta\text{ with }V_T^\theta=X\text{ almost surely}.}
$$

[Market completeness](../../../mathematical-finance.md#complete-market) is a replication property. The following price comparisons also use the usual absence of [arbitrage](../../../mathematical-finance.md#arbitrage), which the source leaves implicit: without it the initial cost of [claim replication](../../../mathematical-finance.md#claim-replication) need not be unique. For example, in a deterministic one-period model with cash worth one at both dates and a [stock](../../../mathematical-finance.md#stock) worth one initially but zero finally, all terminal claims are replicable using cash. Adding any [stock](../../../mathematical-finance.md#stock) holding changes the initial cost without changing the terminal payoff. This is a complete model with [arbitrage](../../../mathematical-finance.md#arbitrage), so it has no well-defined unique replication price.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Under the usual no-[arbitrage](../../../mathematical-finance.md#arbitrage) interpretation from part (a), let $Q^N$ be an [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure) for the strictly positive [numéraire](../../../mathematical-finance.md#numeraire) $N$. Then $M_t=S_t/N_t$ is a [martingale](../../../martingale.md). Define the discounted [European call option](../../../mathematical-finance.md#european-call-option) payoff $Y_t=(S_t-K)^+/N_t=(M_t-K/N_t)^+$. Because $N_{t+1}\geq N_t$ and $K>0$, we have $K/N_{t+1}\leq K/N_t$. The [conditional Jensen inequality](../../../measure-theory.md#conditional-jensen-inequality) therefore gives

$$
\begin{aligned}
\mathbb E^{Q^N}[Y_{t+1}\mid\mathcal F_t]
&\geq\mathbb E^{Q^N}[(M_{t+1}-K/N_t)^+\mid\mathcal F_t]\\
&\geq\big(\mathbb E^{Q^N}[M_{t+1}\mid\mathcal F_t]-K/N_t\big)^+
=Y_t.
\end{aligned}
$$

For the middle step, the strike $K/N_t$ is fixed conditionally on $\mathcal F_t$; alternatively use $\mathbb E[X^+\mid\mathcal F_t]\geq\max\{\mathbb E[X\mid\mathcal F_t],0\}$. Thus $Y$ is a [submartingale](../../../martingale.md#submartingale). [Risk-neutral valuation](../../../mathematical-finance.md#risk-neutral-pricing) in units of $N$ gives $C(T,K)=N_0\mathbb E^{Q^N}Y_T$, with the usual fixed initial prices. **Consequently**

$$
\boxed{C(T+1,K)\geq C(T,K).}
$$

The source's word “increasing” means nondecreasing: a [European call option](../../../mathematical-finance.md#european-call-option) can have zero payoff at successive maturities, so strict increase is not guaranteed. Integrability is understood in the claim class for which the stated replication prices exist.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Let $b$ and $h$ be the numbers of units of the [numéraire](../../../mathematical-finance.md#numeraire) and the [stock](../../../mathematical-finance.md#stock) in a [replicating strategy](../../../mathematical-finance.md#replicating-strategy). The two terminal payoffs of the [European call option](../../../mathematical-finance.md#european-call-option) are $2$ and $0$, so

$$
15b+20h=2,\qquad20b+15h=0.
$$

Solving these simultaneous equations gives $b=-6/35$ and $h=8/35$. **The initial replication cost is**

$$
\boxed{C(1,18)=10b+10h=\frac47.}
$$

As an independent pricing check, let $q$ be the [risk-neutral probability](../../../mathematical-finance.md#risk-neutral-probability) of the state $(15,20)$ under the [numéraire](../../../mathematical-finance.md#numeraire) measure. The discounted [stock](../../../mathematical-finance.md#stock) must have initial value one and terminal mean one:

$$
1=q\frac{20}{15}+(1-q)\frac{15}{20},\qquad q=\frac37.
$$

[Risk-neutral valuation](../../../mathematical-finance.md#risk-neutral-pricing) then gives $10(3/7)(2/15)=4/7$. The physical probabilities $1/2,1/2$ are not the [numéraire](../../../mathematical-finance.md#numeraire)-measure probabilities.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The positive-part function is [convex](../../../real-analysis.md#convex-function), so pathwise [Jensen inequality](../../../real-analysis.md#jensen-s-inequality) gives

$$
\left(\frac1T\sum_{t=1}^T S_t-K\right)^+
\leq\frac1T\sum_{t=1}^T(S_t-K)^+.
$$

To compare the [Asian option](../../../mathematical-finance.md#asian-option) price with [European call option](../../../mathematical-finance.md#european-call-option) prices at different dates, carry each earlier payoff forward using the [numéraire](../../../mathematical-finance.md#numeraire). Purchase $1/T$ of each [replicating strategy](../../../mathematical-finance.md#replicating-strategy) for maturity $t$, and, when its payoff is received, reinvest it in $N$ until $T$. This is a [self-financing portfolio](../../../mathematical-finance.md#self-financing-portfolio), with terminal wealth

$$
\frac1T\sum_{t=1}^T (S_t-K)^+\frac{N_T}{N_t}
\geq\frac1T\sum_{t=1}^T(S_t-K)^+
\geq\left(\frac1T\sum_{t=1}^T S_t-K\right)^+.
$$

The first inequality uses $N_T\geq N_t$ and nonnegative payoffs. Since the [Asian option](../../../mathematical-finance.md#asian-option) is replicable in the [complete market](../../../mathematical-finance.md#complete-market), absence of [arbitrage](../../../mathematical-finance.md#arbitrage) makes its replication cost no larger than this [superhedging](../../../mathematical-finance.md#superhedging) cost. **Therefore**

$$
\boxed{A(T,K)\leq\frac1T\sum_{t=1}^T C(t,K).}
$$

Equivalently, divide the first pathwise bound by $N_T$, use $(S_t-K)^+/N_T\leq(S_t-K)^+/N_t$, and take [expectations](../../../probability-theory.md#expected-value) under the [numéraire](../../../mathematical-finance.md#numeraire) [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure). Merely averaging earlier payoffs without reinvestment would miss the difference in payment dates.

## 5

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Backward induction makes every $U_t$ [adapted](../../../stochastic-process.md#adapted-process) and [integrable](../../../measure-theory.md#integrability): the [conditional expectation](../../../measure-theory.md#conditional-expectation) of an [integrable random variable](../../../probability-theory.md#integrable-random-variable) is [integrable](../../../measure-theory.md#integrability), and $|\max(a,b)|\leq|a|+|b|$. The [Snell envelope](../../../martingale.md#snell-envelope) recursion directly gives $U_t\geq\mathbb E[U_{t+1}\mid\mathcal F_t]$, so $U$ is a [supermartingale](../../../martingale.md#supermartingale).

If $Z$ is a [submartingale](../../../martingale.md#submartingale), iterating its defining inequality gives $\mathbb E[Z_T\mid\mathcal F_t]\geq Z_t$. Starting at $U_T=Z_T$ and applying the [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation) backwards shows

$$
U_t=\max\{Z_t,\mathbb E[Z_T\mid\mathcal F_t]\}
=\mathbb E[Z_T\mid\mathcal F_t].
$$

This last [conditional expectation](../../../measure-theory.md#conditional-expectation) is a true [martingale](../../../martingale.md). **The conclusions are**

$$
\boxed{U\text{ is a supermartingale};\qquad
Z\text{ submartingale}\ \Longrightarrow\ U_t=\mathbb E[Z_T\mid\mathcal F_t]\text{ is a martingale}.}
$$

In the second case waiting until $T$ attains the [optimal stopping](../../../martingale.md#optimal-stopping) value. It is not generally true that $U_t=Z_t$: that further equality holds when $Z$ itself is a [martingale](../../../martingale.md).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

For the intended [random walk](../../../markov-process.md#random-walk) model, take $S_0$ to be deterministic, or [independent](../../../random-variable.md#independent-random-variables) of all the [independent and identically distributed random variables](../../../random-variable.md#independent-and-identically-distributed-random-variables) $Y_j=S_j-S_{j-1}$. If $\nu$ is their common [probability distribution](../../../probability-theory.md#probability-distribution), then $Y_{t+1}$ is [independent](../../../random-variable.md#independent-random-variables) of $\mathcal F_t=\sigma(S_0,Y_1,\ldots,Y_t)$. This supplies the [Markov property](../../../markov-process.md#markov-property) that the backward [dynamic programming](../../../mathematical-optimization.md#dynamic-programming) argument needs. Define the [transition operator](../../../markov-process.md#transition-operator)

$$
(Ph)(s)=\int_{\mathbb R}h(s+y)\,\nu(dy)
$$

and the deterministic [optimal stopping value function](../../../martingale.md#optimal-stopping-value-function) recursively by

$$
V(T,s)=f(s),\qquad V(t,s)=\max\{f(s),(PV(t+1,\cdot))(s)\}.
$$

At any state where the conditional law is evaluated, [independence](../../../random-variable.md#independent-random-variables) gives

$$
\mathbb E[V(t+1,S_{t+1})\mid\mathcal F_t]=(PV(t+1,\cdot))(S_t).
$$

Backward induction, starting with $U_T=f(S_T)$, proves **the intended representation**

$$
\boxed{U_t=V(t,S_t).}
$$

Integrability along the actual [random walk](../../../markov-process.md#random-walk) makes the recursion finite at the states used by that process, up to null sets. If finite real-valued [value functions](../../../mathematical-optimization.md#value-function) on all of $\mathbb R$ are intended, a convenient sufficient convention is statewise integrability: $\mathbb E|f(s+Y_1+\cdots+Y_k)|<\infty$ for every $s$ and $0\leq k\leq T$. Indeed each stopping value is bounded in absolute value by the [expectation](../../../probability-theory.md#expected-value) of the sum of the absolute rewards. This convention makes the displayed recursion finite and measurable everywhere; the source only assumes integrability from the given starting process.

The printed independence of the increments alone does not suffice if $S_0$ can reveal future increments. Here is a bounded finite-state counterexample, also with a [convex](../../../real-analysis.md#convex-function) reward. Let $T=2$, let $\varepsilon_1,\varepsilon_2$ be [independent](../../../random-variable.md#independent-random-variables) fair signs, and set

$$
S_0=\varepsilon_2,\qquad S_1=\varepsilon_1+\varepsilon_2,
\qquad S_2=\varepsilon_1+2\varepsilon_2,\qquad f(s)=s^+.
$$

The two increments are exactly $\varepsilon_1,\varepsilon_2$, hence [independent and identically distributed](../../../random-variable.md#independent-and-identically-distributed-random-variables). But $\mathcal F_1$ already knows both signs, so $U_1=\max\{S_1^+,S_2^+\}$. On the two positive-probability histories with $S_1=0$, its values are respectively $0$ and $1$. Thus no deterministic $V(1,0)$ can work. Adding independence of $S_0$ from the increments repairs this missing [Markov property](../../../markov-process.md#markov-property) hypothesis.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Use the [random walk](../../../markov-process.md#random-walk) interpretation and [optimal stopping value function](../../../martingale.md#optimal-stopping-value-function) recursion specified in part (b). If $h$ is [convex](../../../real-analysis.md#convex-function), translating and integrating its [convexity](../../../real-analysis.md#convex-function) inequality gives, for $0<\theta<1$,

$$
\begin{aligned}
(Ph)(\theta x+(1-\theta)y)
&=\int h\big(\theta(x+z)+(1-\theta)(y+z)\big)\,\nu(dz)\\
&\leq\theta(Ph)(x)+(1-\theta)(Ph)(y).
\end{aligned}
$$

Thus the [transition operator](../../../markov-process.md#transition-operator) preserves [convex functions](../../../real-analysis.md#convex-function). Also the [pointwise maximum of convex functions](../../../real-analysis.md#pointwise-maximum-of-convex-functions) is [convex](../../../real-analysis.md#convex-function): each of two [convex functions](../../../real-analysis.md#convex-function) at an intermediate point is bounded by the same convex combination of their pointwise maximum at the endpoints. Starting with $V(T,\cdot)=f$, backward induction in

$$
V(t,\cdot)=\max\{f,PV(t+1,\cdot)\}
$$

therefore proves **the asserted convexity in the intended model**:

$$
\boxed{V(t,\cdot)\text{ is convex for every }0\leq t\leq T.}
$$

The statewise integrability convention in part (b) gives finite [convex functions](../../../real-analysis.md#convex-function) on all real states. The same inequality holds for the canonical extended value function wherever the expectations are well-defined. Integrability only along one started process need not make that canonical function finite at unused states: for $T=1$, $S_0=0$, $f(s)=e^{s^2}$ and increment density proportional to $e^{-y^2-|y|}$, $\mathbb E f(S_1)<\infty$, but $\mathbb E f(s+Y_1)=\infty$ for $s>1/2$. This concerns the canonical recursion away from visited states, rather than the almost-sure identity for $U$. Arbitrary off-state versions of $V$ need not be [convex](../../../real-analysis.md#convex-function); the recursive version is the one meant here. No zero-mean assumption on the increments was used, and [convexity](../../../real-analysis.md#convex-function) alone does not make $f(S_t)$ a [submartingale](../../../martingale.md#submartingale) for an arbitrary drift.

## 6

↑ **Parent:** [Paper 211](paper-211.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Apply the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $\xi_t=V(t,S_t)$. The backward equation cancels its [drift](../../../stochastic-calculus.md#drift-coefficient), leaving

$$
d\xi_t=\left(V_t+\frac12a(S_t)^2V_{SS}\right)(t,S_t)dt
+a(S_t)V_S(t,S_t)dW_t
=a(S_t)V_S(t,S_t)dW_t.
$$

Bounded $a$ and $V_S$ make this [Itô integral](../../../stochastic-calculus.md#ito-integral) square-integrable on the finite horizon; in addition $V$ itself is bounded. Hence $\xi$ is a true [martingale](../../../martingale.md), not just a [local martingale](../../../martingale.md#local-martingale), and $\xi_T=g(S_T)$. **Taking conditional expectations gives**

$$
\boxed{\xi_t=\mathbb E[g(S_T)\mid\mathcal F_t].}
$$

The [stock](../../../mathematical-finance.md#stock) is understood to be [adapted](../../../stochastic-process.md#adapted-process) to the stated [Brownian filtration](../../../brownian-motion.md#brownian-filtration), with its initial value fixed there. This is the [Feynman-Kac formula](../../../stochastic-calculus.md#feynman-kac-formula) in the zero-potential, zero-drift case.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Differentiate the backward equation for $V$ with respect to the [stock](../../../mathematical-finance.md#stock) state, and put $w=V_S$. The product derivative of $a^2/2$ is $aa'$, giving

$$
w_t+aa'w_S+\frac12a^2w_{SS}=0,\qquad w(T,S)=g'(S).
$$

The assumed smoothness and bounded derivatives put $w$ in the uniqueness class for the equation defining $U$. Therefore $U=V_S$, and $\pi_t=V_S(t,S_t)$ is the [option delta](../../../mathematical-finance.md#option-delta). Substituting in the [Itô integral](../../../stochastic-calculus.md#ito-integral) from part (a) and using $dS_t=a(S_t)dW_t$ gives **the self-financing representation**

$$
\boxed{\xi_t=V(0,S_0)+\int_0^t\pi_s\,dS_s,\qquad\pi_t=V_S(t,S_t).}
$$

The boundedness hypotheses justify both [stochastic integrals](../../../stochastic-calculus.md#stochastic-integral). This derivation does not divide by $a$ and remains valid even at states with zero [diffusion amplitude](../../../stochastic-calculus.md#diffusion-amplitude).

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

The positive [density process](../../../measure-theory.md#density-process) is the [stochastic exponential](../../../stochastic-calculus.md#doleans-dade-exponential)

$$
Z_t=\exp\!\left(\int_0^t a'(S_s)dW_s-\frac12\int_0^t a'(S_s)^2ds\right).
$$

Since $a'$ is bounded, the [Novikov condition](../../../stochastic-calculus.md#novikov-s-condition) holds; $Z$ is a true [martingale](../../../martingale.md) with $\mathbb EZ_T=1$ and $Z_T>0$. Thus it defines the stated [equivalent probability measure](../../../measure-theory.md#equivalent-probability-measure). The positive sign in the exponent means that the [Girsanov theorem](../../../stochastic-calculus.md#girsanov-theorem) gives

$$
\widehat W_t=W_t-\int_0^t a'(S_s)ds,
\qquad dS_t=a(S_t)d\widehat W_t+a(S_t)a'(S_t)dt.
$$

Under this [change of measure](../../../measure-theory.md#change-of-measure), applying the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $\pi_t=U(t,S_t)$ produces precisely the [drift](../../../stochastic-calculus.md#drift-coefficient) in its backward equation, which vanishes:

$$
d\pi_t=a(S_t)U_S(t,S_t)d\widehat W_t.
$$

Bounded $a$ and $U_S$ make $\pi$ a true [martingale](../../../martingale.md) under $\widehat{\mathbb P}$. Its terminal value is $g'(S_T)$. **Consequently**

$$
\boxed{\pi_t=\mathbb E^{\widehat{\mathbb P}}[g'(S_T)\mid\mathcal F_t].}
$$

The sign can also be checked before changing measure: under the original measure $d\pi=-aa'U_Sdt+aU_SdW$, while the [quadratic covariation](../../../stochastic-calculus.md#quadratic-covariation) term in $d(Z\pi)$ is $Zaa'U_Sdt$, exactly cancelling its [drift](../../../stochastic-calculus.md#drift-coefficient).

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

Take the original measure as the [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure) for this zero-interest model, or interpret $S$ as a discounted [stock](../../../mathematical-finance.md#stock) price. **$\xi_t$ is the arbitrage-free value of the European contingent claim with payoff $g(S_T)$**, and **$\pi_t$ is its option delta and replicating stock holding**. Part (b) supplies the [self-financing portfolio](../../../mathematical-finance.md#self-financing-portfolio):

$$
\boxed{\text{stock holding }\pi_t=V_S(t,S_t),\qquad
\text{cash holding }\xi_t-\pi_tS_t.}
$$

With the cash asset identically one, its value is $\xi_t$ and its gains satisfy $d\xi_t=\pi_t\,dS_t$, so it exactly replicates $g(S_T)$. This [delta hedge](../../../mathematical-finance.md#delta-hedge) is admissible since the assumed nonnegative $V$ gives nonnegative wealth. In this continuous-path setting the holdings can be taken [predictable](../../../martingale.md#predictable-process).

The auxiliary [change of measure](../../../measure-theory.md#change-of-measure) in part (c) expresses the [option delta](../../../mathematical-finance.md#option-delta) as an [expectation](../../../probability-theory.md#expected-value) of terminal payoff sensitivity. It changes the [stock](../../../mathematical-finance.md#stock) drift to $aa'$ and is generally not the original [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure) for the zero-interest stock market. Its role is to value sensitivity under the tilted state dynamics, while the actual [replicating strategy](../../../mathematical-finance.md#replicating-strategy) trades under the original dynamics. No general claim of [market completeness](../../../mathematical-finance.md#complete-market) is needed, including when $a$ can vanish.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2016](../../2016.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
