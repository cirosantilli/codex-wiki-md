# Paper 201

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20201.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20201.pdf)

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
    - [i](#4/d/i)
      - [Solution](#4/d/i/solution)
    - [ii](#4/d/ii)
      - [Solution](#4/d/ii/solution)
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
  - [e](#6/e)
    - [Solution](#6/e/solution)

## 1

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The finite [sigma-algebra](../../../measure-theory.md#sigma-algebra) $\mathcal F_n=\sigma(A_1,\ldots,A_n)$ is partitioned by the nonempty [events](../../../probability-theory.md#event)

$$
C=\bigcap_{j=1}^n B_j,
\qquad B_j\in\{A_j,A_j^c\}.
$$

These are its [atoms](../../../measure-theory.md#atom-of-a-sigma-algebra). Define the [random variable](../../../random-variable.md)

$$
X_n=\sum_{C:\,\mathbb P(C)>0}
\frac{\mathbb E[X\mathbf1_C]}{\mathbb P(C)}\mathbf1_C,
$$

and give it any finite value on the union of the null atoms. It is $\mathcal F_n$-measurable and [integrable](../../../measure-theory.md#lebesgue-integrable-function). Every $A\in\mathcal F_n$ is a union of atoms, so

$$
\mathbb E[X_n\mathbf1_A]
=\sum_{C\subseteq A}\mathbb E[X\mathbf1_C]
=\mathbb E[X\mathbf1_A].
$$

This constructs the requested variable directly, without invoking the general existence theorem for [conditional expectation](../../../measure-theory.md#conditional-expectation).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Uniqueness means [almost sure equality](../../../convergence-of-random-variables.md#almost-sure-equality). Suppose that two $\mathcal F_n$-measurable integrable random variables $Y$ and $Z$ satisfy the integral identity from part (a). The event $D=\{Y>Z\}$ belongs to $\mathcal F_n$, and hence

$$
\mathbb E[(Y-Z)\mathbf1_D]=0.
$$

The integrand is nonnegative and is positive precisely on $D$, so $\mathbb P(D)=0$. Interchanging $Y$ and $Z$ gives $\mathbb P(Z>Y)=0$, and therefore $Y=Z$ almost surely.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For $A\in\mathcal F_n$, the defining identity for $X_{n+1}$ gives

$$
\mathbb E[X_{n+1}\mathbf1_A]=\mathbb E[X\mathbf1_A]
=\mathbb E[X_n\mathbf1_A].
$$

Part (b) therefore identifies $X_n$ with $\mathbb E[X_{n+1}\mid\mathcal F_n]$, so $(X_n,\mathcal F_n)$ is a [martingale](../../../martingale.md).

The atom formula also proves

$$
|X_n|\leq\mathbb E[|X|\mid\mathcal F_n].
$$

Let $B_{n,K}=\{|X_n|>K\}$. Then $\mathbb P(B_{n,K})\leq\mathbb E|X|/K$ by [Markov inequality](../../../probability-inequality.md#markov-inequality), while

$$
\mathbb E[|X_n|\mathbf1_{B_{n,K}}]
\leq\mathbb E[|X|\mathbf1_{B_{n,K}}].
$$

The [uniform absolute continuity for a finite measure](../../../measure-theory.md#uniform-absolute-continuity-for-a-finite-measure) makes the right-hand side uniformly small as $K\to\infty$. Thus $(X_n)$ is [uniformly integrable](../../../convergence-of-random-variables.md#uniform-integrability). The [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem) now supplies an integrable random variable $Y$ such that $X_n\to Y$ both [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) and in $L^1$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Let $\mathcal G=\sigma(A_1,A_2,\ldots)$. The limit $Y$ from part (c) is $\mathcal G$-measurable because each $X_n$ is. If $A\in\bigcup_n\mathcal F_n$, then $A\in\mathcal F_N$ for some $N$, and for every $n\geq N$,

$$
\mathbb E[X_n\mathbf1_A]=\mathbb E[X\mathbf1_A].
$$

The $L^1$ convergence lets us pass to the limit and obtain $\mathbb E[Y\mathbf1_A]=\mathbb E[X\mathbf1_A]$.

The sets on which this identity holds form a [Dynkin system](../../../measure-theory.md#dynkin-system), and $\bigcup_n\mathcal F_n$ is a generating [pi-system](../../../measure-theory.md#pi-system). The [Dynkin lemma](../../../measure-theory.md#dynkin-lemma) therefore extends the identity to every $A\in\mathcal G$. Consequently $Y$ has both defining properties of $\mathbb E[X\mid\mathcal G]$, established here without appealing to the general existence theorem.

## 2

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For an integrable real [random variable](../../../random-variable.md) $X$, its [cumulant-generating function](../../../probability-theory.md#cumulant-generating-function) is the extended-real [convex function](../../../real-analysis.md#convex-function)

$$
\psi(\theta)=\log\mathbb E[e^{\theta X}],
\qquad \theta\in\mathbb R,
$$

where $\psi(\theta)=+\infty$ if the [exponential moment](../../../probability-theory.md#exponential-moment) diverges. Its [Legendre transform of a cumulant-generating function](../../../probability-theory.md#legendre-transform-of-a-cumulant-generating-function) is

$$
\boxed{\psi^*(x)=\sup_{\theta\in\mathbb R}\{\theta x-\psi(\theta)\}.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $X_1,X_2,\ldots$ be [independent and identically distributed random variables](../../../random-variable.md#independent-and-identically-distributed-random-variables), let $S_n=\sum_{j=1}^nX_j$, and write $m=\mathbb E X_1$. [Cramér theorem](../../../probability-theory.md#cramer-s-theorem) states that the empirical means $S_n/n$ obey a [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle) with good [rate function](../../../convergence-of-random-variables.md#rate-function) $\psi^*$. In particular, for $x\geq m$,

$$
\lim_{n\to\infty}\frac1n\log\mathbb P(S_n/n\geq x)=-\psi^*(x),
$$

with the usual extended-real interpretation; the analogous lower-tail formula holds for $x\leq m$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For every $\theta\geq0$, the [exponential Markov bound](../../../probability-inequality.md#exponential-markov-bound) and [independence](../../../random-variable.md#independent-random-variables) give

$$
\mathbb P(S_n/n\geq x)
=\mathbb P(e^{\theta S_n}\geq e^{n\theta x})
\leq e^{-n\theta x}\mathbb E e^{\theta S_n}
=\exp\{-n(\theta x-\psi(\theta))\}.
$$

Taking the [infimum](../../../real-analysis.md#infimum) over $\theta\geq0$ yields

$$
\limsup_{n\to\infty}\frac1n\log\mathbb P(S_n/n\geq x)
\leq-\sup_{\theta\geq0}(\theta x-\psi(\theta)).
$$

For $x\geq m$, [convexity](../../../real-analysis.md#convex-function) makes this supremum equal to $\psi^*(x)$, proving the upper bound in the stated tail form of [Cramér theorem](../../../probability-theory.md#cramer-s-theorem).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Fix $a>m$ and then $x>a$. By the assumptions on the [derivative](../../../calculus.md#derivative) $\psi'$, there is a unique $\theta_x>0$ with $\psi'(\theta_x)=x$. Apply [exponential tilting](../../../probability-theory.md#exponential-tilting) to each summand:

$$
\frac{d\mathbb P_{\theta_x}}{d\mathbb P}(y)
=e^{\theta_xy-\psi(\theta_x)}.
$$

Under the product tilted law, the variables remain [independent and identically distributed random variables](../../../random-variable.md#independent-and-identically-distributed-random-variables) and have mean $x$. Hence the [strong law of large numbers](../../../convergence-of-random-variables.md#strong-law-of-large-numbers) implies that, for every $0<\delta<x-a$,

$$
\mathbb P_{\theta_x}(|S_n/n-x|<\delta)\longrightarrow1.
$$

Changing measure on this event gives

$$
\mathbb P(S_n/n\geq a)
\geq e^{-n[\theta_x(x+\delta)-\psi(\theta_x)]}
\mathbb P_{\theta_x}(|S_n/n-x|<\delta).
$$

Therefore

$$
\liminf_{n\to\infty}\frac1n\log\mathbb P(S_n/n\geq a)
\geq-\psi^*(x)-\theta_x\delta.
$$

First let $\delta\downarrow0$ and then $x\downarrow a$. The [continuity of a convex function](../../../real-analysis.md#continuity-of-a-convex-function) gives the lower bound $-\psi^*(a)$. The endpoint $a=m$ follows by letting $a\downarrow m$, while for $a<m$ the [strong law of large numbers](../../../convergence-of-random-variables.md#strong-law-of-large-numbers) makes the probability tend to one. This proves the required lower bound.

## 3

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Let $(M_k,\mathcal F_k)_{k=0}^N$ be a [martingale](../../../martingale.md), let $a<b$, and let $U_N[a,b]$ count the completed upcrossings of $[a,b]$ by time $N$. [Doob upcrossing inequality](../../../martingale.md#doob-upcrossing-inequality) states

$$
(b-a)\mathbb E U_N[a,b]\leq\mathbb E(M_N-a)^-.
$$

Equivalent conventions for a process with a prescribed initial holding add the corresponding endpoint term.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Assume $\sup_n\mathbb E|M_n|<\infty$. For every pair of [rationals](../../../number-theory.md#rational-number) $a<b$, [Doob upcrossing inequality](../../../martingale.md#doob-upcrossing-inequality) gives

$$
(b-a)\mathbb E U_\infty[a,b]
\leq\sup_n\mathbb E(M_n-a)^-<\infty
$$

by [monotone convergence theorem](../../../measure-theory.md#monotone-convergence-theorem). Thus every rational interval is upcrossed only finitely often almost surely. If a real sequence has distinct [limit inferior](../../../real-analysis.md#limit-inferior) and [limit superior](../../../real-analysis.md#limit-superior), it completes infinitely many upcrossings of some rational interval between them. Hence $M_n$ converges in the [extended real line](../../../arithmetic.md#extended-real-number-line) almost surely.

[Fatou lemma](../../../measure-theory.md#fatou-s-lemma) gives

$$
\mathbb E\!\left[\liminf_n|M_n|\right]
\leq\liminf_n\mathbb E|M_n|<\infty,
$$

so the limit is finite almost surely and integrable. This is the $L^1$-bounded form of the [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let $(M_t)_{t\geq0}$ be a right-continuous [continuous-time martingale](../../../martingale.md#continuous-time-martingale) with $\sup_t\mathbb E|M_t|<\infty$. Restricting it to the nonnegative rational times gives a countable martingale. The argument of part (b), applied on successively finer rational grids, shows that it has a finite almost-sure limit as the rational time tends to infinity. [Right-continuity](../../../calculus.md#right-continuous-function) and the upcrossing characterization prevent the values at arbitrary times from having a different limit. Thus $M_t$ converges almost surely to a finite integrable random variable as $t\to\infty$, which is the [Continuous-time martingale convergence theorem](../../../martingale.md#continuous-time-martingale-convergence-theorem).

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Let $(B_t)$ be [Brownian motion](../../../brownian-motion.md) in $\mathbb R^3$ started at a nonzero point. The function $h(x)=|x|^{-1}$ is a positive [harmonic function](../../../partial-differential-equation.md#harmonic-function) on $\mathbb R^3\setminus\{0\}$ because its [Laplacian](../../../partial-differential-equation.md#laplace-operator) vanishes there. Stopping on annuli and applying [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) shows that $h(B_t)$ is a [local martingale](../../../martingale.md#local-martingale). Letting the inner boundary shrink to zero also shows that three-dimensional Brownian motion does not hit the origin.

A positive local martingale is a [supermartingale](../../../martingale.md#supermartingale), so $h(B_t)$ is $L^1$-bounded by $h(B_0)$. The upcrossing proof from part (c), which applies verbatim to a positive supermartingale, therefore gives a finite almost-sure limit

$$
\boxed{|B_t|^{-1}\longrightarrow Y.}
$$

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

By [Brownian scaling](../../../brownian-motion.md#brownian-scaling),

$$
|B_t|^{-1}\stackrel d=
t^{-1/2}|Z+t^{-1/2}B_0|^{-1},
$$

where $Z$ has the standard three-dimensional [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution). The right-hand side tends to zero in [probability](../../../convergence-of-random-variables.md#convergence-in-probability), since $Z$ has no atom at the origin. Part (d) gives almost-sure convergence to $Y$, which also implies convergence in probability to $Y$. [Uniqueness of a limit in probability](../../../convergence-of-random-variables.md#uniqueness-of-a-limit-in-probability) therefore gives $Y=0$ almost surely. Hence $|B_t|\to\infty$ almost surely, proving the [transience of Brownian motion in dimension at least three](../../../brownian-motion.md#transience-of-brownian-motion-in-dimension-at-least-three) in dimension three.

## 4

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A standard [Brownian motion](../../../brownian-motion.md) $(B_t)_{t\geq0}$ satisfies $B_0=0$ almost surely, has almost surely [continuous](../../../calculus.md#continuous-function) sample paths, and has independent stationary increments such that

$$
\boxed{B_t-B_s\sim N(0,t-s)
\qquad(0\leq s<t).}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The variable $Z=\int_0^1B_t\,dt$ is the $L^2$ limit of [Riemann sums](../../../real-analysis.md#riemann-sum) of the [Gaussian process](../../../stochastic-process.md#gaussian-process) $B$, so it is a [Gaussian random variable](../../../probability-theory.md#normal-distribution). Its mean is zero, and [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem) with $\mathbb E[B_sB_t]=\min(s,t)$ gives

$$
\operatorname{Var}(Z)
=\int_0^1\!\int_0^1\min(s,t)\,ds\,dt
=2\int_0^1\!\int_0^t s\,ds\,dt
=\frac13.
$$

**Therefore $Z\sim N(0,1/3)$.**

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Let $X_1,X_2,\ldots$ be [independent and identically distributed random variables](../../../random-variable.md#independent-and-identically-distributed-random-variables) with mean zero and variance one, and let $S_k=\sum_{j=1}^kX_j$. Define the linearly interpolated process

$$
W_n(t)=\frac1{\sqrt n}
\left(S_{\lfloor nt\rfloor}+(nt-\lfloor nt\rfloor)X_{\lfloor nt\rfloor+1}\right),
\qquad0\leq t\leq1.
$$

The [Donsker invariance principle](../../../convergence-of-random-variables.md#donsker-s-theorem), also called the [functional central limit theorem](../../../convergence-of-random-variables.md#donsker-s-theorem), states that $W_n$ converges [weakly](../../../convergence-of-random-variables.md#convergence-in-distribution) in the space $C[0,1]$ with the [uniform norm](../../../functional-analysis.md#supremum-norm) to standard [Brownian motion](../../../brownian-motion.md).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/i">i</h4>

↑ **Parent:** [D](#4/d)

<h5 id="4/d/i/solution">Solution</h5>

↑ **Parent:** [I](#4/d/i)

The evaluation map $f\mapsto f(1)$ is [continuous](../../../calculus.md#continuous-function) on $C[0,1]$ in the [uniform norm](../../../functional-analysis.md#supremum-norm). The [continuous mapping theorem](../../../convergence-of-random-variables.md#continuous-mapping-theorem) applied to part (c) therefore gives

$$
\frac1{\sqrt n}\sum_{k=1}^nX_k=W_n(1)
\xrightarrow d B_1\sim N(0,1).
$$

This recovers the [central limit theorem](../../../convergence-of-random-variables.md#central-limit-theorem) from the functional version.

<h4 id="4/d/ii">ii</h4>

↑ **Parent:** [D](#4/d)

<h5 id="4/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/d/ii)

Reversing the finite summations gives

$$
\frac1{n^{3/2}}\sum_{k=1}^n\sum_{j=1}^kX_j
=\frac1n\sum_{k=1}^n\frac{S_k}{\sqrt n}.
$$

This is a [Riemann sum](../../../real-analysis.md#riemann-sum) for the continuous functional $f\mapsto\int_0^1f(t)\,dt$ evaluated at the interpolated random walk; the interpolation error tends to zero in probability. The [continuous mapping theorem](../../../convergence-of-random-variables.md#continuous-mapping-theorem) and part (b) yield

$$
\boxed{\frac1{n^{3/2}}\sum_{k=1}^n\sum_{j=1}^kX_j
\xrightarrow d\int_0^1B_t\,dt
\sim N(0,1/3).}
$$

## 5

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Let $D\subset\mathbb R^d$ be bounded, choose $R$ with $D\subset B(0,R)$, and let $T$ and $\tau_R$ be the respective [exit times](../../../brownian-motion.md#brownian-exit-time). Then $T\leq\tau_R$. Since

$$
|B_t|^2-dt
$$

is a [martingale](../../../martingale.md), the [optional sampling theorem for a supermartingale](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) at $\tau_R\wedge n$ gives

$$
d\,\mathbb E_x(\tau_R\wedge n)
=\mathbb E_x|B_{\tau_R\wedge n}|^2-|x|^2
\leq R^2-|x|^2.
$$

[Monotone convergence theorem](../../../measure-theory.md#monotone-convergence-theorem) now gives

$$
\boxed{\mathbb E_xT\leq\mathbb E_x\tau_R
\leq\frac{R^2-|x|^2}{d}<\infty.}
$$

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

For $u\in C^2(\overline D)$, [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) shows that

$$
u(B_{t\wedge T})-u(x)
-\frac12\int_0^{t\wedge T}\Delta u(B_s)\,ds
$$

is a [martingale](../../../martingale.md). Take [expectations](../../../probability-theory.md#expected-value) and let $t\to\infty$. The function $u$ is bounded on the [compact set](../../../topology.md#compact-space) $\overline D$, while $\Delta u$ is bounded and $\mathbb E_xT<\infty$ by part (a). The [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) therefore gives [Dynkin formula for Brownian motion](../../../brownian-motion.md#dynkin-formula-for-brownian-motion)

$$
\boxed{\mathbb E_xu(B_T)
=u(x)+\frac12\mathbb E_x\int_0^T\Delta u(B_s)\,ds.}
$$

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Apply part (b) to $u_n$. Its zero [boundary value](../../../differential-equation.md#dirichlet-boundary-condition) gives

$$
u_n(x)=-\frac12\mathbb E_x\int_0^T\Delta u_n(B_s)\,ds.
$$

The assumptions say that $\Delta u_n(y)\to0$ for every $y\in D$ and that $|\Delta u_n|\leq C$ uniformly. Thus the integrand converges pointwise to zero and is dominated by $CT$, whose expectation is finite by part (a). The [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) gives $u_n(x)\to0$ for every $x\in D$.

## 6

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

A [Lévy process](../../../stochastic-process.md#levy-process) $(X_t)_{t\geq0}$ starts at zero, has [independent](../../../random-variable.md#independent-random-variables) and stationary increments, is [stochastically continuous](../../../stochastic-process.md#stochastic-continuity), and is taken with [càdlàg](../../../calculus.md#cadlag) sample paths. Thus for $0\leq t_0<\cdots<t_n$, the increments $X_{t_j}-X_{t_{j-1}}$ are independent, and the law of $X_{s+t}-X_s$ depends only on $t$.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Write $\mathbb E X_1=\mu$ and $\operatorname{Var}(X_1)=\sigma^2<\infty$. For rational $t=m/n$, stationarity and independence of the $n$ increments over intervals of length $1/n$ give

$$
\mathbb E X_t=t\mu,
\qquad
\operatorname{Var}(X_t)=t\sigma^2,
$$

using [variance additivity for independent random variables](../../../variance.md#variance-additivity-for-independent-random-variables). [Stochastic continuity](../../../stochastic-process.md#stochastic-continuity) extends both identities from rational to real $t$. In the centered case $\mu=0$, this becomes $\mathbb E X_t=0$ and $\mathbb E X_t^2=t\sigma^2$.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

For $s<t$, write $X_t=X_s+Y$, where the increment $Y=X_t-X_s$ is independent of the [natural filtration](../../../stochastic-process.md#natural-filtration) at time $s$, has mean zero, and has variance $(t-s)\sigma^2$. Hence

$$
\mathbb E[X_t^2\mid\mathcal F_s]
=X_s^2+\mathbb E[Y^2]
=X_s^2+(t-s)\sigma^2.
$$

It follows that $M_t=X_t^2-t\sigma^2$ is a martingale, as asserted by the [centered square-integrable Lévy martingale](../../../stochastic-process.md#centered-square-integrable-levy-martingale) identity.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

Let $T=\inf\{t\geq0:X_t\notin(-a,b)\}$, and suppose the jumps of $X$ have absolute value at most $c$. A nonconstant centered finite-variance [Lévy process](../../../stochastic-process.md#levy-process) oscillates, so $T<\infty$ almost surely. Before $T$ the process lies in $(-a,b)$, and at $T$ its bounded overshoot gives $X_T\in[-a-c,b+c]$. Thus the variables $X_{T\wedge n}^2$ are uniformly bounded.

Apply the [optional sampling theorem for a supermartingale](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) to the martingale from part (c):

$$
\mathbb E[X_{T\wedge n}^2]
=\sigma^2\mathbb E[T\wedge n].
$$

[Bounded convergence theorem](../../../measure-theory.md#bounded-convergence-theorem) on the left and [monotone convergence theorem](../../../measure-theory.md#monotone-convergence-theorem) on the right yield

$$
\boxed{\mathbb E[X_T^2]=\sigma^2\mathbb E[T].}
$$

<h3 id="6/e">e</h3>

↑ **Parent:** [6](#6)

<h4 id="6/e/solution">Solution</h4>

↑ **Parent:** [E](#6/e)

Let $X_t=N_t^+-N_t^-$, where $N^+$ and $N^-$ are independent [Poisson processes](../../../probability-theory.md#poisson-process) of rate $\lambda$. This [symmetric Poisson difference process](../../../probability-theory.md#symmetric-poisson-difference-process) is centered, has jumps $\pm1$, and has variance rate $\sigma^2=2\lambda$. If $a,b$ are positive integers, then $X_T\in\{-a,b\}$ exactly. Optional sampling of the martingale $X_t$ gives

$$
\mathbb P(X_T=b)=\frac{a}{a+b},
\qquad
\mathbb P(X_T=-a)=\frac{b}{a+b}.
$$

Consequently

$$
\mathbb E[X_T^2]
=b^2\frac{a}{a+b}+a^2\frac{b}{a+b}
=ab.
$$

Part (d) now gives the [mean exit time](../../../probability-theory.md#expected-value)

$$
\boxed{\mathbb E T=\frac{ab}{2\lambda}.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
