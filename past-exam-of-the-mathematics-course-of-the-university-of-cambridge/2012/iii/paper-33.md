# Paper 33

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_33.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_33.pdf)

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

## 1

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use the [natural filtration](../../../stochastic-process.md#natural-filtration) $\mathcal F_n=\sigma(X_1,\ldots,X_n)$ of the [simple symmetric random walk](../../../probability-theory.md#simple-symmetric-random-walk). The event $\{T_1\leq n\}=\bigcup_{k=0}^n\{S_k=1\}$ belongs to $\mathcal F_n$, so $T_1$ is a [stopping time](../../../martingale.md#stopping-time).

For a positive integer $m$, set $\tau_m=T_1\wedge T_{-m}$. This exit time from the finite interval is integrable: in each block of $m+1$ steps there is a [probability](../../../probability-theory.md#probability) at least $2^{-(m+1)}$ of all steps being positive, which forces exit if it has not already occurred. Consequently the survival [probabilities](../../../probability-theory.md#probability) have a geometric upper bound.

We use the bounded-time [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale): if $M$ is a [martingale](../../../martingale.md) and $\sigma$ a bounded [stopping time](../../../martingale.md#stopping-time), then $\mathbb E M_\sigma=\mathbb E M_0$. Apply it at $\tau_m\wedge n$ to $S_n$ and to the [square-minus-time martingale of a simple symmetric random walk](../../../probability-theory.md#square-minus-time-martingale-of-a-simple-symmetric-random-walk) $S_n^2-n$. The stopped positions lie in $[-m,1]$, so [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem) and [monotone convergence](../../../measure-theory.md#monotone-convergence-theorem) give

$$
\mathbb E S_{\tau_m}=0,\qquad \mathbb E\tau_m=\mathbb E S_{\tau_m}^2.
$$

Writing $p_m=\mathbb P(T_1<T_{-m})$, the first equation becomes $p_m-m(1-p_m)=0$, hence $p_m=m/(m+1)$. The second gives $\mathbb E\tau_m=p_m+m^2(1-p_m)=m$. Since $\tau_m\leq T_1$, its [expectation](../../../probability-theory.md#expected-value) satisfies $\mathbb E T_1\geq m$ for every $m$. Therefore

$$
\boxed{\mathbb E T_1=+\infty.}
$$

Nevertheless $\mathbb P(T_1<\infty)\geq p_m\to1$. Thus the [infinite mean first passage of a simple symmetric random walk](../../../probability-theory.md#infinite-mean-first-passage-of-a-simple-symmetric-random-walk) occurs despite almost sure finiteness; using unrestricted optional stopping directly at $T_1$ would be unjustified.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Define the [stopped martingale](../../../martingale.md#stopped-martingale)

$$
\boxed{M_n=1-S_{n\wedge T_1}.}
$$

It is nonnegative: before the first visit to $1$, the nearest-neighbour [random walk](../../../markov-process.md#random-walk) is at most $0$, and afterwards the stopped position is $1$. Each $M_n$ is integrable, with $|M_n|\leq n+1$. Moreover

$$
M_{n+1}-M_n=-\mathbf1_{\{T_1>n\}}X_{n+1}.
$$

The indicator is $\mathcal F_n$-measurable and the increment has conditional mean zero, so $M_n$ is a [martingale](../../../martingale.md) with $\mathbb E M_n=M_0=1$.

Part (a) shows $T_1<\infty$ almost surely, so every such path eventually has $M_n=0$. Thus $M_n\to0$ almost surely. But $\mathbb E|M_n-0|=1$ for every $n$, so there is no [convergence in L1](../../../convergence-of-random-variables.md#convergence-in-l1). Any possible [L1 convergence](../../../convergence-of-random-variables.md#convergence-in-l1) limit would agree with the almost sure limit. This is a **nonnegative [martingale](../../../martingale.md) with [almost sure convergence](../../../convergence-of-random-variables.md#almost-sure-convergence) but no [convergence in L1](../../../convergence-of-random-variables.md#convergence-in-l1)**, and hence it is not [uniformly integrable](../../../convergence-of-random-variables.md#uniform-integrability).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Because each increment is $\pm1$, the event at time $k$ defining $T$ is exactly $\{X_{k-1}=X_k=1\}$. Therefore, for $n\geq2$,

$$
\{T\leq n\}=\bigcup_{k=2}^n\{X_{k-1}=X_k=1\}\in\mathcal F_n,
$$

and for $n<2$ this event is empty. Thus **$T$ is a [stopping time](../../../martingale.md#stopping-time)** for the [natural filtration](../../../stochastic-process.md#natural-filtration).

On the other hand, $\{U\leq0\}=\{T=2\}=\{X_1=X_2=1\}$. This event has [probability](../../../probability-theory.md#probability) $1/4$, whereas the initial [sigma-algebra](../../../measure-theory.md#sigma-algebra) $\mathcal F_0$ is trivial, even after completion up to null sets. It therefore cannot belong to $\mathcal F_0$. Hence **$U=T-2$ is not a [stopping time](../../../martingale.md#stopping-time)**. Subtracting a deterministic delay from a [stopping time](../../../martingale.md#stopping-time) can require information from the future.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The time $T$ is the [waiting time for two consecutive successes](../../../martingale.md#waiting-time-for-two-consecutive-successes) in [independent](../../../random-variable.md#independent-random-variables) fair trials. First note its integrability: if any one of the disjoint pairs $(X_1,X_2),\ldots,(X_{2k-1},X_{2k})$ is $++$, then $T\leq2k$. Thus $\mathbb P(T>2k)\leq(3/4)^k$.

Let $e_0$ be the expected additional waiting time with no trailing positive step, and let $e_1$ be the expected additional time when the preceding step was positive. Conditioning on the next [independent](../../../random-variable.md#independent-random-variables) increment gives

$$
e_0=1+\tfrac12e_0+\tfrac12e_1,\qquad e_1=1+\tfrac12e_0.
$$

A negative step returns either state to state $0$; a positive step moves state $0$ to state $1$ and completes the pattern from state $1$. Substitution yields $e_0=2+e_1=3+e_0/2$, so $e_0=6$. The original process starts in state $0$, and therefore

$$
\boxed{\mathbb E T=6.}
$$

Overlapping pairs are dependent, so regarding each successive pair as a fresh trial of success [probability](../../../probability-theory.md#probability) $1/4$ would give the wrong [expectation](../../../probability-theory.md#expected-value).

## 2

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $Y_i$ be [independent and identically distributed random variables](../../../random-variable.md#independent-and-identically-distributed-random-variables) with [moment-generating function](../../../probability-theory.md#moment-generating-function) finite on an open interval about $0$. Put

$$
\Lambda(\theta)=\log\mathbb E e^{\theta Y_1},\qquad I(x)=\sup_{\theta\in\mathbb R}\{\theta x-\Lambda(\theta)\},
$$

allowing $\Lambda=+\infty$ outside its finite domain. The [Cramér theorem](../../../probability-theory.md#cramer-s-theorem) states that $\bar Y_n=n^{-1}\sum_{i=1}^nY_i$ satisfies a [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle) with speed $n$ and good [rate function](../../../convergence-of-random-variables.md#rate-function) $I$, the [Legendre transform of a cumulant-generating function](../../../probability-theory.md#legendre-transform-of-a-cumulant-generating-function). Explicitly, for every closed set $F$ and open set $O$,

$$
\limsup_{n\to\infty}\frac1n\log\mathbb P(\bar Y_n\in F)\leq-\inf_{x\in F}I(x),\qquad
\liminf_{n\to\infty}\frac1n\log\mathbb P(\bar Y_n\in O)\geq-\inf_{x\in O}I(x).
$$

Here $\log0=-\infty$ and $\inf\varnothing=+\infty$. The [rate function](../../../convergence-of-random-variables.md#rate-function) is lower semicontinuous and its finite sublevel sets are compact. **The exponential-moment hypothesis is essential for this form of the [Cramér theorem](../../../probability-theory.md#cramer-s-theorem).**

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For the unit-rate [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution), direct integration gives

$$
\mathbb E e^{\theta Y_1}=\frac1{1-\theta}\quad(\theta<1),\qquad \Lambda(\theta)=-\log(1-\theta).
$$

For $x>0$, maximizing $\theta x+\log(1-\theta)$ gives $\theta=1-1/x$, and therefore $I(x)=x-1-\log x$. For $x\leq0$ the supremum is infinite, as seen by taking $\theta\to-\infty$.

For $a>1$, $I$ is increasing on $[a,\infty)$, and its continuity gives $\inf_{[a,\infty)}I=\inf_{(a,\infty)}I=I(a)$. The closed-set upper bound and open-set lower bound of the [Cramér theorem](../../../probability-theory.md#cramer-s-theorem) squeeze the desired limit to $-I(a)$. For $a=1$, both infima are $0$, because $I(1)=0$ and $I(x)\to0$ as $x\downarrow1$. For $0\leq a<1$, the [strong law of large numbers](../../../convergence-of-random-variables.md#strong-law-of-large-numbers) gives $S_n/n\to1$ almost surely, so the tail [probability](../../../probability-theory.md#probability) tends to $1$; at $a=0$ it is identically $1$.

Consequently the [exponential sample-mean upper-tail rate](../../../probability-theory.md#exponential-sample-mean-upper-tail-rate) is

$$
\boxed{\lim_{n\to\infty}\frac1n\log\mathbb P(S_n\geq na)=\begin{cases}0,&0\leq a\leq1,\\-(a-1-\log a),&a>1.\end{cases}}
$$

The threshold case uses the rate-function lower bound on the open half-line, rather than applying the law of large numbers at equality.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The transformation of the [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) gives, for $x\geq1$,

$$
\mathbb P(X_1\geq x)=\mathbb P(U_1\leq x^{-2})=x^{-2}.
$$

Thus $X_1$ has a [Pareto distribution](../../../continuous-probability-distribution.md#pareto-distribution) with lower endpoint $1$ and shape $2$. It has mean $2$, but no positive exponential moments, so the preceding version of the [Cramér theorem](../../../probability-theory.md#cramer-s-theorem) is unavailable.

At $a=0$, the event in question is certain. For every fixed $a>0$ and all sufficiently large $n$, positivity of the summands gives the [one-big-jump polynomial lower bound](../../../continuous-probability-distribution.md#one-big-jump-polynomial-lower-bound)

$$
1\geq\mathbb P(W_n\geq na)\geq\mathbb P(X_1\geq na)=(na)^{-2}.
$$

Taking logarithms and dividing by $n$ gives an upper bound $0$ and a lower bound $-2\log(na)/n\to0$. Hence

$$
\boxed{\lim_{n\to\infty}\frac1n\log\mathbb P(W_n\geq na)=0\quad\text{for every }a\geq0.}
$$

This covers thresholds below, at and above the mean. Above the mean it means decay is slower than exponential speed $n$, not that the tail [probability](../../../probability-theory.md#probability) tends to $1$.

## 3

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

On a [measurable space](../../../measure-theory.md#measurable-space) $(E,\mathcal E)$ with a sigma-finite [measure](../../../measure-theory.md#measure) $\mu$, a [Poisson random measure](../../../probability-theory.md#poisson-random-measure) $N$ is a random counting measure such that $N(A)$ has the [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) with parameter $\mu(A)$ for every measurable $A$ of finite intensity, and the counts on finitely many pairwise disjoint measurable sets are [independent](../../../random-variable.md#independent-random-variables). The sample measures are countably additive; repeated atoms are allowed if the intensity has atoms.

When $\mu(A)=\infty$, exhaustion by finite-intensity subsets gives $N(A)=\infty$ almost surely. Indeed their counts increase, and the [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) [probability](../../../probability-theory.md#probability) of a count at most any fixed integer tends to zero as the parameter tends to infinity. **[Independent](../../../random-variable.md#independent-random-variables) Poisson counts on disjoint sets, with means prescribed by $\mu$, characterize the [Poisson random measure](../../../probability-theory.md#poisson-random-measure).**

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For a measurable $A$ with $(\mu+\nu)(A)<\infty$, independence of the two [Poisson random measures](../../../probability-theory.md#poisson-random-measure) gives

$$
\mathbb P((\Phi+\Psi)(A)=k)=\sum_{j=0}^k e^{-\mu(A)}\frac{\mu(A)^j}{j!}e^{-\nu(A)}\frac{\nu(A)^{k-j}}{(k-j)!}
=e^{-(\mu+\nu)(A)}\frac{((\mu+\nu)(A))^k}{k!}.
$$

Thus its count has the [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) with the summed parameter. If $A_1,\ldots,A_m$ are disjoint, the variables within each family of counts are [independent](../../../random-variable.md#independent-random-variables), and independence of $\Phi$ and $\Psi$ makes the two families [independent](../../../random-variable.md#independent-random-variables) of each other. Hence the pairs $(\Phi(A_j),\Psi(A_j))$, and therefore their sums, are [independent](../../../random-variable.md#independent-random-variables) over $j$.

Adding sample counting measures preserves countable additivity. The definition in (a) therefore proves

$$
\boxed{\Phi+\Psi\text{ is a Poisson random measure of intensity }\mu+\nu.}
$$

This proves the required [Superposition theorem for Poisson point processes](../../../probability-theory.md#superposition-theorem-for-poisson-point-processes) directly from count distributions.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Interpret the second process as an [independent](../../../random-variable.md#independent-random-variables) copy of the unit-rate [Poisson process](../../../probability-theory.md#poisson-process). First, the sums are finite almost surely. On $[0,1]$ there are finitely many arrivals, none at $0$, so their inverse-square contributions are finite. On $[1,\infty)$,

$$
\mathbb E\sum_{Z_i\geq1}Z_i^{-2}=\int_1^\infty z^{-2}\,dz=1.
$$

For completeness, this [expectation](../../../probability-theory.md#expected-value) identity follows first for nonnegative simple functions from $\mathbb E N(A)=|A|$, and then for all nonnegative measurable functions by [monotone convergence](../../../measure-theory.md#monotone-convergence-theorem). Thus no unproved Poisson-integral formula is needed, and the tail sum is finite almost surely.

By (b), merging the two processes produces a rate-$2$ [Poisson process](../../../probability-theory.md#poisson-process) with arrival times $V_i$. Its rescaled arrivals $2V_i$ form a unit-rate [Poisson process](../../../probability-theory.md#poisson-process): for a measurable set $A$, their count is the merged count on $A/2$, with parameter $2|A/2|=|A|$, and disjoint-set independence is preserved. Consequently

$$
X+Y=\sum_iV_i^{-2}=4\sum_i(2V_i)^{-2}\ \stackrel{d}{=}\ 4X.
$$

Therefore **$\boxed{c=4}$**. This is the scaling of an [inverse-power sum over Poisson arrivals](../../../probability-theory.md#inverse-power-sum-over-poisson-arrivals) with exponent $2$.

The PDF does not explicitly repeat the second process's rate. If that rate were $\rho$ rather than $1$, the same count argument would give $X+Y\stackrel d=(1+\rho)^2X$. The numerical value $4$ uses the intended independent-unit-rate-copy interpretation.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Use the independent-mark interpretation: the [Brownian motions](../../../brownian-motion.md) attached to the atoms are [independent](../../../random-variable.md#independent-random-variables) of one another and of the initial [Poisson random measure](../../../probability-theory.md#poisson-random-measure). Fix $t$ and define

$$
p_t(x)=\mathbb P\bigl(\exists s\in[0,t]:|x+\xi(s)-f(s)|\leq1\bigr).
$$

Conditionally on the initial atoms, each atom is retained as a dangerous atom if its own path meets the target by time $t$. These tests are [independent](../../../random-variable.md#independent-random-variables), with position-dependent retention [probability](../../../probability-theory.md#probability) $p_t(x)$. The permitted [Poisson thinning](../../../probability-theory.md#poisson-thinning) property makes the dangerous atoms a [Poisson random measure](../../../probability-theory.md#poisson-random-measure) of intensity $p_t(x)\,dx$.

Its total intensity is computed without invoking a marking or displacement theorem. The event in the definition of $p_t(x)$ says that $x$ belongs to

$$
W_-(t)=\bigcup_{0\leq s\leq t}\mathcal B(f(s)-\xi(s),1).
$$

By the [Tonelli theorem](../../../measure-theory.md#tonelli-theorem),

$$
\int_{\mathbb R^d}p_t(x)\,dx=\mathbb E\int_{\mathbb R^d}\mathbf1_{\{x\in W_-(t)\}}\,dx=\mathbb E\operatorname{vol}(W_-(t)).
$$

Symmetry of [Brownian motion](../../../brownian-motion.md) gives $-\xi\stackrel d=\xi$ as processes. It therefore identifies the last [expectation](../../../probability-theory.md#expected-value) with $\mathbb E\operatorname{vol}(W(t))$, where the sign of the deterministic path $f$ is unchanged. This swept set is a [Wiener sausage](../../../brownian-motion.md#wiener-sausage) with an added deterministic path.

The total intensity is finite on each bounded time interval. To see this explicitly, write $K_t=1+\sup_{s\leq t}|f(s)|$ and $R_t=\sup_{s\leq t}|\xi(s)|$. The sausage is contained in a ball of radius $K_t+R_t$. On a finite time grid, splitting according to the first crossing of a positive level $u$ by a one-dimensional [Brownian motion](../../../brownian-motion.md) shows that the chance of ending above $u$, conditional on the crossing, is at least $1/2$: the remaining [independent](../../../random-variable.md#independent-random-variables) increment is symmetric. Thus the grid maximum exceeds $u$ with [probability](../../../probability-theory.md#probability) at most twice the final Gaussian upper tail. Dense grids and continuity give the same bound for the path maximum. Applying this to each coordinate and its negative gives

$$
\mathbb P(R_t>u)\leq4d\,\mathbb P(N(0,t)>u/\sqrt d)\leq4d\,e^{-u^2/(2dt)}\qquad(t>0).
$$

The last inequality follows from $\mathbb E e^{\theta N(0,t)}=e^{\theta^2t/2}$ and minimizing the exponential Markov bound. Integration of this tail gives finite moments of $R_t$ of every positive order, so $\mathbb E\operatorname{vol}(W(t))<\infty$.

There are consequently only finitely many dangerous atoms on each compact time interval, almost surely. For closed balls, continuity of the paths makes each finite hitting-time infimum attained. The event $T>t$ is therefore the absence of dangerous atoms up to time $t$.

The open-ball convention has the same survival [probability](../../../probability-theory.md#probability) at each fixed $t$. Indeed for any compact path range $K$, the difference between its closed and open radius-one neighborhoods is the shell $\{x:\operatorname{dist}(x,K)=1\}$, which has zero [Lebesgue measure](../../../measure-theory.md#lebesgue-measure). To see this, choose a nearest $y\in K$ for a shell point $x$. For every sufficiently small $\varepsilon>0$, the ball of radius $\varepsilon/2$ centered at $x-\varepsilon(x-y)$ lies in the open neighborhood and inside the ball of radius $3\varepsilon/2$ about $x$. Thus the shell has a fixed proportional hole at every scale; the [Lebesgue density theorem](../../../measure-theory.md#lebesgue-s-density-theorem) forces its measure to be zero. By the [Tonelli theorem](../../../measure-theory.md#tonelli-theorem), closed-touch and open-entry retention probabilities have equal integrals. Independent thinning therefore gives no atom that touches only the boundary before this fixed horizon, almost surely. This also excludes a difference at an open-entry infimum equal to $t$.

 The zero-count [probability](../../../probability-theory.md#probability) of a [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) is $e^{-\lambda}$, and hence

$$
\boxed{\mathbb P(T>t)=\exp\{-\mathbb E\operatorname{vol}(W(t))\}.}
$$

This [survival among independently moving Poisson traps](../../../brownian-motion.md#survival-among-independently-moving-poisson-traps) formula has been derived using only [independent](../../../random-variable.md#independent-random-variables) thinning and the defining Poisson zero-count [probability](../../../probability-theory.md#probability), with the [expectation](../../../probability-theory.md#expected-value)/volume step supplied by Tonelli's theorem.

## 4

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For a nonnegative [submartingale](../../../martingale.md#submartingale) $(M_k)_{0\leq k\leq n}$ and $M_n^*=\max_{0\leq k\leq n}M_k$, the weak form of the [Doob maximal inequality](../../../martingale.md#doob-maximal-inequality-for-a-nonnegative-submartingale) is

$$
\boxed{u\,\mathbb P(M_n^*\geq u)\leq\mathbb E[M_n\mathbf1_{\{M_n^*\geq u\}}]\leq\mathbb E M_n\qquad(u>0).}
$$

To prove it, let $A_k$ be the event that $k$ is the first index with $M_k\geq u$. These events are disjoint, $A_k\in\mathcal F_k$, and their union is $A=\{M_n^*\geq u\}$. The [submartingale](../../../martingale.md#submartingale) property gives $\mathbb E[M_n\mid\mathcal F_k]\geq M_k$. Multiplying by $\mathbf1_{A_k}$, taking expectations and summing yields $\mathbb E[M_n\mathbf1_A]\geq\sum_k\mathbb E[M_k\mathbf1_{A_k}]\geq u\mathbb P(A)$. Nonnegativity gives the second inequality.

The associated [Doob Lp maximal inequality](../../../martingale.md#doob-lp-maximal-inequality), for $p>1$ and $M_n\in L^p$, is

$$
\boxed{\|M_n^*\|_p\leq\frac p{p-1}\|M_n\|_p.}
$$

Indeed $M_k\leq\mathbb E[M_n\mid\mathcal F_k]$, so conditional [Jensen inequality](../../../real-analysis.md#jensen-s-inequality) first ensures finite $p$th moments for all $M_k$ and hence for the finite maximum. Integrating the weak inequality against $pu^{p-2}\,du$ and using the [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) gives

$$
\mathbb E(M_n^*)^p\leq\frac p{p-1}\mathbb E[M_n(M_n^*)^{p-1}]
\leq\frac p{p-1}\|M_n\|_p\|M_n^*\|_p^{p-1}.
$$

The last step is [Holder inequality](../../../functional-analysis.md#holder-inequality). Dividing, unless the maximum is zero, proves the stated norm bound. For an arbitrary [martingale](../../../martingale.md), its absolute value is a nonnegative [submartingale](../../../martingale.md#submartingale) by conditional [Jensen inequality](../../../real-analysis.md#jensen-s-inequality), so both corresponding absolute-maximum bounds follow.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The [moment-generating function of a normal distribution](../../../probability-theory.md#moment-generating-function-of-a-normal-distribution) gives

$$
\mathbb E e^{\lambda X_1}=\exp\left(-\lambda+\frac{\lambda^2}{2}\right).
$$

Independence of $X_{n+1}$ from $\mathcal F_n$ implies

$$
\mathbb E[e^{\lambda S_{n+1}}\mid\mathcal F_n]=e^{\lambda S_n}\exp\left(-\lambda+\frac{\lambda^2}{2}\right).
$$

Every exponential here is integrable. Thus the process is a [martingale](../../../martingale.md) exactly when $-\lambda+\lambda^2/2=0$. Its two roots are $0$ and $2$, and the unique positive root is

$$
\boxed{\lambda=2.}
$$

The resulting [exponential martingale of a random walk](../../../markov-process.md#exponential-martingale-of-a-random-walk) is nonnegative and has [expectation](../../../probability-theory.md#expected-value) $1$ at every finite time.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The [strong law of large numbers](../../../convergence-of-random-variables.md#strong-law-of-large-numbers) gives $S_n/n\to-1$ almost surely, so $S_n\to-\infty$. Therefore the infinite-horizon maximum $Z$ is finite and attained almost surely; also $Z\geq0$ because $S_0=0$.

Apply the [Doob maximal inequality](../../../martingale.md#doob-maximal-inequality-for-a-nonnegative-submartingale) to $M_k=e^{2S_k}$ through time $n$. Since $\mathbb E M_n=1$,

$$
\mathbb P\left(\max_{0\leq k\leq n}S_k>t\right)\leq e^{-2t}\qquad(t\geq0).
$$

These finite-horizon events increase to $\{Z>t\}$. Continuity of [probability](../../../probability-theory.md#probability) under increasing unions gives

$$
\boxed{\mathbb P(Z>t)\leq e^{-2t}=e^{-\lambda t}.}
$$

For $t<0$ the same bound is trivial, because its right side exceeds $1$. Only bounded-horizon maximal inequalities were used before passing to the limit; no unjustified stopping at an infinite-horizon crossing time is needed.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

For $0<b<\lambda=2$, integrate the identity $e^{bz}-1=\int_0^z be^{bt}\,dt$ for $z\geq0$. The [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) and the tail bound in (c) give

$$
\mathbb E e^{bZ}=1+b\int_0^\infty e^{bt}\mathbb P(Z>t)\,dt
\leq1+b\int_0^\infty e^{-(2-b)t}\,dt=\frac2{2-b}.
$$

For $b=0$ the [expectation](../../../probability-theory.md#expected-value) is $1$, and for $b<0$ the fact $Z\geq0$ gives $0<e^{bZ}\leq1$. Therefore

$$
\boxed{\mathbb E e^{bZ}<\infty\quad\text{for every }b<2.}
$$

This is an [exponential moment bound for a Gaussian random-walk maximum](../../../markov-process.md#exponential-moment-bound-for-a-gaussian-random-walk-maximum). The upper-tail bound proves the requested sufficient range; it alone does not establish a converse at the endpoint.

## 5

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Put $\tau=T_r\wedge T_R$. First establish almost sure finiteness. The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives the [martingale](../../../martingale.md) $|B_t|^2-2t$ for planar [Brownian motion](../../../brownian-motion.md). Stop it at $t\wedge T_R$. The stopped path has norm at most $R$, so

$$
2\mathbb E(t\wedge T_R)=\mathbb E|B_{t\wedge T_R}|^2-|x|^2\leq R^2-|x|^2.
$$

By [monotone convergence](../../../measure-theory.md#monotone-convergence-theorem), $\mathbb E T_R<\infty$, and hence $\tau<\infty$ almost surely.

The function $h(y)=\log|y|$ is a [harmonic function](../../../partial-differential-equation.md#harmonic-function) away from $0$: in polar coordinates its [Laplacian](../../../calculus.md#laplacian) is $h''(\rho)+h'(\rho)/\rho=-\rho^{-2}+\rho^{-2}=0$. The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) shows $h(B_{t\wedge\tau})$ is a [local martingale](../../../martingale.md#local-martingale). It is bounded between $\log r$ and $\log R$, so it is a true [martingale](../../../martingale.md) and passage to $\tau$ is justified by [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem). Writing $p=\mathbb P_x(T_r<T_R)$ and using continuity at exit gives

$$
\log|x|=\mathbb E_x\log|B_\tau|=p\log r+(1-p)\log R.
$$

Solving yields the [planar Brownian annulus hitting probability](../../../brownian-motion.md#planar-brownian-annulus-hitting-probability)

$$
\boxed{\mathbb P_x(T_r<T_R)=\frac{\log R-\log|x|}{\log R-\log r}.}
$$

The stopping argument stays away from the singularity of the logarithm until the calculation is complete.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

First fix a deterministic point $y$ different from the initial point. By translation, work with $y=0$ and $B_0=x\ne0$. For $R>|x|$, hitting $0$ before $T_R$ requires hitting every circle of radius $r\in(0,|x|)$ before $T_R$. Part (a) gives

$$
\mathbb P_x(T_0<T_R)\leq\frac{\log R-\log|x|}{\log R-\log r}\longrightarrow0\qquad(r\downarrow0).
$$

Any finite-time hit of $0$ lies before exit from some sufficiently large integer-radius circle, since a continuous path on a finite interval is bounded. A countable union over such radii therefore shows that this fixed point is never hit. This is the [polar point for planar Brownian motion](../../../brownian-motion.md#polar-point-for-planar-brownian-motion) property; it is a statement about each fixed point, not about avoiding all points simultaneously.

For the initial point $x$, fix a deterministic $\varepsilon>0$. The [Gaussian distribution](../../../probability-theory.md#normal-distribution) of $B_\varepsilon$ has a density, so $B_\varepsilon\ne x$ almost surely. Conditional on $\mathcal F_\varepsilon$, the future is [Brownian motion](../../../brownian-motion.md) starting from $B_\varepsilon$, and the preceding fixed-point result shows that it never hits $x$. Taking $\varepsilon=1/m$ and a countable union proves **there is no return to the starting point at any positive time**.

In contrast, neighborhoods are revisited arbitrarily late. Choose $r>0$ so that the closed disk centered at $x$ of radius $r$ lies in the given open set $U$. From any point $z$ outside this disk, let $R\to\infty$ in part (a), centered at $x$. It gives

$$
\mathbb P_z(T_r<\infty)\geq\lim_{R\to\infty}\frac{\log R-\log|z-x|}{\log R-\log r}=1.
$$

At each deterministic integer time $n$, condition on $B_n$. If it is in the disk there is already a visit to $U$ at time $n$; if it is outside, the [Markov property](../../../markov-process.md#markov-property) and the last calculation ensure a later visit to that disk, hence to $U$. With [probability](../../../probability-theory.md#probability) one this holds for all $n$ simultaneously. Thus **the set of visits to $U$ is unbounded**. The [recurrence of planar Brownian motion](../../../brownian-motion.md#recurrence-of-planar-brownian-motion) concerns neighborhoods even though every fixed point is polar.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Let $L$ be the fixed line and choose $y\in L$. Take orthonormal vectors $e_1,e_2$ spanning the plane perpendicular to $L$. The process

$$
Y_t=\bigl(e_1\cdot(B_t-y),e_2\cdot(B_t-y)\bigr)
$$

is standard planar [Brownian motion](../../../brownian-motion.md) starting from $Y_0\ne0$. Indeed the projected increments are centered [Gaussian random vectors](../../../probability-and-statistics.md#gaussian-random-vector) with covariance $(t-s)I_2$, are [independent](../../../random-variable.md#independent-random-variables) on disjoint intervals, and have continuous paths.

The event $B_t\in L$ is exactly $Y_t=0$. The [polar point for planar Brownian motion](../../../brownian-motion.md#polar-point-for-planar-brownian-motion) result in (b) therefore gives

$$
\boxed{\mathbb P_x(\exists t\geq0:B_t\in L)=0\qquad(x\notin L).}
$$

This is a [projection criterion for Brownian avoidance of affine subspaces](../../../brownian-motion.md#projection-criterion-for-brownian-avoidance-of-affine-subspaces): avoiding a fixed point in a two-dimensional projection excludes hitting the original line.

## 6

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Let $M_t=\max_{0\leq s\leq t}B_s$. The [Brownian reflection principle](../../../brownian-motion.md#reflection-principle-wiener-process) gives

$$
\mathbb P(M_t>1)=2\mathbb P(B_t>1).
$$

Here is the reflection argument: on paths that hit $1$ before $t$, reflect all increments after their first hitting time. The [Strong Markov property](../../../markov-process.md#strong-markov-property) gives [independent](../../../random-variable.md#independent-random-variables) [Brownian motion](../../../brownian-motion.md) after that time, whose sign can be reversed without changing its law. This exchanges paths ending below $1$ with paths ending above $1$. The latter have necessarily hit $1$, and the endpoint has no atom at $1$, giving the displayed equality. It also shows that $M_t$ has a continuous distribution at every positive level.

Writing $\Phi$ for the [standard normal distribution function](../../../probability-theory.md#standard-normal-distribution-function), the [probability](../../../probability-theory.md#probability) of staying below the barrier is therefore

$$
\mathbb P(B_s\leq1\text{ for all }s\leq t)=2\Phi(t^{-1/2})-1.
$$

Since $\Phi(h)-\Phi(0)\sim h/\sqrt{2\pi}$ as $h\downarrow0$, the [Brownian barrier survival asymptotic](../../../brownian-motion.md#brownian-barrier-survival-asymptotic) is

$$
\boxed{\alpha=\tfrac12,\qquad \lim_{t\to\infty}\sqrt t\,\mathbb P(B_s\leq1\text{ for all }s\leq t)=\sqrt{\frac2\pi}.}
$$

Any smaller exponent gives a zero limit and any larger exponent gives an infinite limit, so this is the unique exponent producing a finite positive constant.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Let $X_i$ be [independent and identically distributed random variables](../../../random-variable.md#independent-and-identically-distributed-random-variables) with mean $0$ and [variance](../../../variance.md) $\sigma^2\in(0,\infty)$, and put $S_0=0$, $S_k=\sum_{i=1}^kX_i$. Define the polygonal interpolation

$$
W_n(s)=\frac{S_{\lfloor ns\rfloor}+(ns-\lfloor ns\rfloor)X_{\lfloor ns\rfloor+1}}{\sigma\sqrt n}\qquad(0\leq s\leq1),
$$

with the endpoint $W_n(1)=S_n/(\sigma\sqrt n)$. The [Donsker invariance principle](../../../convergence-of-random-variables.md#donsker-s-theorem) states

$$
\boxed{W_n\ \Rightarrow\ B\quad\text{in }C([0,1])\text{ with the uniform topology},}
$$

where $B$ is standard one-dimensional [Brownian motion](../../../brownian-motion.md) and the arrow denotes [weak convergence of probability measures](../../../convergence-of-random-variables.md#weak-convergence-of-probability-measures) on this path space. Equivalently, the step interpolation converges in the [Skorokhod space](../../../functional-analysis.md#skorokhod-space) with its $J_1$ topology. The continuous interpolation version is sufficient for the maximum in part (c).

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

For the [simple symmetric random walk](../../../probability-theory.md#simple-symmetric-random-walk), the increments have mean $0$ and [variance](../../../variance.md) $1$. Use the polygonal interpolation from (b). The maximum functional is Lipschitz in the [supremum norm](../../../functional-analysis.md#supremum-norm), since

$$
\left|\max_{0\leq s\leq1}g(s)-\max_{0\leq s\leq1}h(s)\right|\leq\|g-h\|_\infty.
$$

Each interpolating segment is linear, so its maximum occurs at a grid endpoint. The [continuous mapping theorem](../../../convergence-of-random-variables.md#continuous-mapping-theorem) applied to the [Donsker invariance principle](../../../convergence-of-random-variables.md#donsker-s-theorem) gives

$$
\frac1{\sqrt n}\max_{0\leq j\leq n}S_j\ \Rightarrow\ \max_{0\leq s\leq1}B_s.
$$

The limiting maximum has no atom at $a>0$ by the [Brownian reflection principle](../../../brownian-motion.md#reflection-principle-wiener-process), so the closed-tail [probabilities](../../../probability-theory.md#probability) converge at this threshold. Including $j=0$ does not change the event because $a>0$. Therefore the [random-walk maximum limit from Donsker invariance](../../../convergence-of-random-variables.md#random-walk-maximum-limit-from-donsker-invariance) is

$$
\boxed{\lim_{n\to\infty}\mathbb P\left(\max_{j\leq n}S_j\geq a\sqrt n\right)=2\bigl(1-\Phi(a)\bigr),\qquad a>0.}
$$

Here $\Phi$ is the [standard normal distribution function](../../../probability-theory.md#standard-normal-distribution-function). The normalization and the positive-threshold condition are those in the PDF; the TeX aid's $\sqrt t$ is not the printed expression.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
