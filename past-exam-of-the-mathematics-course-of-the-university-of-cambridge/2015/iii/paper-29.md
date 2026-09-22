# Paper 29

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_29.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_29.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
- [6](#6)
  - [i](#6/i)
    - [Solution](#6/i/solution)
  - [ii](#6/ii)
    - [Solution](#6/ii/solution)
  - [iii](#6/iii)
    - [Solution](#6/iii/solution)

## 1

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Write $z^- =\max(-z,0)$. For $a<b$, let $U_N[a,b]$ be the [upcrossing count](../../../martingale.md#upcrossing-count) obtained by successively buying at an observation at or below $a$ and selling at an observation at or above $b$, with the first purchase allowed at time zero. The [Doob upcrossings lemma](../../../martingale.md#doob-upcrossing-inequality) for an integrable discrete-time [martingale](../../../martingale.md) is

$$
\boxed{(b-a)\mathbb E U_N[a,b]\leq\mathbb E(X_N-a)^--\mathbb E(X_0-a)^-\leq\mathbb E(X_N-a)^-.}
$$

The weaker last bound is also the usual [Doob upcrossing inequality](../../../martingale.md#doob-upcrossing-inequality).

To prove it, hold one unit between each purchase and sale, and zero units otherwise. If $H_k$ records the holding over $(k,k+1]$, the decision is $\mathcal F_k$-[measurable](../../../measure-theory.md#measurability), with $H_k\in\{0,1\}$. The resulting [martingale transform](../../../martingale.md#martingale-transform) has gain

$$
G_N=\sum_{k=0}^{N-1}H_k(X_{k+1}-X_k),\qquad \mathbb E G_N=0.
$$

Each completed [upcrossing](../../../martingale.md#upcrossing) earns at least $b-a$. An unfinished holding loses at most $(X_N-a)^-$. If a purchase occurs at zero, its price is $X_0\leq a$, giving the additional discount $(X_0-a)^-$, whether that holding has been sold or remains open. If no purchase occurs at zero, this extra term is zero. Therefore, path by path,

$$
G_N\geq(b-a)U_N[a,b]-(X_N-a)^-+(X_0-a)^-.
$$

Taking [expectations](../../../probability-theory.md#expected-value) proves the bound.

The [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem), stated without proof, says that a discrete-time [martingale](../../../martingale.md) satisfying $\sup_n\mathbb E|X_n|<\infty$ converges [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) to a finite [integrable random variable](../../../probability-theory.md#integrable-random-variable) $X_\infty$. In particular every nonnegative [martingale](../../../martingale.md) converges [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) to a finite limit. Under [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability), the [uniformly integrable martingale convergence theorem](../../../martingale.md#uniformly-integrable-martingale-convergence-theorem) additionally gives [convergence in L1](../../../convergence-of-random-variables.md#convergence-in-l1) and $X_n=\mathbb E[X_\infty\mid\mathcal F_n]$.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

A [martingale](../../../martingale.md) has [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability) when its entire family of time values has uniformly small integrable tails:

$$
\boxed{\lim_{K\to\infty}\sup_{n\geq0}\mathbb E\bigl[|X_n|\mathbf1_{\{|X_n|>K\}}\bigr]=0.}
$$

Here every $X_n$ is an [integrable random variable](../../../probability-theory.md#integrable-random-variable). This implies $\sup_n\mathbb E|X_n|<\infty$, because the contribution from $|X_n|\leq K$ is at most $K$. Mere boundedness of these [expectations](../../../probability-theory.md#expected-value) does not imply [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability).

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Put $Z_n=X_{n\wedge T}$. The [stopped martingale in discrete time](../../../martingale.md#stopped-martingale-in-discrete-time) identity

$$
Z_{n+1}-Z_n=\mathbf1_{\{T>n\}}(X_{n+1}-X_n)
$$

shows that $Z$ is a [martingale](../../../martingale.md): the [indicator function](../../../measure-theory.md#indicator-function) is $\mathcal F_n$-[measurable](../../../measure-theory.md#measurability) and the increment has zero [conditional expectation](../../../measure-theory.md#conditional-expectation). Integrability follows because $Z_n$ is selected from the finitely many integrable values $X_0,\ldots,X_n$.

For the [bounded stopping time](../../../martingale.md#bounded-stopping-time) $\tau=n\wedge T$, the [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) in its conditional form gives

$$
X_\tau=\mathbb E[X_n\mid\mathcal F_\tau].
$$

Here $\mathcal F_\tau$ is the [stopping-time sigma-algebra](../../../martingale.md#stopping-time-sigma-algebra). Indeed, for $A\in\mathcal F_\tau$, partition $A$ into $A\cap\{\tau=k\}\in\mathcal F_k$ and apply the [martingale](../../../martingale.md) identity $\mathbb E[X_n\mid\mathcal F_k]=X_k$ on each piece. This proves the displayed [conditional expectation](../../../measure-theory.md#conditional-expectation) identity directly.

Let $C=\sup_n\mathbb E|X_n|<\infty$ and $A_n=\{|Z_n|>K\}\in\mathcal F_{n\wedge T}$. Conditional absolute-value domination and the [Markov inequality](../../../probability-inequality.md#markov-inequality) give $\mathbb P(A_n)\leq C/K$ and, for any $R>0$,

$$
\begin{aligned}
\mathbb E[|Z_n|\mathbf1_{A_n}]&\leq\mathbb E[|X_n|\mathbf1_{A_n}]\\
&\leq\mathbb E[|X_n|\mathbf1_{\{|X_n|>R\}}]+R\mathbb P(A_n)\\
&\leq\sup_j\mathbb E[|X_j|\mathbf1_{\{|X_j|>R\}}]+\frac{RC}{K}.
\end{aligned}
$$

First choose $R$ using the [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability) of $X$, and then choose $K$. The estimate is uniform in $n$, proving **[uniform integrability of a stopped uniformly integrable martingale](../../../martingale.md#uniform-integrability-of-a-stopped-uniformly-integrable-martingale)**. No finiteness assumption on $T$ is needed.

## 2

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

A [càdlàg martingale](../../../martingale.md#cadlag-martingale) is an [adapted process](../../../stochastic-process.md#adapted-process) $X$ with [càdlàg](../../../calculus.md#cadlag) paths, integrable $X_t$ at each finite time, and

$$
\boxed{\mathbb E[X_t\mid\mathcal F_s]=X_s\quad(0\leq s\leq t).}
$$

The [càdlàg](../../../calculus.md#cadlag) requirement means that the chosen path version is right-continuous and has a finite left limit at every positive time. With a complete [filtration](../../../stochastic-process.md#filtration-probability-theory), it suffices that this holds on one common event of probability one, since the process can be redefined on the exceptional [null set](../../../measure-theory.md#null-set).

The [usual hypotheses for a filtration](../../../stochastic-process.md#usual-conditions-for-a-filtration) are **completeness and right continuity**. Completeness means that $\mathcal F_0$ contains every subset of every null event of the ambient [probability space](../../../probability-theory.md#probability-space); right continuity means

$$
\boxed{\mathcal F_t=\bigcap_{u>t}\mathcal F_u.}
$$

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Fix $t>0$ and partition $[0,t]$ into $m$ equal intervals, with $r_k=kt/m$. Round $t\wedge T$ upward within this interval. The corresponding sampled value is

$$
Y_m=X_0\mathbf1_{\{T=0\}}+\sum_{k=1}^{m-1}X_{r_k}\mathbf1_{\{r_{k-1}<T\leq r_k\}}+X_t\mathbf1_{\{T>r_{m-1}\}}.
$$

Every time in this sum is at most $t$. The [stopping time](../../../martingale.md#stopping-time) property makes each [indicator function](../../../measure-theory.md#indicator-function) $\mathcal F_t$-[measurable](../../../measure-theory.md#measurability), while the [adapted process](../../../stochastic-process.md#adapted-process) property makes each sampled value $\mathcal F_t$-[measurable](../../../measure-theory.md#measurability). Consequently $Y_m$ is $\mathcal F_t$-[measurable](../../../measure-theory.md#measurability).

The rounded times approach $t\wedge T$ from the right, so right continuity gives $Y_m\to X_{t\wedge T}$ for the chosen pathwise [càdlàg](../../../calculus.md#cadlag) version. If path regularity is instead stated only [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), the usual complete [filtration](../../../stochastic-process.md#filtration-probability-theory) handles the exceptional [null set](../../../measure-theory.md#null-set); on an incomplete [filtration](../../../stochastic-process.md#filtration-probability-theory) one should formulate that case as existence of an [adapted](../../../stochastic-process.md#adapted-process) version. At $t=0$, the value is simply $X_0$. Thus **$X^T$ is an [adapted process](../../../stochastic-process.md#adapted-process)**, by [adaptedness of a stopped right-continuous process](../../../stochastic-process.md#adaptedness-of-a-stopped-right-continuous-process). The argument actually needs neither the [martingale](../../../martingale.md) property nor boundedness of $T$.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Recall the [stopping-time sigma-algebra](../../../martingale.md#stopping-time-sigma-algebra):

$$
\mathcal F_S=\{A\in\mathcal F:A\cap\{S\leq t\}\in\mathcal F_t\text{ for every }t\geq0\}.
$$

For the proposed random time,

$$
\{U\leq t\}=\bigl(A\cap\{S\leq t\}\bigr)\cup\bigl(A^c\cap\{T\leq t\}\bigr).
$$

The first set belongs to $\mathcal F_t$. Since $S\leq T$, the second can be written

$$
A^c\cap\{T\leq t\}=\{T\leq t\}\setminus\bigl(A\cap\{S\leq t\}\bigr),
$$

which also belongs to $\mathcal F_t$. Therefore **$U$ is a [stopping time](../../../martingale.md#stopping-time)**, as in [pasting ordered stopping times](../../../martingale.md#pasting-ordered-stopping-times). Moreover $S\leq U\leq T$, so $U$ is a [bounded stopping time](../../../martingale.md#bounded-stopping-time).

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

Fix deterministic $0\leq s<t$ and $A\in\mathcal F_s$. The [pasting ordered stopping times](../../../martingale.md#pasting-ordered-stopping-times) argument shows that $U=s\mathbf1_A+t\mathbf1_{A^c}$ is a [bounded stopping time](../../../martingale.md#bounded-stopping-time). The given stopped-expectation property, applied to $U$ and to the deterministic [stopping time](../../../martingale.md#stopping-time) $t$, yields

$$
0=\mathbb E X_U-\mathbb E X_t=\mathbb E[(X_s-X_t)\mathbf1_A].
$$

This holds for every $A\in\mathcal F_s$. Since $X_s$ is $\mathcal F_s$-[measurable](../../../measure-theory.md#measurability) and both time values are integrable, it is exactly the defining test for [conditional expectation](../../../measure-theory.md#conditional-expectation):

$$
\boxed{\mathbb E[X_t\mid\mathcal F_s]=X_s.}
$$

Hence **$X$ is a [martingale](../../../martingale.md)**. This proof of the [characterization of a martingale by bounded continuous-time stopped expectations](../../../martingale.md#characterization-of-a-martingale-by-bounded-continuous-time-stopped-expectations) uses only deterministic two-time pastings; the [càdlàg](../../../calculus.md#cadlag) assumption and the [usual conditions for a filtration](../../../stochastic-process.md#usual-conditions-for-a-filtration) are stronger than needed for this implication.

## 3

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

First prove [nowhere monotonicity of Brownian motion](../../../brownian-motion.md#nowhere-monotonicity-of-brownian-motion). On a fixed interval $[a,b]$ with rational endpoints and $a<b$, the $2^m$ increments over its equal subdivision are independent centered [normal random variables](../../../probability-theory.md#gaussian-random-variable). If the [Brownian motion](../../../brownian-motion.md) path were nondecreasing, all these increments would be nonnegative, an event with probability $2^{-2^m}$. Letting $m\to\infty$ gives probability zero. The same argument excludes nonincreasing paths. A countable union over rational intervals shows that, [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), no nontrivial interval supports a [monotone function](../../../calculus.md#monotonic-function) restriction of the path, since every such interval contains one with rational endpoints.

Work on this event and on the event of continuous paths. Inside any open interval $I\subset(0,\infty)$, choose two separated smaller intervals, the first to the left of the second. The first contains $r<s$ with $B_r<B_s$, because its restriction is not nonincreasing. The second contains $u<v$ with $B_u>B_v$, because its restriction is not nondecreasing. Thus $r<s<u<v$, all in $I$.

By the [extreme value theorem](../../../real-analysis.md#extreme-value-theorem), the path attains its maximum on $[r,v]$. This value exceeds $B_r$, since it is at least $B_s$, and exceeds $B_v$, since it is at least $B_u$. A maximizing time therefore lies in $(r,v)$ and is a [local maximum of Brownian motion](../../../brownian-motion.md#local-maximum-of-brownian-motion). Every open interval in the half-line contains a positive-time interval of this kind. Consequently **the set of [local maxima of Brownian motion](../../../brownian-motion.md#local-maximum-of-brownian-motion) is dense in $[0,\infty)$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence)**.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

For fixed rational $0\leq t_1<t_2<t_3<t_4$, write

$$
\max_{t_3\leq t\leq t_4}B_t-\max_{t_1\leq t\leq t_2}B_t
=\underbrace{B_{t_3}-B_{t_2}}_{Z}+\underbrace{\max_{t_3\leq t\leq t_4}(B_t-B_{t_3})}_{V}+\underbrace{B_{t_2}-\max_{t_1\leq t\leq t_2}B_t}_{W}.
$$

By [independent increments](../../../stochastic-process.md#independent-increments), $Z$ is independent of $(V,W)$ and has [normal distribution](../../../probability-theory.md#normal-distribution) $N(0,t_3-t_2)$. Conditional on $(V,W)$, the displayed difference has a continuous [probability density function](../../../continuous-probability-distribution.md#probability-density-function); in particular it equals zero with probability zero. Taking the countable intersection over all such rational quadruples proves that, on one event of probability one, the maxima over any two separated rational closed intervals are distinct.

Suppose a [local maximum](../../../analysis.md#local-maximum) at $t$ were not a [strict local maximum](../../../analysis.md#strict-local-maximum). There is a neighbourhood in which every value is at most $B_t$, and, arbitrarily close to $t$, some other time $u$ strictly inside that neighbourhood has $B_u=B_t$. Choose separated rational closed intervals containing $t$ and $u$, both lying inside that neighbourhood. When one time is zero, use a first interval with left endpoint zero. Both interval maxima equal $B_t$, contrary to the preceding event.

Therefore **every [local maximum of Brownian motion](../../../brownian-motion.md#local-maximum-of-brownian-motion) is a [strict local maximum](../../../analysis.md#strict-local-maximum) [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence)**, simultaneously over all times. This countable-interval argument avoids an invalid intersection of probability-one events over uncountably many candidate times.

## 4

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

A standard form of the [Kakutani solution of the Dirichlet problem](../../../analysis.md#kakutani-solution-of-the-dirichlet-problem) uses a bounded [domain](../../../topology.md#domain-mathematical-analysis) $D\subset\mathbb R^d$, continuous [Dirichlet boundary data](../../../differential-equation.md#dirichlet-boundary-data) $f\in C(\partial D)$, and regularity of every boundary point for the [Dirichlet problem](../../../analysis.md#dirichlet-problem). The boundedness of $D$ makes $\partial D$ a [compact set](../../../topology.md#compact-space), so $f$ is a [bounded function](../../../function.md#bounded-function) and a [uniformly continuous function](../../../calculus.md#uniformly-continuous-function). A bounded domain with $C^2$ boundary is a sufficient geometric case; one must not omit boundary regularity for an arbitrary bounded domain.

One standard analytic characterization of a [regular boundary point](../../../analysis.md#regular-boundary-point) on a bounded domain is the existence of a positive harmonic barrier: for each $\xi\in\partial D$ there is a [harmonic function](../../../partial-differential-equation.md#harmonic-function) $h_\xi\in C(\overline D)$ with $h_\xi(\xi)=0$ and $h_\xi(x)>0$ for $x\in\overline D\setminus\{\xi\}$. This is the harmonic form of a [barrier for the Dirichlet problem](../../../analysis.md#barrier-for-the-dirichlet-problem); the barrier characterization of regularity is a standard fact of [potential theory](../../../analysis.md#potential-theory).

Let $B$ be $d$-dimensional [Brownian motion](../../../brownian-motion.md) started at $x\in D$ and let $\tau_D=\inf\{t\geq0:B_t\notin D\}$ be its [Brownian exit time](../../../brownian-motion.md#brownian-exit-time). Then the unique solution in $C(\overline D)\cap C^2(D)$ is

$$
\boxed{u(x)=\mathbb E_x[f(B_{\tau_D})]\quad(x\in D),\qquad u(\xi)=f(\xi)\quad(\xi\in\partial D).}
$$

Equivalently, $u(x)=\int_{\partial D}f(\xi)\,\omega_D(x,d\xi)$, where $\omega_D$ is [harmonic measure](../../../brownian-motion.md#harmonic-measure), the exit [probability distribution](../../../probability-theory.md#probability-distribution) of [Brownian motion](../../../brownian-motion.md). The [harmonic function](../../../partial-differential-equation.md#harmonic-function) equation is $\Delta u=0$, with the [Laplace operator](../../../partial-differential-equation.md#laplace-operator) convention $\Delta=\sum_j\partial_j^2$.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

The construction is well defined. Since $D$ is contained in a ball, its [Brownian exit time](../../../brownian-motion.md#brownian-exit-time) is finite [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence): at successive integer times there is a fixed positive probability that the next independent unit-time [Brownian motion](../../../brownian-motion.md) increment has length greater than the ball's diameter, forcing an exit. The survival probability is therefore bounded by a geometric sequence. Path continuity gives $B_{\tau_D}\in\partial D$. Thus the bounded [Dirichlet boundary data](../../../differential-equation.md#dirichlet-boundary-data) give a bounded Borel function $u$ on $D$.

For interior harmonicity, fix a ball with closure in $D$, centred at $x$, and let $\sigma$ be its [Brownian exit time](../../../brownian-motion.md#brownian-exit-time). The [Strong Markov property](../../../markov-process.md#strong-markov-property), followed by the [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation), gives

$$
u(x)=\mathbb E_x[u(B_\sigma)].
$$

The [orthogonal invariance of Brownian motion](../../../brownian-motion.md#orthogonal-invariance-of-brownian-motion) makes $B_\sigma$ uniform on the boundary sphere. Hence $u$ has the spherical [mean value property for harmonic functions](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions) for every such ball. A locally bounded Borel function with this property is smooth and harmonic: integrating the spherical averages against any smooth radial [mollifier](../../../distribution-theory.md#mollifier) gives $u=u*\rho$ locally, which first proves smoothness; the [mean value property for harmonic functions](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions) then implies $\Delta u=0$.

For the boundary limit at $\xi$, choose the harmonic [barrier for the Dirichlet problem](../../../analysis.md#barrier-for-the-dirichlet-problem) $h_\xi$ from (i). The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma), localized inside $D$, makes $h_\xi(B_{t\wedge\tau_D})$ a bounded [martingale](../../../martingale.md). Compact localization and the [bounded convergence theorem](../../../measure-theory.md#bounded-convergence-theorem), first to the exit and then as $t\to\infty$, yield

$$
\mathbb E_x h_\xi(B_{\tau_D})=h_\xi(x).
$$

For $\varepsilon>0$, if $\partial D\setminus B(\xi,\varepsilon)$ is nonempty, [compactness](../../../topology.md#compact-space) and barrier positivity give

$$
c_\varepsilon=\min_{\eta\in\partial D,\ |\eta-\xi|\geq\varepsilon}h_\xi(\eta)>0,\qquad
\mathbb P_x(|B_{\tau_D}-\xi|\geq\varepsilon)\leq\frac{h_\xi(x)}{c_\varepsilon}\longrightarrow0\quad(x\to\xi).
$$

If that boundary subset is empty, the probability is already zero. Therefore

$$
|u(x)-f(\xi)|\leq\sup_{\eta\in\partial D,\ |\eta-\xi|<\varepsilon}|f(\eta)-f(\xi)|+2\|f\|_\infty\mathbb P_x(|B_{\tau_D}-\xi|\geq\varepsilon).
$$

First let $x\to\xi$ and then $\varepsilon\downarrow0$. The [continuity](../../../calculus.md#continuous-function) of the [Dirichlet boundary data](../../../differential-equation.md#dirichlet-boundary-data) proves $u(x)\to f(\xi)$.

Finally, the difference of two continuous solutions is a [harmonic function](../../../partial-differential-equation.md#harmonic-function) vanishing on the boundary. The [maximum principle for harmonic functions](../../../partial-differential-equation.md#maximum-principle-for-harmonic-functions) on the bounded domain gives that it is zero. Thus **the [Kakutani solution of the Dirichlet problem](../../../analysis.md#kakutani-solution-of-the-dirichlet-problem) exists, attains every prescribed boundary value, and is unique**.

## 5

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

For $A>0$, the first time $T_A=\inf\{n\geq0:X_n<-A\}$ is a [stopping time](../../../martingale.md#stopping-time). On $\{T_A\geq1\}$, the [bounded increments](../../../stochastic-process.md#bounded-increments) assumption controls the overshoot:

$$
X_{T_A}\geq-A-M.
$$

Before that time, $X_n\geq-A$. Allowing the possibility $T_A=0$, the process

$$
Y_n=X_{n\wedge T_A}+A+M+X_0^-
$$

is a nonnegative [martingale](../../../martingale.md). Indeed, the [stopped martingale in discrete time](../../../martingale.md#stopped-martingale-in-discrete-time) is a [martingale](../../../martingale.md), and the integrable $\mathcal F_0$-[measurable](../../../measure-theory.md#measurability) variable $X_0^-$ is a constant-in-time [martingale](../../../martingale.md). If $T_A=0$, nonnegativity follows from $X_0+X_0^-=X_0^+$. Its [expectations](../../../probability-theory.md#expected-value) are constant and finite, so the [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem) makes $Y_n$ converge to a finite value [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence).

On $\{T_A=\infty\}$ this proves finite convergence of $X_n$. Taking the countable union over positive integer $A$, we conclude that $X_n$ converges finitely on the event $\{\inf_nX_n> -\infty\}$. Apply the same reasoning to the [martingale](../../../martingale.md) $-X$ to obtain finite convergence on $\{\sup_nX_n<\infty\}$.

Outside the event of finite convergence, both the infimum and the supremum of the sequence must therefore be infinite in the respective directions. Removing any finite initial segment cannot change this, because each of its values is finite. Hence

$$
\boxed{\mathbb P\bigl(\{X_n\text{ converges finitely}\}\cup\{\liminf_nX_n=-\infty,\ \limsup_nX_n=+\infty\}\bigr)=1.}
$$

This is the [bounded-increment martingale convergence-or-oscillation dichotomy](../../../stochastic-process.md#bounded-increment-martingale-convergence-or-oscillation-dichotomy). The $X_0^-$ term ensures the proof also covers an unbounded integrable initial value.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Let independent [Bernoulli random variables](../../../discrete-probability-distribution.md#bernoulli-distribution) $Y_n$ have success probabilities $2^{-n}$, for $n\geq1$, and use their [natural filtration](../../../stochastic-process.md#natural-filtration). Define

$$
\boxed{X_0=0,\qquad X_n=\sum_{k=1}^n(1-2^kY_k).}
$$

Each increment is integrable, finite, and independent of the previous [filtration](../../../stochastic-process.md#filtration-probability-theory), with [expectation](../../../probability-theory.md#expected-value)

$$
\mathbb E(1-2^nY_n)=1-2^n2^{-n}=0.
$$

Thus $X$ is a [martingale](../../../martingale.md). The increments have no common finite bound, since a success produces a jump of size $2^n-1$.

Since $\sum_n\mathbb P(Y_n=1)<\infty$, the [First Borel-Cantelli lemma](../../../probability-theory.md#borel-cantelli-first-lemma) says that only finitely many successes occur [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Consequently

$$
X_n=n-\sum_{k\geq1}2^kY_k
$$

for all sufficiently large $n$, with the random sum finite [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Therefore **$X_n\to+\infty$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence)**, so neither finite convergence nor two-sided oscillation occurs. This [rare-jump martingale divergence](../../../martingale.md#rare-jump-martingale-divergence) example gives probability zero, rather than one, for the union in (i).

## 6

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="6/i">i</h3>

↑ **Parent:** [6](#6)

<h4 id="6/i/solution">Solution</h4>

↑ **Parent:** [I](#6/i)

Use the intrinsic definition of a [Lévy process](../../../stochastic-process.md#levy-process): $X_0=0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), its increments over disjoint time intervals are independent, their [probability distributions](../../../probability-theory.md#probability-distribution) depend only on interval length, and $X$ has [stochastic continuity](../../../stochastic-process.md#stochastic-continuity). In symbols,

$$
X_{s+t}-X_s\overset d=X_t,\qquad X_{t+h}\longrightarrow X_t\text{ in probability as }h\to0
$$

with times restricted to the half-line. Such a [stochastic process](../../../stochastic-process.md) has a [càdlàg modification](../../../stochastic-process.md#cadlag-modification), and is usually represented by that version. Requiring [càdlàg](../../../calculus.md#cadlag) paths in the definition is a common equivalent convention at the level of modifications; it is important to distinguish this from a claim about the paths of an arbitrary supplied version.

For the [characteristic function](../../../probability-theory.md#characteristic-function), write

$$
\boxed{\mathbb E e^{i\theta X_t}=e^{t\psi(\theta)}=e^{-t\Psi(\theta)},\qquad\Psi=-\psi.}
$$

Here $\psi(0)=0$ and $\psi$ is the positive-time-sign [characteristic exponent of a Lévy process](../../../stochastic-process.md#characteristic-exponent-of-a-levy-process). The [independent increments](../../../stochastic-process.md#independent-increments) and [stationary increments](../../../stochastic-process.md#stationary-increments) give $\phi_{s+t}(\theta)=\phi_s(\theta)\phi_t(\theta)$; [stochastic continuity](../../../stochastic-process.md#stochastic-continuity) gives continuity in time and $\phi_0=1$. This continuous multiplicative [semigroup](../../../algebra.md#semigroup) has the stated exponential form. Its exponent has the [Lévy–Khintchine formula](../../../stochastic-process.md#levy-khintchine-formula)

$$
\psi(\theta)=ib\theta-\frac{\sigma^2\theta^2}{2}+\int_{\mathbb R\setminus\{0\}}\left(e^{i\theta y}-1-i\theta y\mathbf1_{\{|y|\leq1\}}\right)\nu(dy),
$$

where $b\in\mathbb R$, $\sigma^2\geq0$, and the [Lévy measure](../../../stochastic-process.md#levy-measure) $\nu$ satisfies $\int(1\wedge y^2)\nu(dy)<\infty$. The truncation convention fixes the [drift coefficient](../../../stochastic-calculus.md#drift-coefficient) $b$; the displayed sign convention agrees with $\Psi=-\psi$.

<h3 id="6/ii">ii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6/ii)

Construct a rate-$\lambda$ [Poisson process](../../../probability-theory.md#poisson-process), for $\lambda>0$, from independent waiting times $E_j$ with [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) $\operatorname{Exp}(\lambda)$. Put $S_k=E_1+\cdots+E_k$, $S_0=0$, and $N_t=\max\{k:S_k\leq t\}$. The [strong law of large numbers](../../../convergence-of-random-variables.md#strong-law-of-large-numbers) gives $S_k/k\to1/\lambda$, so there are only finitely many arrivals on each finite interval. Consequently the counting paths are [càdlàg](../../../calculus.md#cadlag), and $N_0=0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence).

At any deterministic time $s$, the [memorylessness of the exponential distribution](../../../continuous-probability-distribution.md#memorylessness-of-the-exponential-distribution) says that the residual waiting time has again [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) $\operatorname{Exp}(\lambda)$ and is independent of the observed history. Subsequent waiting times are fresh independent copies. Thus the [Poisson process](../../../probability-theory.md#poisson-process) restarts independently at $s$, proving [independent increments](../../../stochastic-process.md#independent-increments) and [stationary increments](../../../stochastic-process.md#stationary-increments). Integrating the joint waiting-time densities over $0<s_1<\cdots<s_k\leq t<s_{k+1}$ gives

$$
\mathbb P(N_t=k)=e^{-\lambda t}\frac{(\lambda t)^k}{k!},\qquad k\geq0,
$$

so its time values have the expected [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution).

For $h\downarrow0$,

$$
\mathbb P(N_h\ne0)=1-e^{-\lambda h}\longrightarrow0.
$$

Together with [stationary increments](../../../stochastic-process.md#stationary-increments), this gives [stochastic continuity](../../../stochastic-process.md#stochastic-continuity) at every time, from either side where applicable. All the [Lévy process](../../../stochastic-process.md#levy-process) requirements hold, and

$$
\boxed{\mathbb E e^{i\theta N_t}=\exp\{\lambda t(e^{i\theta}-1)\},\qquad\psi(\theta)=\lambda(e^{i\theta}-1).}
$$

For $\lambda=0$, the identically zero process gives the degenerate case.

<h3 id="6/iii">iii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#6/iii)

First, [convergence in probability](../../../convergence-of-random-variables.md#convergence-in-probability) at $t=0$ gives $X_0=0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), since every $X_0^n=0$. For any finite set of times, the corresponding vectors converge in probability: the [union bound](../../../probability-inequality.md#boole-s-inequality) controls the probability that any coordinate differs by more than a fixed tolerance. The same holds for their increment vectors, hence also for their [convergence in distribution](../../../convergence-of-random-variables.md#convergence-in-distribution).

For $0=t_0<t_1<\cdots<t_m$, set $D_j^n=X^n_{t_j}-X^n_{t_{j-1}}$ and $D_j=X_{t_j}-X_{t_{j-1}}$. The [characteristic function of a random vector](../../../probability-theory.md#characteristic-function-of-a-random-vector) factors for the independent increments of each $X^n$:

$$
\mathbb E\exp\left(i\sum_{j=1}^m\theta_jD_j^n\right)=\prod_{j=1}^m\mathbb E e^{i\theta_jD_j^n}.
$$

Pass to the limit using [convergence in distribution](../../../convergence-of-random-variables.md#convergence-in-distribution) and bounded [continuous functions](../../../calculus.md#continuous-function). The resulting factorization of the [characteristic function of a random vector](../../../probability-theory.md#characteristic-function-of-a-random-vector), with the [uniqueness theorem for characteristic functions](../../../probability-theory.md#uniqueness-theorem-for-characteristic-functions), proves [independence](../../../random-variable.md#independent-random-variables) of the $D_j$. Similarly $X^n_{s+t}-X^n_s\overset d=X^n_t$ passes to the limit, proving [stationary increments](../../../stochastic-process.md#stationary-increments) for $X$.

It remains to prove [stochastic continuity](../../../stochastic-process.md#stochastic-continuity). For $\varepsilon>0$, the [triangle inequality](../../../topological-analysis.md#triangle-inequality) and the [union bound](../../../probability-inequality.md#boole-s-inequality) imply, for every fixed $n$,

$$
\begin{aligned}
\limsup_{t\downarrow0}\mathbb P(|X_t|>\varepsilon)
&\leq\limsup_{t\downarrow0}\mathbb P(|X_t-X_t^n|>\varepsilon/2)
+\limsup_{t\downarrow0}\mathbb P(|X_t^n|>\varepsilon/2)\\
&=\limsup_{t\downarrow0}\mathbb P(|X_t-X_t^n|>\varepsilon/2).
\end{aligned}
$$

The second term vanishes by [stochastic continuity](../../../stochastic-process.md#stochastic-continuity) of $X^n$. Now let $n\to\infty$ and use the additional near-zero approximation hypothesis. We obtain $X_t\to0$ in probability as $t\downarrow0$. The [stationary increments](../../../stochastic-process.md#stationary-increments) transfer this to every time: both $X_{s+h}-X_s$ and $X_s-X_{s-h}$ have the law of $X_h$ for $h>0$ when defined. Thus **$X$ has all the intrinsic [Lévy process](../../../stochastic-process.md#levy-process) properties**, proving [closure of Lévy processes under locally controlled convergence in probability](../../../stochastic-process.md#closure-of-levy-processes-under-locally-controlled-convergence-in-probability).

If one requires the supplied process itself to be [càdlàg](../../../calculus.md#cadlag), the hypotheses justify a [càdlàg modification](../../../stochastic-process.md#cadlag-modification), rather than that stronger pathwise assertion. To see the distinction, take $X^n\equiv0$, let $U$ have [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) on $(0,1)$, and put $X_t=\mathbf1_{\{t=U\}}$. At each fixed time $t$, $X_t=0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), so both approximation hypotheses hold with zero error probability. Nevertheless every path has an isolated spike at $U$ and is not right-continuous there. Its identically zero [modification of a stochastic process](../../../stochastic-process.md#modification-of-a-stochastic-process) is a [Lévy process](../../../stochastic-process.md#levy-process) with [càdlàg](../../../calculus.md#cadlag) paths. **The conclusion is exact under the intrinsic definition, and exact up to modification under the convention requiring [càdlàg](../../../calculus.md#cadlag) paths.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
