# Paper 79

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper79.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper79.pdf)

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
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 79](paper-79.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

At [large-deviation speed](../../../convergence-of-random-variables.md#large-deviation-speed) $L$, the [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) gives the [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle) on $\mathbb R$ with [good rate function](../../../convergence-of-random-variables.md#good-rate-function)

$$
\boxed{J(b)=\begin{cases}\lambda b,&b\geq0,\\+\infty,&b<0.\end{cases}}
$$

In particular, $\mathbb P(B/L\geq b)=e^{-\lambda Lb}$ for $b\geq0$. Its finite [sublevel sets](../../../calculus.md#sublevel-set) are the [compact sets](../../../topology.md#compact-space) $[0,r/\lambda]$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Write $S_L=\sum_{i=1}^LA_i$ and $Z_L=S_L/L$. The [cumulant-generating function](../../../probability-theory.md#cumulant-generating-function) of one [normal random variable](../../../probability-theory.md#gaussian-random-variable) is

$$
\kappa(\theta)=\log\mathbb E e^{\theta A_1}=\mu\theta+\frac{\sigma^2\theta^2}{2},\qquad \theta\in\mathbb R.
$$

[Cramér's theorem](../../../probability-theory.md#cramer-s-theorem) states that empirical means of [independent and identically distributed random variables](../../../random-variable.md#independent-and-identically-distributed-random-variables) whose [moment-generating function](../../../probability-theory.md#moment-generating-function) is finite on a neighborhood of zero satisfy a [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle) at the sample-size [large-deviation speed](../../../convergence-of-random-variables.md#large-deviation-speed), with [good rate function](../../../convergence-of-random-variables.md#good-rate-function) equal to the [Legendre-Fenchel transform](../../../convex-optimization.md#convex-conjugate) of their [cumulant-generating function](../../../probability-theory.md#cumulant-generating-function). Here that gives

$$
I(x)=\sup_{\theta\in\mathbb R}\left\{\theta(x-\mu)-\frac{\sigma^2\theta^2}{2}\right\}.
$$

For $\sigma^2>0$, differentiation gives the maximizing parameter $\theta=(x-\mu)/\sigma^2$, and hence

$$
\boxed{I(x)=\frac{(x-\mu)^2}{2\sigma^2}.}
$$

This [rate function](../../../convergence-of-random-variables.md#rate-function) tends to infinity as $|x|\to\infty$, so its finite [sublevel sets](../../../calculus.md#sublevel-set) are [compact](../../../topology.md#compact-space). Equivalently, the [Gärtner–Ellis theorem](../../../convergence-of-random-variables.md#gartner-ellis-theorem) applies because the limiting scaled [cumulant-generating function](../../../probability-theory.md#cumulant-generating-function) is finite and differentiable everywhere; it is [lower semicontinuous](../../../calculus.md#lower-semicontinuity) and [essentially smooth](../../../real-analysis.md#essential-smoothness-of-a-convex-function), with no finite domain boundary at which to check steepness. If $\sigma^2=0$ is permitted, $Z_L=\mu$ deterministically and the [rate function](../../../convergence-of-random-variables.md#rate-function) is zero at $\mu$ and infinity elsewhere.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The [product large-deviation principle](../../../convergence-of-random-variables.md#product-large-deviation-principle) states that independent families satisfying [large deviation principles](../../../convergence-of-random-variables.md#large-deviation-principle) at the same speed with [good rate functions](../../../convergence-of-random-variables.md#good-rate-function) $J$ and $I$ have joint [good rate function](../../../convergence-of-random-variables.md#good-rate-function) $J(b)+I(z)$. The [contraction principle for large deviations](../../../convergence-of-random-variables.md#contraction-principle-for-large-deviations) states that a [continuous map](../../../topology.md#continuous-map) $f$ sends such a principle to one with [good rate function](../../../convergence-of-random-variables.md#good-rate-function) $\inf_{f(u)=x}I(u)$. Apply these results to $(B/L,S_L/L)$ and addition. The resulting [infimal convolution](../../../convex-optimization.md#infimal-convolution) is

$$
K(x)=\inf_{b\geq0}\left\{\lambda b+\frac{(x-b-\mu)^2}{2\sigma^2}\right\}.
$$

For $\sigma^2>0$, the unconstrained stationary point is $b=x-\mu-\lambda\sigma^2$. [Convexity](../../../real-analysis.md#convex-function) gives the constrained minimum at $b_*=(x-\mu-\lambda\sigma^2)^+$, so

$$
\boxed{K(x)=\begin{cases}\dfrac{(x-\mu)^2}{2\sigma^2},&x\leq\mu+\lambda\sigma^2,\\\lambda(x-\mu)-\dfrac{\lambda^2\sigma^2}{2},&x\geq\mu+\lambda\sigma^2.\end{cases}}
$$

The two branches agree in value and first derivative at their junction. Both tails tend to infinity, giving a [good rate function](../../../convergence-of-random-variables.md#good-rate-function). This is the [fixed exponential perturbation of a Gaussian empirical mean](../../../convergence-of-random-variables.md#fixed-exponential-perturbation-of-a-gaussian-empirical-mean).

There is a reason to use the [product large-deviation principle](../../../convergence-of-random-variables.md#product-large-deviation-principle) rather than invoke the supplied [Gärtner–Ellis theorem](../../../convergence-of-random-variables.md#gartner-ellis-theorem) without checking its hypotheses. The limiting scaled [cumulant-generating function](../../../probability-theory.md#cumulant-generating-function) here is

$$
\Lambda(\theta)=\begin{cases}\mu\theta+\sigma^2\theta^2/2,&\theta<\lambda,\\+\infty,&\theta\geq\lambda.\end{cases}
$$

At $\lambda$ it is neither [lower semicontinuous](../../../calculus.md#lower-semicontinuity) nor steep from the left: its left derivative tends to the finite value $\mu+\lambda\sigma^2$. Its [Legendre-Fenchel transform](../../../convex-optimization.md#convex-conjugate) still equals $K$, but the stated [Gärtner–Ellis theorem](../../../convergence-of-random-variables.md#gartner-ellis-theorem) does not establish the full lower bound on the linear branch. The [product large-deviation principle](../../../convergence-of-random-variables.md#product-large-deviation-principle) and [contraction principle for large deviations](../../../convergence-of-random-variables.md#contraction-principle-for-large-deviations) do establish it. In the degenerate case $\sigma^2=0$, the answer is $K(x)=\lambda(x-\mu)$ for $x\geq\mu$, and infinity otherwise.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The sum still has a [normal distribution](../../../probability-theory.md#normal-distribution), now with

$$
\mathbb E\frac{C+S_L}{L}=\mu+\frac{\nu}{L},\qquad
\operatorname{Var}\frac{C+S_L}{L}=\frac{\sigma^2}{L}+\frac{\rho^2}{L^2}.
$$

Its scaled [cumulant-generating function](../../../probability-theory.md#cumulant-generating-function) is

$$
\frac1L\log\mathbb E e^{\theta(C+S_L)}
=\mu\theta+\frac{\sigma^2\theta^2}{2}+\frac{\nu\theta+\rho^2\theta^2/2}{L}.
$$

The limit is the same everywhere-finite function as in part (b), so the [Gärtner–Ellis theorem](../../../convergence-of-random-variables.md#gartner-ellis-theorem) gives

$$
\boxed{I_C(x)=\frac{(x-\mu)^2}{2\sigma^2}}
$$

at [large-deviation speed](../../../convergence-of-random-variables.md#large-deviation-speed) $L$, when $\sigma^2>0$.

One can also see exactly why $C$ has no effect through [exponential equivalence](../../../convergence-of-random-variables.md#exponential-equivalence). For every $\varepsilon>0$, the [Chernoff bound](../../../probability-inequality.md#chernoff-bound) for the two [Gaussian tail bounds](../../../probability-and-statistics.md#gaussian-tail-bound) gives, when $L\varepsilon>|\nu|$ and $\rho^2>0$,

$$
\mathbb P(|C|>L\varepsilon)\leq2\exp\left(-\frac{(L\varepsilon-|\nu|)^2}{2\rho^2}\right).
$$

Its logarithm divided by $L$ tends to $-\infty$. If $\rho^2=0$, this probability is eventually zero. The transfer result for [exponential equivalence](../../../convergence-of-random-variables.md#exponential-equivalence) says that coupled families whose distance exceeds each fixed positive tolerance with superexponentially small probability share a [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle) with the same [good rate function](../../../convergence-of-random-variables.md#good-rate-function). Apply it to $(C+S_L)/L$ and $S_L/L$. This also covers $\sigma^2=0$, with the point-mass [rate function](../../../convergence-of-random-variables.md#rate-function) from part (b).

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

All three normalized sums converge in probability to $\mu$: the [weak law of large numbers](../../../convergence-of-random-variables.md#weak-law-of-large-numbers) controls $S_L/L$, and the two fixed [random variables](../../../random-variable.md) vanish after division by $L$. Their rare fluctuations nevertheless differ. A fixed [normal random variable](../../../probability-theory.md#gaussian-random-variable) would have to fluctuate by order $L$ to alter the mean by a fixed amount, and that costs $\exp(-\text{constant}\,L^2)$. A fixed [exponential random variable](../../../continuous-probability-distribution.md#exponential-distribution) can do the same for a cost of order $\exp(-\text{constant}\,L)$, exactly the [large-deviation speed](../../../convergence-of-random-variables.md#large-deviation-speed) of the empirical mean.

Below $\mu+\lambda\sigma^2$, the optimal exponential contribution is zero, and the [Gaussian](../../../probability-theory.md#normal-distribution) empirical mean supplies the fluctuation. Above it, the optimal empirical mean remains at $\mu+\lambda\sigma^2$, while $B/L$ supplies $x-\mu-\lambda\sigma^2$. This explains the quadratic-to-linear change in the [rate function](../../../convergence-of-random-variables.md#rate-function) and why only the upper tail is altered. **Convergence to the same typical value does not imply the same large-deviation behavior.**

## 2

↑ **Parent:** [Paper 79](paper-79.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Work in a [Hausdorff space](../../../topology.md#hausdorff-space) $E$, for example a [metric space](../../../topological-analysis.md#metric-space). A [rate function](../../../convergence-of-random-variables.md#rate-function) is a [lower semicontinuous](../../../calculus.md#lower-semicontinuity) map $I:E\to[0,\infty]$. A [good rate function](../../../convergence-of-random-variables.md#good-rate-function) additionally has [compact](../../../topology.md#compact-space) finite [sublevel sets](../../../calculus.md#sublevel-set) $\{x:I(x)\leq r\}$.

A [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle) at [large-deviation speed](../../../convergence-of-random-variables.md#large-deviation-speed) $L$ requires, for every [open set](../../../topology.md#open-set) $G$ and [closed set](../../../topology.md#closed-set) $F$,

$$
-\inf_{x\in G}I(x)\leq\liminf_{L\to\infty}\frac1L\log\mathbb P(X_L\in G),\qquad
\limsup_{L\to\infty}\frac1L\log\mathbb P(X_L\in F)\leq-\inf_{x\in F}I(x).
$$

The conventions are $\log0=-\infty$ and $\inf\varnothing=+\infty$. A [weak large deviation principle](../../../convergence-of-random-variables.md#weak-large-deviation-principle) imposes the same lower bound but only the upper bound for [compact sets](../../../topology.md#compact-space). [Exponential tightness](../../../convergence-of-random-variables.md#exponential-tightness) supplies [compact sets](../../../topology.md#compact-space) $K_M$ with $\limsup L^{-1}\log\mathbb P(X_L\notin K_M)<-M$ for every $M\geq0$. The strict inequality can equivalently be obtained from the common non-strict definition by choosing a larger containment level.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Fix a finite $r\geq0$ and choose $M>r$. By [exponential tightness](../../../convergence-of-random-variables.md#exponential-tightness), choose a [compact set](../../../topology.md#compact-space) $K_M$ with outside probability having upper exponential rate strictly below $-M$. A [compact set](../../../topology.md#compact-space) in a [Hausdorff space](../../../topology.md#hausdorff-space) is closed, so its complement is an [open set](../../../topology.md#open-set). The lower bound of the [weak large deviation principle](../../../convergence-of-random-variables.md#weak-large-deviation-principle) gives

$$
-\inf_{x\notin K_M}I(x)
\leq\liminf_L\frac1L\log\mathbb P(X_L\notin K_M)
\leq\limsup_L\frac1L\log\mathbb P(X_L\notin K_M)<-M.
$$

Consequently $\inf_{K_M^c}I>M$, and $\{I\leq r\}\subset K_M$. [Lower semicontinuity](../../../calculus.md#lower-semicontinuity) makes this [sublevel set](../../../calculus.md#sublevel-set) closed in $E$, hence a closed subset of a [compact set](../../../topology.md#compact-space). Thus it is [compact](../../../topology.md#compact-space). **Every finite sublevel set is compact, so $I$ is a good rate function.**

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $F$ be any [closed set](../../../topology.md#closed-set). For each $M>0$, choose $K_M$ as above. The probability decomposition

$$
\mathbb P(X_L\in F)\leq\mathbb P(X_L\in F\cap K_M)+\mathbb P(X_L\notin K_M)
$$

reduces the first term to a [compact set](../../../topology.md#compact-space), where the weak upper bound applies. For nonnegative numbers $u_L,v_L$, the inequality $u_L+v_L\leq2\max(u_L,v_L)$ shows that the upper exponential rate of their sum is no larger than the maximum of their upper exponential rates. Hence

$$
\limsup_L\frac1L\log\mathbb P(X_L\in F)
\leq\max\left\{-\inf_{F\cap K_M}I,-M\right\}
\leq\max\left\{-\inf_F I,-M\right\}.
$$

Let $M\to\infty$. This proves the full closed-set upper bound, including when $\inf_F I=+\infty$. The open-set lower bound was already assumed. Combining with part (b), **the weak principle upgrades to a large deviation principle with good rate function $I$**. This is [exponential tightness upgrades a weak large deviation principle](../../../convergence-of-random-variables.md#exponential-tightness-upgrades-a-weak-large-deviation-principle).

## 3

↑ **Parent:** [Paper 79](paper-79.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Measure $Q_t$ immediately after service in slot $(t-1,t)$, and let $a_t\geq0$ denote work eligible for that slot's service. Writing $x^+=\max(x,0)$, the [Lindley recursion](../../../queueing-theory.md#lindley-recursion) is

$$
\boxed{Q_t=(Q_{t-1}+a_t-c)^+.}
$$

Start with an empty [queue](../../../queueing-theory.md#queue-queueing-theory) at time $-N$. Repeated substitution gives its time-zero [queue workload](../../../queueing-theory.md#workload-of-a-queue)

$$
Q_0^{(N)}(a,c)=\max_{0\leq n\leq N}\left\{\sum_{j=0}^{n-1}a_{-j}-cn\right\},
$$

where the empty sum is zero. The increasing limit defines the minimal causal [queue workload](../../../queueing-theory.md#workload-of-a-queue):

$$
\boxed{Q_0(a,c)=\sup_{n\geq0}\{A_n(a)-cn\},\qquad A_n(a)=\sum_{j=0}^{n-1}a_{-j},\quad A_0=0.}
$$

If the mean of the remote past is $\lambda<c$, then $A_n(a)/n\to\lambda$, so $A_n(a)-cn\to-\infty$. The [supremum](../../../real-analysis.md#supremum) is then finite and is attained at a finite window. The same formula with indices shifted gives $Q_t(a,c)$ and satisfies the [Lindley recursion](../../../queueing-theory.md#lindley-recursion) directly: split the supremum into the zero-window term and all positive-window terms.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

There is an indexing issue in the printed topology. Its cumulative sums omit $a_0$, whereas the post-slot [workload of a queue](../../../queueing-theory.md#workload-of-a-queue) in part (a) includes $a_0$. To see the problem, take all $a_t=\lambda$ for $t\leq-1$, with $\lambda<c$, and compare two inputs with $a_0=\lambda$ and $a_0=c+1$. Their distance according to the printed cumulative-sum expression is zero, yet

$$
Q_0(a,c)=0,\qquad Q_0(b,c)=1.
$$

Thus **the post-slot workload is not continuous in the literal printed topology**. On two-sided sequences that expression is a [seminorm](../../../topological-vector-space.md#seminorm), since it also ignores future coordinates; the fixed-mean input class is not a [vector space](../../../vector-space.md) (if signed inputs are allowed, it is an affine set).

The appropriate repair for the post-slot convention is to use one-sided past inputs including time zero and the [weighted cumulative-input topology for a slotted queue](../../../queueing-theory.md#weighted-cumulative-input-topology-for-a-slotted-queue):

$$
d_\#(a,b)=\sup_{n\geq1}\frac{|A_n(a)-A_n(b)|}{n+1}.
$$

This is a finite [metric](../../../topological-analysis.md#metric) on the fixed-mean class, since cumulative differences are $o(n)$; equality of all cumulative sums implies equality of all past coordinates. It is equivalent to augmenting the printed cumulative-difference distance by $|a_0-b_0|$: their cumulative sums differ only by this extra coordinate and a one-step shift.

Here is the full corrected [continuity](../../../calculus.md#continuous-function) proof. Fix $a$ with $A_n(a)/n\to\lambda<c$, and let $\varepsilon=(c-\lambda)/4$. Choose $N\geq1$ such that $A_n(a)/n\leq\lambda+\varepsilon$ whenever $n\geq N$. If $d_\#(a,b)<\varepsilon/2$, then, for all such $n$,

$$
A_n(b)-cn\leq n(\lambda+\varepsilon-c)+(n+1)d_\#(a,b)
\leq n(\lambda+2\varepsilon-c)<0.
$$

Both [queue workloads](../../../queueing-theory.md#workload-of-a-queue) therefore maximize over the same finite collection $0\leq n<N$, containing the value zero. For any two finite lists, the difference of their maxima is at most the maximum absolute difference of corresponding entries. Thus

$$
\boxed{|Q_0(a,c)-Q_0(b,c)|\leq(N+1)d_\#(a,b)}
$$

in this neighborhood. In particular the [queue workload](../../../queueing-theory.md#workload-of-a-queue) is locally [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity) and hence [continuous](../../../calculus.md#continuous-function).

An alternative indexing repair retains the printed topology but interprets the time-zero function as the workload before slot $(-1,0)$, namely $\sup_{n\geq0}\{\sum_{j=1}^na_{-j}-cn\}$. The same finite-window argument proves its [continuity](../../../calculus.md#continuous-function). One must then shift the time labels consistently in the later recursions. The remaining answers use the post-slot convention and $d_\#$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The work passed downstream in slot $(t-1,t)$ is

$$
D_t=\min\{c,Q_{t-1}+a_t\}=Q_{t-1}+a_t-Q_t.
$$

Because this work is eligible for downstream service in the same slot, the downstream [Lindley recursion](../../../queueing-theory.md#lindley-recursion) is

$$
\boxed{R_t=(R_{t-1}+D_t-d)^+.}
$$

Put $T_t=Q_t+R_t$. If $R_{t-1}+D_t\geq d$, then

$$
T_t=Q_{t-1}+R_{t-1}+a_t-d\geq0.
$$

If $R_{t-1}+D_t<d$, then $D_t<d<c$, so the upstream server did not use its full capacity. Consequently $D_t=Q_{t-1}+a_t$ and $Q_t=0$. Also $R_t=0$ and $Q_{t-1}+R_{t-1}+a_t-d<0$. Both cases yield

$$
\boxed{Q_t+R_t=(Q_{t-1}+R_{t-1}+a_t-d)^+.}
$$

This [slower-server tandem workload identity](../../../queueing-theory.md#slower-server-tandem-workload-identity) uses both $d<c$ and eligibility for same-slot downstream service. It would not describe a system with an obligatory one-slot transfer delay.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Define the downstream [queue workload](../../../queueing-theory.md#workload-of-a-queue) by starting both [queues](../../../queueing-theory.md#queue-queueing-theory) empty at time $-N$ and taking the increasing remote-past limit. For each finite $N$, part (c) makes their total [queue workload](../../../queueing-theory.md#workload-of-a-queue) exactly the single-server workload with service $d$, while the upstream [queue workload](../../../queueing-theory.md#workload-of-a-queue) is the single-server workload with service $c$. Therefore

$$
R_0^{(N)}(a,c,d)=Q_0^{(N)}(a,d)-Q_0^{(N)}(a,c).
$$

The downstream limit is increasing: the coupled upstream and downstream recursions are increasing in their initial state, because $D_t=\min(c,Q_{t-1}+a_t)$ is increasing in $Q_{t-1}$. With finite upstream [queue workload](../../../queueing-theory.md#workload-of-a-queue), taking the limit gives

$$
\boxed{R_0(a,c,d)=Q_0(a,d)-Q_0(a,c).}
$$

The result is nonnegative because reducing service cannot reduce [queue workload](../../../queueing-theory.md#workload-of-a-queue). It can be $+\infty$ when the slower server is unstable; under $\lambda<d<c$, both quantities are finite. The finite-upstream condition matters: subtracting two infinite [queue workloads](../../../queueing-theory.md#workload-of-a-queue) would not define a downstream queue.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

The indexing defect also affects the downstream claim. For the two inputs in part (b), now choose $\lambda<d<c$. The constant input has zero downstream [queue workload](../../../queueing-theory.md#workload-of-a-queue), while the input with $a_0=c+1$ has

$$
Q_0(b,d)=c+1-d,\qquad Q_0(b,c)=1,\qquad R_0(b,c,d)=c-d>0.
$$

Their printed distance is zero, so the literal post-slot downstream [continuity](../../../calculus.md#continuous-function) assertion is false as well.

In the corrected [weighted cumulative-input topology for a slotted queue](../../../queueing-theory.md#weighted-cumulative-input-topology-for-a-slotted-queue), apply the finite-window proof of part (b) separately with services $d$ and $c$. Both have strictly negative long-window drift because $\lambda<d<c$. There are a neighborhood of $a$ and finite constants $C_d,C_c$ such that

$$
|R_0(a,c,d)-R_0(b,c,d)|
\leq |Q_0(a,d)-Q_0(b,d)|+|Q_0(a,c)-Q_0(b,c)|
\leq(C_d+C_c)d_\#(a,b).
$$

This proves [continuity](../../../calculus.md#continuous-function), and indeed local [Lipschitz continuity](../../../real-analysis.md#lipschitz-continuity), for the intended downstream function.

Suppose a family of random arrival paths $a^{(L)}$ has a [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle) in this corrected input space, at speed $L$ with [good rate function](../../../convergence-of-random-variables.md#good-rate-function) $\mathcal I$. The [contraction principle for large deviations](../../../convergence-of-random-variables.md#contraction-principle-for-large-deviations) then gives the downstream [good rate function](../../../convergence-of-random-variables.md#good-rate-function)

$$
\boxed{J_R(r)=\inf\{\mathcal I(a):Q_0(a,d)-Q_0(a,c)=r\}.}
$$

It is infinity for $r<0$. The path [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle), its topology, and its subcritical domain must actually be established for the chosen stochastic model: a collection of finite-dimensional [large deviation principles](../../../convergence-of-random-variables.md#large-deviation-principle) alone does not control infinitely long workload windows. Nor should upstream departures be assumed [independent](../../../random-variable.md#independent-random-variables); the path contraction avoids that unjustified assumption.

## 4

↑ **Parent:** [Paper 79](paper-79.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Consider a stationary nonnegative work-input process in slotted time, with cumulative work $A_n$ over the last $n$ slots and a work-conserving server of capacity $c$ per slot. Assume its past average tends almost surely to $m<c$. The [Lindley recursion](../../../queueing-theory.md#lindley-recursion) then defines the finite stationary [queue workload](../../../queueing-theory.md#workload-of-a-queue)

$$
Q=\sup_{n\geq0}(A_n-cn).
$$

This is work remaining, rather than the number of customers when customer service requirements vary. With unit work per customer the two notions coincide. Stationarity makes the [distribution](../../../distribution-theory.md#distribution-mathematical-analysis) of a past cumulative window equal to that of a forward window of the same length.

For a parameter $\theta>0$ and a positive window length $n$, the [effective bandwidth](../../../queueing-theory.md#effective-bandwidth) is

$$
\boxed{\alpha(\theta,n)=\frac{1}{\theta n}\log\mathbb E e^{\theta A_n}.}
$$

It measures a traffic rate through exponential moments, so it retains information about rare bursts that the mean alone discards. If the limiting scaled [cumulant-generating function](../../../probability-theory.md#cumulant-generating-function) exists, put

$$
\kappa(\theta)=\lim_{n\to\infty}\frac1n\log\mathbb E e^{\theta A_n},\qquad
\alpha(\theta)=\frac{\kappa(\theta)}{\theta}.
$$

The finite-window [effective bandwidth](../../../queueing-theory.md#effective-bandwidth) matters when the relevant overflow window is short or when arrivals are correlated; one should not replace it by its long-window limit without justification.

The following proof gives an actual upper bound for the infinite-horizon [queue workload](../../../queueing-theory.md#workload-of-a-queue). For $B>0$, if $Q>B$, at least one positive integer $n$ has $A_n-cn>B$. The [union bound](../../../probability-inequality.md#boole-s-inequality) followed by the [Chernoff bound](../../../probability-inequality.md#chernoff-bound) gives

$$
\mathbb P(Q>B)\leq\sum_{n\geq1}\mathbb P(A_n>B+cn)
\leq e^{-\theta B}\sum_{n\geq1}\exp\{\theta n[\alpha(\theta,n)-c]\}.
$$

Assume each finite-window exponential moment is finite and $\kappa(\theta)<c\theta$. Choose $\eta>0$ such that $\kappa(\theta)+\eta<c\theta$. For all sufficiently large $n$, the summand is at most $e^{-n(c\theta-\kappa(\theta)-\eta)}$. Its tail is a convergent geometric series, and its finite prefix is finite. Denote the resulting sum by $K_\theta$. The [exponential workload bound from cumulative arrival moments](../../../queueing-theory.md#exponential-workload-bound-from-cumulative-arrival-moments) therefore proves, for $b>0$,

$$
\limsup_{L\to\infty}\frac1L\log\mathbb P(Q>Lb)\leq-\theta b.
$$

Optimizing over admissible parameters gives

$$
\boxed{\limsup_{L\to\infty}\frac1L\log\mathbb P(Q>Lb)\leq-b\theta_*,\qquad
\theta_* =\sup\{\theta>0:\kappa(\theta)<c\theta\}.}
$$

Only parameters with the stated finite-window moments are included. If there are no such positive parameters, the argument yields only the trivial exponent zero. Infinite $\theta_*$ means that the upper rate is $-\infty$. For a non-strict threshold $Q\geq Lb$, first bound it by $Q>L(b-\varepsilon)$ and then let $\varepsilon\downarrow0$. This proof permits dependence between slots. It proves the required upper bound; it does not assert a matching lower bound for every arrival process.

This also gives a closed-set large-deviation upper bound for $Q/L$: set $I_+(q)=\theta_*q$ for $q>0$, $I_+(0)=0$, and $I_+(q)=+\infty$ for $q<0$. If a [closed set](../../../topology.md#closed-set) $F$ contains zero, its desired upper bound is the trivial bound zero. If $F$ contains positive points but not zero, its positive part has a smallest point $b>0$, and $\mathbb P(Q/L\in F)\leq\mathbb P(Q\geq Lb)$ gives the bound $-\inf_F I_+$. If it contains no nonnegative points, its probability is zero. This verifies the upper half of a [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle); the actual [rate function](../../../convergence-of-random-variables.md#rate-function) can be larger when a matching lower bound is unavailable.

For [independent and identically distributed](../../../random-variable.md#independent-and-identically-distributed-random-variables) slot arrivals $a_t$, let $\kappa(\theta)=\log\mathbb E e^{\theta a_0}$. Now $\log\mathbb E e^{\theta A_n}=n\kappa(\theta)$, so [effective bandwidth](../../../queueing-theory.md#effective-bandwidth) is independent of window length. For $\kappa(\theta)<c\theta$, the geometric-series prefactor is explicitly

$$
K_\theta=\frac{e^{\kappa(\theta)-c\theta}}{1-e^{\kappa(\theta)-c\theta}}.
$$

Thus the familiar [workload Chernoff bound for independent increments](../../../queueing-theory.md#workload-chernoff-bound-for-independent-increments) is a special case, and the largest admissible parameter is often the positive root of $\kappa(\theta)=c\theta$.

For these independent increments there is a sharper argument that works at the root itself when its exponential moment is finite. Along the past read in reverse order, put $S_n=A_n-cn$ and $M_n=e^{\theta S_n}$. If $\mathbb E e^{\theta(a_0-c)}\leq1$, then $M_n$ is a nonnegative [supermartingale](../../../martingale.md#supermartingale) starting at one. For the first crossing time $\tau_B=\inf\{n\geq0:S_n\geq B\}$, bounded [optional stopping](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) gives

$$
1\geq\mathbb E M_{\tau_B\wedge N}\geq e^{\theta B}\mathbb P(\tau_B\leq N).
$$

Let $N\to\infty$. Strict negative drift makes $S_n\to-\infty$ almost surely, so its supremum is attained and the crossing event agrees with $\{Q\geq B\}$. Consequently

$$
\boxed{\mathbb P(Q\geq B)\leq e^{-\theta B}.}
$$

This strengthens the prefactor but uses temporal [independence](../../../random-variable.md#independent-random-variables), which was unnecessary for the previous proof.

Several examples show what the [effective bandwidth](../../../queueing-theory.md#effective-bandwidth) constraint means. Deterministic traffic of $r$ work units per slot has $\kappa(\theta)=\theta r$ and [effective bandwidth](../../../queueing-theory.md#effective-bandwidth) $r$ at every parameter; if $c\geq r$ there is no stationary backlog. For independent on-off slots carrying $r$ units with probability $p$ and zero otherwise, the [Bernoulli effective bandwidth](../../../queueing-theory.md#bernoulli-effective-bandwidth) is

$$
\alpha(\theta)=\frac{\log(1-p+pe^{\theta r})}{\theta}.
$$

For $0<p<1$, it rises from the mean $pr$ to the peak $r$. When $pr<c<r$, strict [convexity](../../../real-analysis.md#convex-function) of $\kappa(\theta)-c\theta$, its negative derivative at zero, and its divergence to infinity give a unique positive root. When $c\geq r$, no slot can increase the [queue workload](../../../queueing-theory.md#workload-of-a-queue). In the specific case $r=2,c=1,p<1/2$, the workload increases by one with probability $p$ and decreases by one, reflected at zero, with probability $1-p$. Its stationary probabilities satisfy

$$
\pi_{k+1}=\frac{p}{1-p}\pi_k,\qquad
\pi_k=(1-q)q^k,\quad q=\frac{p}{1-p}.
$$

The service-root equation has $e^{\theta_*}=(1-p)/p$, and thus $\mathbb P(Q\geq k)=q^k=e^{-\theta_* k}$. This example realizes the upper exponent exactly.

For independent [Poisson](../../../discrete-probability-distribution.md#poisson-distribution) slot counts of mean $\nu$, with unit work per arrival, the [Poisson effective bandwidth](../../../queueing-theory.md#poisson-effective-bandwidth) is

$$
\alpha(\theta)=\frac{\nu(e^\theta-1)}{\theta}.
$$

Stability requires $c>\nu$. There is a unique positive root of $\nu(e^\theta-1)=c\theta$, again by strict [convexity](../../../real-analysis.md#convex-function), negative initial derivative after subtracting $c\theta$, and growth to infinity. For independent exponentially distributed work with rate $\beta$, the corresponding expressions are

$$
\kappa(\theta)=-\log(1-\theta/\beta),\qquad
\alpha(\theta)=\frac{-\log(1-\theta/\beta)}{\theta},\qquad 0<\theta<\beta.
$$

If $c>1/\beta$, the positive service root lies strictly below $\beta$. The finite [moment-generating function](../../../probability-theory.md#moment-generating-function) domain cannot be ignored.

To see statistical aggregation explicitly, let the entire arrival processes of $k$ sources be [independent](../../../random-variable.md#independent-random-variables), though each source may itself have dependence over time. Their cumulative totals satisfy

$$
\mathbb E e^{\theta\sum_{j=1}^k A_n^{(j)}}=\prod_{j=1}^k\mathbb E e^{\theta A_n^{(j)}},\qquad
\boxed{\alpha_{\rm total}(\theta,n)=\sum_{j=1}^k\alpha_j(\theta,n).}
$$

Thus the shared [queue](../../../queueing-theory.md#queue-queueing-theory) has an exponential overflow bound when $\sum_j\alpha_j(\theta)<c$, with the finite-window conditions proved above. One must use a common parameter $\theta$; adding individual service-root exponents is not the rule. For example, an independent [Poisson](../../../discrete-probability-distribution.md#poisson-distribution) source of mean $\nu$ and an independent on-off source of size $r$ and probability $p$ have aggregate [cumulant-generating function](../../../probability-theory.md#cumulant-generating-function)

$$
\kappa_{\rm total}(\theta)=\nu(e^\theta-1)+\log(1-p+pe^{\theta r}).
$$

For $\nu>0$ and $c>\nu+pr$, their positive service root exists and determines the optimized upper exponent. Several independent [Poisson](../../../discrete-probability-distribution.md#poisson-distribution) sources similarly have the same formula as one source with intensity $\sum_j\nu_j$.

The connection with [large deviation principles](../../../convergence-of-random-variables.md#large-deviation-principle) also appears in a many-source scaling. For $L$ independent copies of a source, aggregate service $Lc$ and buffer $Lb$, fix a window $n$. Let $X_i(n)$ be each copy's cumulative input in that window. Their total exceeds $L(b+cn)$ only if the empirical mean exceeds $b+cn$. Its [Chernoff bound](../../../probability-inequality.md#chernoff-bound) has exponent

$$
V_n(b)=\sup_{\theta\geq0}\{\theta(b+cn)-\log\mathbb E e^{\theta X_1(n)}\}
=\sup_{\theta\geq0}\theta\{b+n[c-\alpha(\theta,n)]\}.
$$

If exponential moments exist near zero, [Cramér's theorem](../../../probability-theory.md#cramer-s-theorem) gives the corresponding finite-window [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle). The threshold exceeds the mean because $m<c$ and $b>0$. A finite union of windows has upper exponential rate at most $-\min_n V_n(b)$ over those windows. Passing to infinitely many windows requires uniform control of long-window probabilities, not simply an interchange of a limit with an infinite union. A good sample-path [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle) in a topology where the [queue workload](../../../queueing-theory.md#workload-of-a-queue) is [continuous](../../../calculus.md#continuous-function), as in Question 3, instead permits the [contraction principle for large deviations](../../../convergence-of-random-variables.md#contraction-principle-for-large-deviations) to derive a workload [rate function](../../../convergence-of-random-variables.md#rate-function) and its closed-set overflow upper bound.

Finally, the [mean and peak limits of effective bandwidth](../../../queueing-theory.md#mean-and-peak-limits-of-effective-bandwidth) quantify the safety margin. With exponential moments near zero, independent slot work of mean $m$ and [variance](../../../variance.md) $v$ has

$$
\alpha(\theta)=m+\frac{v\theta}{2}+O(\theta^2).
$$

For bounded work, its large-parameter limit is the essential peak. Stronger tail requirements select larger $\theta$ and hence more capacity; finite-window [effective bandwidths](../../../queueing-theory.md#effective-bandwidth) also reflect temporal burst correlations. A stable heavy-tailed input can lack every positive exponential moment, in which case this exponential-bound method supplies no positive decay rate. Stability and exponentially small overflow are distinct requirements.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
