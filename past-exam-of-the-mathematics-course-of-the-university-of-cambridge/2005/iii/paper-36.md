# Paper 36

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper36.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper36.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)

## 1

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Write $p=1+\varepsilon$ and assume $\lambda>0$. The [large-deviation speed](../../../convergence-of-random-variables.md#large-deviation-speed) is $a_N=N^p$, and the answer is

$$
\boxed{I_A(x)=\begin{cases}\lambda x,&x\geq0,\\+\infty,&x<0.\end{cases}}
$$

Here and below a [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle) at speed $a_N$ means the open-set lower bound $\liminf a_N^{-1}\log\mathbb P(X_N\in G)\geq-\inf_G I$ and the closed-set upper bound $\limsup a_N^{-1}\log\mathbb P(X_N\in F)\leq-\inf_F I$. The displayed [rate function](../../../convergence-of-random-variables.md#rate-function) is nontrivial and is a [good rate function](../../../convergence-of-random-variables.md#good-rate-function).

For $0<u<v$, the [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) gives

$$
\mathbb P(A/a_N\in(u,v))=e^{-\lambda a_Nu}-e^{-\lambda a_Nv},
\qquad
\lim_N a_N^{-1}\log\mathbb P(A/a_N\in(u,v))=-\lambda u.
$$

Shrinking an interval about any $x>0$ supplies the local lower bound $-\lambda x$; neighborhoods of zero have [probability](../../../probability-theory.md#probability) tending to one. Every [open set](../../../topology.md#open-set) intersecting the nonnegative half-line contains one of these neighborhoods, giving the open-set bound. If a [closed set](../../../topology.md#closed-set) $F$ contains zero, its upper bound is just $\mathbb P(\cdot)\leq1$. If it meets $[0,\infty)$ but excludes zero, closedness gives $b=\inf(F\cap[0,\infty))>0$, and $\mathbb P(A/a_N\in F)\leq e^{-\lambda a_Nb}$. A [closed set](../../../topology.md#closed-set) disjoint from the support has [probability](../../../probability-theory.md#probability) zero. This proves the full [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle), including the boundary at zero.

The fixed exponential tail explains the speed: an excursion of size $xN^{1+\varepsilon}$ costs $e^{-\lambda xN^{1+\varepsilon}}$. The full [Gärtner–Ellis theorem](../../../convergence-of-random-variables.md#gartner-ellis-theorem) is unnecessary here; the limiting [cumulant-generating function](../../../probability-theory.md#cumulant-generating-function) is flat on $\theta<\lambda$ and infinite at $\theta\geq\lambda$, so it fails the theorem's [essential smoothness](../../../real-analysis.md#essential-smoothness-of-a-convex-function) hypothesis.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Assume $\sigma^2>0$; otherwise the scaled sum is deterministic and no nontrivial [rate function](../../../convergence-of-random-variables.md#rate-function) is possible. The sum has [normal distribution](../../../probability-theory.md#normal-distribution) $B_N\sim N(N\mu,N\sigma^2)$. For $X_N=B_N/N^{1+\varepsilon}$, use the faster [large-deviation speed](../../../convergence-of-random-variables.md#large-deviation-speed) $b_N=N^{1+2\varepsilon}$. The [moment-generating function of a normal distribution](../../../probability-theory.md#moment-generating-function-of-a-normal-distribution) yields

$$
\frac1{b_N}\log\mathbb E e^{b_N\theta X_N}
=\mu\theta N^{-\varepsilon}+\frac{\sigma^2\theta^2}{2}
\longrightarrow \Lambda(\theta)=\frac{\sigma^2\theta^2}{2}.
$$

The limiting [cumulant-generating function](../../../probability-theory.md#cumulant-generating-function) is finite and differentiable on all of $\mathbb R$, hence satisfies the [Gärtner–Ellis theorem](../../../convergence-of-random-variables.md#gartner-ellis-theorem). Its [Legendre-Fenchel transform](../../../convex-optimization.md#convex-conjugate) is obtained by maximizing $\theta x-\sigma^2\theta^2/2$, whose maximizer is $\theta=x/\sigma^2$. Thus

$$
\boxed{\text{speed }N^{1+2\varepsilon},\qquad I_B(x)=\frac{x^2}{2\sigma^2}\quad(x\in\mathbb R).}
$$

The drift disappears because the scaled [mean](../../../probability-theory.md#expected-value) is $\mu/N^\varepsilon\to0$. The [rate function](../../../convergence-of-random-variables.md#rate-function) is nontrivial and good. The corrected scaled [cumulant-generating function](../../../probability-theory.md#cumulant-generating-function) used here contains an [expectation](../../../probability-theory.md#expected-value); the corresponding formula in the paper's reference material omits it.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Use the [large-deviation speed](../../../convergence-of-random-variables.md#large-deviation-speed) $a_N=N^{1+\varepsilon}$ from part (a). For every $\eta>0$, the [Chernoff bound](../../../probability-inequality.md#chernoff-bound) for a [normal distribution](../../../probability-theory.md#normal-distribution) gives, for all sufficiently large $N$,

$$
\mathbb P(|B_N|>\eta a_N)
\leq2\exp\!\left[-\frac{(\eta a_N-|N\mu|)^2}{2N\sigma^2}\right].
$$

Consequently

$$
\limsup_N a_N^{-1}\log\mathbb P(|B_N|>\eta a_N)=-\infty,
$$

because the exponent has order $N^{1+2\varepsilon}$, exceeding $a_N$ by a factor $N^\varepsilon$. Thus $(A+B_N)/a_N$ and $A/a_N$ satisfy [exponential equivalence](../../../convergence-of-random-variables.md#exponential-equivalence). This conclusion does not require [independence](../../../random-variable.md#independent-random-variables) between $A$ and $B_N$, since their difference is exactly $B_N/a_N$.

The [exponential equivalence](../../../convergence-of-random-variables.md#exponential-equivalence) theorem transfers the [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle) and its [good rate function](../../../convergence-of-random-variables.md#good-rate-function), giving

$$
\boxed{\text{speed }N^{1+\varepsilon},\qquad I_{A+B}(x)=
\begin{cases}\lambda x,&x\geq0,\\+\infty,&x<0.\end{cases}}
$$

Large positive excursions are cheapest through the single [exponential random variable](../../../continuous-probability-distribution.md#exponential-distribution); a negative excursion would require the [Gaussian random variable](../../../probability-theory.md#gaussian-random-variable) sum to move on its faster scale. If $\sigma=0$, the deterministic shift $N\mu/a_N\to0$ gives the same conclusion directly.

## 2

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The printed [mean](../../../probability-theory.md#expected-value) is $1/(\lambda i)$, so $T_i$ has [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) of rate $i\lambda$. Let $S_k=\sum_{i=1}^kT_i$, with fixed $k$. Then

$$
\boxed{\text{speed }N,\qquad I_k^{\rm fixed}(x)=
\begin{cases}\lambda x,&x\geq0,\\+\infty,&x<0.\end{cases}}
$$

Here is a direct proof, which also identifies the exceptional role of the slowest exponential clock. For $0<\theta<\lambda$, [independence](../../../random-variable.md#independent-random-variables) and the [moment-generating function](../../../probability-theory.md#moment-generating-function) give

$$
\mathbb E e^{\theta S_k}=\prod_{i=1}^k\frac{i\lambda}{i\lambda-\theta}<\infty,\qquad
\limsup_N N^{-1}\log\mathbb P(S_k\geq Nx)\leq-\theta x.
$$

Letting $\theta\uparrow\lambda$ proves the tail upper bound $-\lambda x$. For a local lower bound at $x>0$, fix $0<\eta<x$ and $M>0$ with $\mathbb P(\sum_{i=2}^kT_i\leq M)>0$; for $k=1$ this [probability](../../../probability-theory.md#probability) is one. For large $N$, the event

$$
N(x-\eta/2)<T_1<N(x+\eta/2),\qquad
\sum_{i=2}^kT_i\leq M
$$

puts $S_k/N$ in $(x-\eta,x+\eta)$. Its logarithmic [probability](../../../probability-theory.md#probability) divided by $N$ tends to $-\lambda(x-\eta/2)$. Shrinking $\eta$ gives the local lower bound $-\lambda x$. At zero, $S_k/N\to0$ almost surely and neighborhoods have [probability](../../../probability-theory.md#probability) tending to one.

For any [closed set](../../../topology.md#closed-set) excluding zero, its nonnegative part is bounded away from zero; the tail upper bound applies at its [infimum](../../../real-analysis.md#infimum). Sets outside the support have [probability](../../../probability-theory.md#probability) zero. Together with the local lower bounds this proves the full [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle), with a [good rate function](../../../convergence-of-random-variables.md#good-rate-function). Equivalently, the [product large-deviation principle](../../../convergence-of-random-variables.md#product-large-deviation-principle) for the fixed vector $(T_1/N,\ldots,T_k/N)$ and the [contraction principle for large deviations](../../../convergence-of-random-variables.md#contraction-principle-for-large-deviations) minimize $\sum_i i\lambda u_i$ subject to $u_i\geq0$ and $\sum_i u_i=x$; all the excursion is assigned to $u_1$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Interpret the additional copies in $Z_N$ as [independent](../../../random-variable.md#independent-random-variables) of the initial $T_1,\ldots,T_k$, as well as of one another. Set $r=k\lambda$. The [Cramér theorem](../../../probability-theory.md#cramer-s-theorem) for rate-$r$ [exponential random variables](../../../continuous-probability-distribution.md#exponential-distribution) gives the [rate function](../../../convergence-of-random-variables.md#rate-function)

$$
K_r(z)=\begin{cases}rz-1-\log(rz),&z>0,\\+\infty,&z\leq0.\end{cases}
$$

Indeed their [cumulant-generating function](../../../probability-theory.md#cumulant-generating-function) is $\log(r/(r-\theta))$ for $\theta<r$, and the maximizer in its [Legendre-Fenchel transform](../../../convex-optimization.md#convex-conjugate) is $\theta=r-1/z$. For $Z_N/N$, replacing $N$ summands by $N-k$ does not change either the speed $N$ or this [rate function](../../../convergence-of-random-variables.md#rate-function). One can also see this directly from $N^{-1}\log\mathbb E e^{\theta Z_N}\to\log(r/(r-\theta))$ and the [Gärtner–Ellis theorem](../../../convergence-of-random-variables.md#gartner-ellis-theorem).

The [product large-deviation principle](../../../convergence-of-random-variables.md#product-large-deviation-principle), followed by the [contraction principle for large deviations](../../../convergence-of-random-variables.md#contraction-principle-for-large-deviations) under addition, now gives

$$
I_k(x)=\inf_{\substack{y\geq0,\ z>0\\y+z=x}}\{\lambda y+K_r(z)\}.
$$

For $x>0$ this is the minimum over $0<z\leq x$ of

$$
\lambda x+(r-\lambda)z-1-\log(rz).
$$

If $k>1$, its derivative with respect to $z$ is $r-\lambda-1/z$. Hence the optimum is $z=\min(x,1/[\lambda(k-1)])$, and

$$
\boxed{I_k(x)=
\begin{cases}
+\infty,&x\leq0,\\
k\lambda x-1-\log(k\lambda x),&0<x\leq\frac1{\lambda(k-1)},\\
\lambda x+\log\frac{k-1}{k},&x\geq\frac1{\lambda(k-1)}.
\end{cases}\qquad\text{speed }N.}
$$

The two expressions agree at the transition and have the same derivative $\lambda$. The minimum rate zero occurs at the typical value $x=1/(k\lambda)$. If $k=1$, the minimand is $\lambda x-1-\log(\lambda z)$, decreasing in $z$, so instead

$$
\boxed{I_1(x)=\lambda x-1-\log(\lambda x)\ (x>0),\qquad I_1(x)=+\infty\ (x\leq0).}
$$

These are [good rate functions](../../../convergence-of-random-variables.md#good-rate-function). The affine branch for $k>1$ is the [slow exponential plus an exponential sample mean](../../../continuous-probability-distribution.md#slow-exponential-plus-an-exponential-sample-mean) mechanism: the bulk ceases to carry additional excess, which instead comes from $T_1$. In particular, blindly applying the full [Gärtner–Ellis theorem](../../../convergence-of-random-variables.md#gartner-ellis-theorem) to the combined sum would be unjustified. Its limiting [cumulant-generating function](../../../probability-theory.md#cumulant-generating-function) is $\log(r/(r-\theta))$ only for $\theta<\lambda$, with a finite boundary slope when $k>1$; [essential smoothness](../../../real-analysis.md#essential-smoothness-of-a-convex-function) fails. The product and contraction argument proves the missing lower bounds.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Write $S_N=\sum_{i=1}^NT_i$. The answer is

$$
\boxed{\text{speed }N,\qquad I(x)=
\begin{cases}\lambda x,&x\geq0,\\+\infty,&x<0.\end{cases}}
$$

The [sum of exponential variables with linearly increasing rates](../../../continuous-probability-distribution.md#sum-of-exponential-variables-with-linearly-increasing-rates) has the distribution of the maximum of $N$ [independent](../../../random-variable.md#independent-random-variables) rate-$\lambda$ [exponential random variables](../../../continuous-probability-distribution.md#exponential-distribution). To prove this identity, start $N$ [independent](../../../random-variable.md#independent-random-variables) rate-$\lambda$ exponential clocks. The first rings after a rate-$N\lambda$ exponential time; the [memoryless property](../../../continuous-probability-distribution.md#memorylessness-of-the-exponential-distribution) leaves $N-1$ fresh [independent](../../../random-variable.md#independent-random-variables) clocks. Repeating this argument shows that the successive [order statistic](../../../probability-theory.md#order-statistic) gaps are [independent](../../../random-variable.md#independent-random-variables), with rates $N\lambda,(N-1)\lambda,\ldots,\lambda$. Their sum has the distribution of $S_N$. Therefore

$$
\mathbb P(S_N\leq t)=(1-e^{-\lambda t})^N\quad(t\geq0).
$$

For $x>0$, $N e^{-\lambda Nx}\to0$, and hence

$$
\mathbb P(S_N>Nx)=1-(1-e^{-\lambda Nx})^N
\sim N e^{-\lambda Nx},\qquad
\lim_NN^{-1}\log\mathbb P(S_N>Nx)=-\lambda x.
$$

If $0<u<v$, subtracting the two tails gives the interval exponent $-\lambda u$, since the tail at $Nv$ is exponentially smaller. Also $\mathbb E S_N=\lambda^{-1}\sum_{i=1}^N i^{-1}=O(\log N)$, so the [Markov inequality](../../../probability-inequality.md#markov-inequality) gives $S_N/N\to0$ in [probability](../../../probability-theory.md#probability). Local lower bounds at positive points and at zero follow; the tail estimate gives the closed-set upper bound exactly as in part (a). This proves the full [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle).

There is also a deduction from part (b). For fixed $k$ and $i>k$, a rate-$i\lambda$ [exponential random variable](../../../continuous-probability-distribution.md#exponential-distribution) is stochastically smaller than a rate-$k\lambda$ one. Coupling by the same uniform variables therefore gives $S_N\leq S_k+Z_N$ with [independent](../../../random-variable.md#independent-random-variables) additional copies. For fixed $x>0$ and sufficiently large $k$, the upper-tail exponent from part (b) is $-\lambda x-\log((k-1)/k)$. Let $k\to\infty$ to obtain $-\lambda x$; the lower tail estimate $\mathbb P(S_N>Nx)\geq\mathbb P(T_1>Nx)=e^{-\lambda Nx}$ matches it. The exact maximum identity additionally supplies all local lower bounds.

## 3

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Put $\kappa=2(1-H)>0$. For the [Gaussian process](../../../stochastic-process.md#gaussian-process) $Z$, [self-similarity of a stochastic process](../../../stochastic-process.md#self-similarity-of-a-stochastic-process) gives the identity in distribution

$$
\frac{Z(N\,\cdot)}{N}\ \overset d=\ N^{H-1}Z
=\frac{Z}{\sqrt{N^\kappa}}.
$$

Apply the given small-noise [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle) with $L=N^\kappa$. The answer is

$$
\boxed{\text{speed }N^{2(1-H)},\qquad\text{good rate function }I.}
$$

No [Legendre-Fenchel transform](../../../convex-optimization.md#convex-conjugate) needs to be recomputed: the scaled paths have exactly the small-noise law at this scale.

If the stated small-noise [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle) is indexed only by integer $L$, use $L_N=\lfloor N^\kappa\rfloor$. This gives speed $N^\kappa$ as well, since $L_N/N^\kappa\to1$. The multiplying factor $\sqrt{L_N/N^\kappa}\to1$ does not change the [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle). To justify this last step, the error in the path norm is $o(1)\|Z/\sqrt{L_N}\|$. For each fixed $M$, [good rate functions](../../../convergence-of-random-variables.md#good-rate-function) have bounded sublevel sets, so $\inf_{\|f\|\geq M}I(f)\to\infty$ as $M\to\infty$. The closed-set upper bound then makes the [probability](../../../probability-theory.md#probability) of an error greater than any fixed $\eta>0$ superexponentially small. Thus [exponential equivalence](../../../convergence-of-random-variables.md#exponential-equivalence) applies. This also justifies positive real, rather than only integer, rescalings used in part (c).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $\delta=C-\mu>0$, and first suppose $\sigma>0$. For the infinite-horizon contraction, use the usual [sublinear path space for fluid queues](../../../queueing-theory.md#sublinear-path-space-for-fluid-queues),

$$
\mathcal C_0=\{f\in C([0,\infty)):f(0)=0,\ f(t)/(1+t)\to0\},
\qquad \|f\|_{\rm sl}=\sup_{t\geq0}\frac{|f(t)|}{1+t}.
$$

We interpret the supplied path-space [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle) in this norm, or in a topology with the same workload-continuity property. The paper does not specify its norm explicitly; mere convergence on compact time intervals would not justify an infinite-horizon contraction.

Define the [queue workload](../../../queueing-theory.md#workload-of-a-queue) functional

$$
R(f)=\sup_{t\geq0}\{\sigma f(t)-\delta t\}.
$$

It is finite and nonnegative on the [sublinear path space for fluid queues](../../../queueing-theory.md#sublinear-path-space-for-fluid-queues). Here is the required continuity argument. Fix $f$ and choose $T\geq1$ so that $|\sigma f(t)|\leq\delta t/4$ for $t\geq T$. If $\|g-f\|_{\rm sl}<\delta/(4\sigma)$, then for $t\geq T$,

$$
\sigma g(t)-\delta t
\leq\frac{\delta t}{4}+\frac{\delta(1+t)}4-\delta t
=\frac{\delta}{4}-\frac{\delta t}{2}<0.
$$

The corresponding expression for $f$ is also negative there, whereas at zero both are zero. Each [supremum](../../../real-analysis.md#supremum) can therefore be restricted to $[0,T]$, giving

$$
|R(g)-R(f)|\leq\sigma(1+T)\|g-f\|_{\rm sl}.
$$

Thus $R$ is a [continuous map](../../../topology.md#continuous-map); this proof also shows why the negative drift is essential.

Substituting $t=Ns$ into the [queue workload](../../../queueing-theory.md#workload-of-a-queue) gives

$$
\frac{r(X)}N=\sup_{s\geq0}\left\{\sigma\frac{Z(Ns)}N-\delta s\right\}
=R\!\left(\frac{Z(N\,\cdot)}N\right).
$$

The [contraction principle for large deviations](../../../convergence-of-random-variables.md#contraction-principle-for-large-deviations) says that a continuous image of a family with [good rate function](../../../convergence-of-random-variables.md#good-rate-function) $I$ has the same [large-deviation speed](../../../convergence-of-random-variables.md#large-deviation-speed) and [good rate function](../../../convergence-of-random-variables.md#good-rate-function) obtained by minimizing $I$ over each fibre. Consequently

$$
\boxed{\text{speed }N^{2(1-H)},\qquad
J(q)=\inf_{\{f:R(f)=q\}}I(f)\quad(q\geq0),\qquad J(q)=+\infty\quad(q<0).}
$$

In particular $J(0)=0$: $Z/\sqrt L\to0$ in the path norm almost surely, so the given [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle) and [lower semicontinuity](../../../calculus.md#lower-semicontinuity) give $I(0)=0$, and $R(0)=0$. If $\sigma=0$, the [queue workload](../../../queueing-theory.md#workload-of-a-queue) is identically zero and the [rate function](../../../convergence-of-random-variables.md#rate-function) is zero at zero and infinite elsewhere. No unspecified [variance](../../../variance.md) normalization of the [fractional Brownian motion](../../../stochastic-process.md#fractional-brownian-motion) is needed for this variational answer.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let $\kappa=2(1-H)$ and fix $a>0$. Starting with part (b), the [contraction principle for large deviations](../../../convergence-of-random-variables.md#contraction-principle-for-large-deviations) under the map $q\mapsto q/a$ gives an LDP for $r(X)/(aN)$ with speed $N^\kappa$ and [rate function](../../../convergence-of-random-variables.md#rate-function) $q\mapsto J(aq)$.

Alternatively, replace $N$ by $aN$ in parts (a) and (b), using the real-scale justification in part (a). The same family has [large-deviation speed](../../../convergence-of-random-variables.md#large-deviation-speed) $(aN)^\kappa$ and [rate function](../../../convergence-of-random-variables.md#rate-function) $J(q)$. When expressed at speed $N^\kappa$, that [rate function](../../../convergence-of-random-variables.md#rate-function) is $a^\kappa J(q)$. The two descriptions of the same [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle) must agree:

$$
J(aq)=a^\kappa J(q).
$$

For clarity, uniqueness here is a general property of [lower semicontinuous](../../../calculus.md#lower-semicontinuity) [rate functions](../../../convergence-of-random-variables.md#rate-function): at a point $x$, the shrinking-neighborhood logarithmic bounds recover $I(x)$, since $\inf_{B(x,\eta)}I\to I(x)$ as $\eta\downarrow0$. Thus two [rate functions](../../../convergence-of-random-variables.md#rate-function) for the same family and speed cannot differ.

Taking the base argument $q=1$ and replacing $a$ by any positive [queue](../../../queueing-theory.md#queue-queueing-theory) size gives

$$
\boxed{J(q)=q^{2(1-H)}J(1)\quad(q>0),\qquad J(0)=0.}
$$

For $q<0$ the [rate function](../../../convergence-of-random-variables.md#rate-function) is infinite. In the usual nondegenerate case $J(1)$ is finite, so the formula also holds at $q=0$. This is the [self-similar Gaussian workload rate](../../../queueing-theory.md#self-similar-gaussian-workload-rate); the exponent comes from the [Hurst parameter](../../../stochastic-process.md#hurst-exponent), while the constant comes from the path [rate function](../../../convergence-of-random-variables.md#rate-function) and the drift and noise scales.

## 4

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For the amount of work $A_j(0,t]$ offered by one flow in a time interval of length $t$, its [effective bandwidth](../../../queueing-theory.md#effective-bandwidth) at parameter $\theta>0$ and timescale $t>0$ is

$$
\boxed{\alpha_j(\theta,t)=\frac1{\theta t}\log\mathbb E e^{\theta A_j(0,t]}.}
$$

Its units are work per unit time. The parameter $\theta$ measures the price placed on bursts: a stringent rare-overflow target generally requires a larger value of $\theta$ than a loose target. The timescale $t$ describes the duration of the congestion episode. When the limit exists, write

$$
\Lambda_j(\theta)=\lim_{t\to\infty}t^{-1}\log\mathbb E e^{\theta A_j(0,t]},
\qquad a_j(\theta)=\Lambda_j(\theta)/\theta.
$$

This is the long-time [effective bandwidth](../../../queueing-theory.md#effective-bandwidth). It includes a burstiness cost, rather than just the [mean](../../../probability-theory.md#expected-value) offered rate. For a finite-time flow with the required moments, $\lim_{\theta\downarrow0}\alpha_j(\theta,t)=\mathbb E A_j(0,t]/t$, and [effective bandwidth](../../../queueing-theory.md#effective-bandwidth) is increasing in $\theta$. If $A_j(0,t]/t$ is bounded, its limit as $\theta\to\infty$ is the essential [supremum](../../../real-analysis.md#supremum) of that interval's input rate, the peak-rate limit. The analogous long-time [mean](../../../probability-theory.md#expected-value) limit requires the usual interchange or regularity assumptions.

For [independent](../../../random-variable.md#independent-random-variables) flows their [cumulant-generating functions](../../../probability-theory.md#cumulant-generating-function) add, so

$$
\alpha_{\rm total}(\theta,t)=\sum_j\alpha_j(\theta,t),\qquad
a_{\rm total}(\theta)=\sum_j a_j(\theta).
$$

The [Chernoff bound](../../../probability-inequality.md#chernoff-bound) therefore gives, for any $\theta>0$ in the common domain,

$$
\mathbb P(A_{\rm total}(0,t]>Ct+b)
\leq\exp\{-\theta[b+Ct-t\alpha_{\rm total}(\theta,t)]\}.
$$

Optimizing over $\theta$ produces the relevant [Legendre-Fenchel transform](../../../convex-optimization.md#convex-conjugate). The [Cramér theorem](../../../probability-theory.md#cramer-s-theorem) states that sample means of [independent and identically distributed](../../../random-variable.md#independent-and-identically-distributed-random-variables) inputs whose [moment-generating function](../../../probability-theory.md#moment-generating-function) is finite near zero have a [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle), with [rate function](../../../convergence-of-random-variables.md#rate-function) equal to the [Legendre-Fenchel transform](../../../convex-optimization.md#convex-conjugate) of their [cumulant-generating function](../../../probability-theory.md#cumulant-generating-function). More generally, the [Gärtner–Ellis theorem](../../../convergence-of-random-variables.md#gartner-ellis-theorem) applies to a convergent scaled log [moment-generating function](../../../probability-theory.md#moment-generating-function) when zero lies inside its domain and the limit is [lower semicontinuous](../../../calculus.md#lower-semicontinuity) and [essentially smooth](../../../real-analysis.md#essential-smoothness-of-a-convex-function). It gives the same transform as a [good rate function](../../../convergence-of-random-variables.md#good-rate-function). A sample-path version, together with the [contraction principle for large deviations](../../../convergence-of-random-variables.md#contraction-principle-for-large-deviations) for the [queue workload](../../../queueing-theory.md#workload-of-a-queue), translates input deviations into overflow deviations. The compact-time and infinite-horizon continuity/tail hypotheses must be checked for the chosen traffic model.

A particularly useful rigorous [queue](../../../queueing-theory.md#queue-queueing-theory) bound holds for inputs with [stationary increments](../../../stochastic-process.md#stationary-increments) and [independent increments](../../../stochastic-process.md#independent-increments), such that $\mathbb E e^{\theta A(t)}=e^{t\Lambda(\theta)}$. If $\Lambda(\theta)\leq C\theta$, then

$$
M_t=e^{\theta(A(t)-Ct)}
$$

is a nonnegative [supermartingale](../../../martingale.md#supermartingale), since its conditional increment factor is $e^{(t-s)(\Lambda(\theta)-C\theta)}\leq1$. The [maximal inequality for a nonnegative supermartingale](../../../martingale.md#maximal-inequality-for-a-nonnegative-supermartingale) on $[0,T]$, followed by $T\to\infty$, gives the [continuous-time exponential workload bound](../../../queueing-theory.md#continuous-time-exponential-workload-bound)

$$
\boxed{\mathbb P(W\geq b)\leq e^{-\theta b},
\qquad W\overset d=\sup_{t\geq0}(A(t)-Ct),\quad
\sum_j a_j(\theta)\leq C.}
$$

Here $W$ is the stationary [queue workload](../../../queueing-theory.md#workload-of-a-queue) of the stable infinite-buffer [queue](../../../queueing-theory.md#queue-queueing-theory), represented by input from the past. This directly bounds the [supremum](../../../real-analysis.md#supremum) over time; applying a one-time [Chernoff bound](../../../probability-inequality.md#chernoff-bound) alone would not establish it.

For a nonzero [Compound Poisson process](../../../stochastic-process.md#compound-poisson-process) with bounded positive packet sizes and [mean](../../../probability-theory.md#expected-value) input rate less than $C$, a positive root $\theta_*$ of $\Lambda(\theta)=C\theta$ exists and is unique. Here the root theorem can be made explicit:

$$
e^{-\theta_*(b+s_{\max})}\leq\mathbb P(W\geq b)\leq e^{-\theta_*b}\quad(b>0).
$$

The upper bound was just proved. For the lower bound, use [exponential tilting](../../../probability-theory.md#exponential-tilting) with density $e^{\theta_*(A(t)-Ct)}$ at time $t$. Under the tilted law the net input has positive [mean](../../../probability-theory.md#expected-value) drift $\Lambda'(\theta_*)-C>0$, by strict convexity and the positive-root equation. The [strong law of large numbers](../../../convergence-of-random-variables.md#strong-law-of-large-numbers) then makes the first crossing time $\tau_b$ finite almost surely under that law. Its overshoot is at most $s_{\max}$. Changing measure at $\tau_b$, first on $\{\tau_b\leq T\}$ and then letting $T\to\infty$, gives

$$
\mathbb P(\tau_b<\infty)=\mathbb E_*\!\left[e^{-\theta_*(A(\tau_b)-C\tau_b)}\right]
\geq e^{-\theta_*(b+s_{\max})}.
$$

Dividing the logarithmic bounds by $b$ proves $\lim_{b\to\infty}b^{-1}\log\mathbb P(W\geq b)=-\theta_*$.

Thus the familiar admission rule compares $\sum_j a_j(\theta)$ with $C$, choosing $\theta$ from the desired buffer-tail exponent. For more general inputs, a logarithmic root theorem requires its own light-tail and renewal or sample-path hypotheses; the displayed supermartingale upper bound needs only the moment and increment assumptions stated above.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The capacity and quality targets alone do not determine flow counts: the per-flow traffic statistics must also be supplied. The following explicit model gives a computable sufficient region, with genuine upper bounds on both loss fractions.

Measure [queue workload](../../../queueing-theory.md#workload-of-a-queue) and buffer size in bits. Denote capacity by $C$, shared buffer size by $B$, voice delay limit by $D$, target voice loss by $\ell_v$, and target data loss by $\ell_d$, with $0<\ell_v,\ell_d<1$. Let there be $n_v$ voice flows and $n_d$ data flows. Model each class-$j$ flow, $j\in\{v,d\}$, by a stationary [Compound Poisson process](../../../stochastic-process.md#compound-poisson-process) with packet rate $\nu_j$ and positive [independent](../../../random-variable.md#independent-random-variables) packet sizes $S_j$, and assume [independence](../../../random-variable.md#independent-random-variables) across flows and marks. Use a work-conserving preemptive-resume [priority queue with a shared buffer](../../../queueing-theory.md#priority-queue-with-a-shared-buffer), with voice priority and [first come first served](../../../queueing-theory.md#first-come-first-served) within each class. This preemptive or fluid approximation makes the predicted voice waiting time exactly $V/C$, where $V$ is the remaining voice [queue workload](../../../queueing-theory.md#workload-of-a-queue) just before arrival. Assume packet sizes are bounded by a known $s_{\max}<B$ and interpret the buffer gate as a packet-fit test; rejecting packets which do not fit is the packet version of the full-buffer rule.

For one flow the [Compound Poisson process](../../../stochastic-process.md#compound-poisson-process) formula gives

$$
\Lambda_j(\theta)=\nu_j(\mathbb E e^{\theta S_j}-1),\qquad
\boxed{a_j(\theta)=\frac{\nu_j(\mathbb E e^{\theta S_j}-1)}{\theta}.}
$$

For fixed-size packets of size $s_j$, substitute $e^{\theta s_j}$. Estimate the packet rate and size law from measurements or a declared traffic contract. Also require the strict stability inequality

$$
n_v\nu_v\mathbb E S_v+n_d\nu_d\mathbb E S_d<C.
$$

Define $B_0=B-s_{\max}>0$ and $K=CD$. Couple the switch with an unthinned infinite-buffer aggregate [queue](../../../queueing-theory.md#queue-queueing-theory) and an unthinned infinite-buffer voice-only [queue](../../../queueing-theory.md#queue-queueing-theory), both driven by the same offered packets and both served at rate $C$. Under the preemptive [service discipline](../../../queueing-theory.md#service-discipline), dropping arrivals can only decrease both the total [queue workload](../../../queueing-theory.md#workload-of-a-queue) and the voice [queue workload](../../../queueing-theory.md#workload-of-a-queue). Thus total switch [queue workload](../../../queueing-theory.md#workload-of-a-queue) $Q$ and voice [queue workload](../../../queueing-theory.md#workload-of-a-queue) $V$ satisfy $Q\leq W_T$ and $V\leq W_V$ in the stationary coupling. A packet-fit loss implies $Q>B-S_j\geq B_0$, and a voice-delay rejection implies $V\geq K$.

Apply the [continuous-time exponential workload bound](../../../queueing-theory.md#continuous-time-exponential-workload-bound) to the two comparison [queues](../../../queueing-theory.md#queue-queueing-theory). For any positive $\theta_T,\theta_V$ satisfying

$$
n_v a_v(\theta_T)+n_d a_d(\theta_T)\leq C,\qquad
n_v a_v(\theta_V)\leq C,
$$

the stationary loss-event [probabilities](../../../probability-theory.md#probability) obey

$$
\boxed{p_d\leq e^{-\theta_T B_0},\qquad
p_v\leq e^{-\theta_T B_0}+e^{-\theta_V K}.}
$$

The second inequality is a [union bound](../../../probability-inequality.md#boole-s-inequality): voice can be lost either at the shared buffer or at its delay gate. Data congestion therefore contributes to voice loss despite its lower service priority. [Poisson arrivals see time averages](../../../queueing-theory.md#poisson-arrivals-see-time-averages) applies to each offered packet stream, whose future arrivals are [independent](../../../random-variable.md#independent-random-variables) of the prearrival state; the stationary event bounds are consequently bounds on the offered-packet loss fractions. Voice packets that are admitted have [queueing delay](../../../queueing-theory.md#queueing-delay) below $D$, because later voice packets join behind them and data work cannot delay them in this model.

To turn the bounds into flow counts, allocate loss budgets

$$
0<\eta_B<\min(\ell_d,\ell_v),\qquad
\eta_V=\ell_v-\eta_B,\qquad
\theta_T=\frac{\log(1/\eta_B)}{B_0},\quad
\theta_V=\frac{\log(1/\eta_V)}{CD}.
$$

For example, $\eta_B=\min(\ell_d,\ell_v/2)$ and $\eta_V=\ell_v-\eta_B$ also work; equality with $\ell_d$ is harmless. The required sufficient [effective-bandwidth admission region with a voice delay gate](../../../queueing-theory.md#effective-bandwidth-admission-region-with-a-voice-delay-gate) is

$$
\boxed{\begin{gathered}
n_v a_v(\theta_V)\leq C,\\
n_v a_v(\theta_T)+n_d a_d(\theta_T)\leq C,\\
n_v\nu_v\mathbb E S_v+n_d\nu_d\mathbb E S_d<C,\qquad
n_v,n_d\in\mathbb Z_{\geq0}.
\end{gathered}}
$$

It ensures $p_d\leq\ell_d$ and $p_v\leq\ell_v$. A simple enumeration is

$$
0\leq n_v\leq\left\lfloor\frac C{a_v(\theta_V)}\right\rfloor,\qquad
0\leq n_d\leq
\left\lfloor\frac{C-n_v a_v(\theta_T)}{a_d(\theta_T)}\right\rfloor,
$$

discarding negative bounds and pairs failing strict mean-load stability. The formulas assume positive-rate nonzero-size flows. Optimize a chosen revenue or flow-count objective over these integer pairs. Searching over the budget split $\eta_B$ can enlarge the sufficient region. For a bit-fluid buffer gate with no packet-fit issue, $B_0$ can be replaced by $B$.

Real nonpreemptive packet service needs an additional residual-service allowance or an explicit priority [queue workload](../../../queueing-theory.md#workload-of-a-queue) analysis: a voice packet may have to wait for the data packet already in service. Burst-correlated voice sources also require richer descriptors, such as measured finite-time [effective bandwidths](../../../queueing-theory.md#effective-bandwidth) $\alpha_j(\theta,t)$ or a Markov-modulated source model. For such inputs, additivity still holds for [independent](../../../random-variable.md#independent-random-variables) flows, but the independent-increment supermartingale bound is not automatic; use a valid sample-path [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle) or a model-specific overflow bound, with prefactors or a safety margin when using asymptotics. If packet arrivals do not form a [Poisson process](../../../probability-theory.md#poisson-process), loss fractions must be assessed at arrival epochs rather than inferred solely from time-average [queue workload](../../../queueing-theory.md#workload-of-a-queue) [probabilities](../../../probability-theory.md#probability). These qualifications explain both how to calculate an admission region from specified traffic statistics and why the five switch/QoS parameters by themselves cannot supply a numerical answer.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
