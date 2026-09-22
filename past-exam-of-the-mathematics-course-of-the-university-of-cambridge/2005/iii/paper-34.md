# Paper 34

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper34.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper34.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
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
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
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
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)

## 1

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

For a [martingale](../../../martingale.md) and a [stopping time](../../../martingale.md#stopping-time) $T\leq N$, expand the stopped value using its [martingale differences](../../../martingale.md#martingale-difference):

$$
M_T-M_0=\sum_{k=1}^N\mathbf1_{\{T\geq k\}}(M_k-M_{k-1}).
$$

The event $\{T\geq k\}=\{T>k-1\}$ belongs to the [filtration](../../../stochastic-process.md#filtration-probability-theory) $\mathcal F_{k-1}$. Each summand is integrable and its [conditional expectation](../../../measure-theory.md#conditional-expectation) given $\mathcal F_{k-1}$ is zero. Taking [expectations](../../../probability-theory.md#expected-value) of this finite sum therefore proves **$\mathbb E M_T=\mathbb E M_0$ for every bounded stopping time**. This proves the forward direction of the [bounded-stopping-time characterization of a martingale](../../../martingale.md#bounded-stopping-time-characterization-of-a-martingale) without assuming an [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale).

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

For $A\in\mathcal F_n$, define the bounded [stopping time](../../../martingale.md#stopping-time) $T=n+1$ on $A$ and $T=n$ on $A^c$. Before time $n$ its stopping events are empty, at time $n$ the event $\{T\leq n\}=A^c$ belongs to $\mathcal F_n$, and subsequently it has stopped everywhere. Subtract the assumed mean identity for this $T$ from that for the constant [stopping time](../../../martingale.md#stopping-time) $n$ to obtain

$$
\mathbb E\bigl[\mathbf1_A(M_{n+1}-M_n)\bigr]=0\qquad(A\in\mathcal F_n).
$$

Since $M_n$ is integrable and $\mathcal F_n$-[measurable](../../../measure-theory.md#measurability), this is precisely the defining property of [conditional expectation](../../../measure-theory.md#conditional-expectation) giving **$\mathbb E[M_{n+1}\mid\mathcal F_n]=M_n$**. Thus the [adapted process](../../../stochastic-process.md#adapted-process) is a [martingale](../../../martingale.md), completing the [bounded-stopping-time characterization of a martingale](../../../martingale.md#bounded-stopping-time-characterization-of-a-martingale).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The required condition is [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability), written entirely in terms of the given [probability laws](../../../probability-theory.md#probability-distribution):

$$
\boxed{\lim_{R\to\infty}\sup_n\int_{\{|x|>R\}}|x|\,\mu_n(dx)=0.}
$$

Together with the given [almost sure convergence](../../../convergence-of-random-variables.md#almost-sure-convergence), this implies [L1 convergence](../../../convergence-of-random-variables.md#convergence-in-l1) to an integrable $M_\infty$. Passing to the limit in $\mathbb E[M_m\mid\mathcal F_n]=M_n$, using the contraction property of [conditional expectation](../../../measure-theory.md#conditional-expectation) in [L1 space](../../../measure-theory.md#l1-space), gives $M_n=\mathbb E[M_\infty\mid\mathcal F_n]$.

For every bounded [stopping time](../../../martingale.md#stopping-time) $S$, the same identity holds with $\mathcal F_S$: split an event of its [stopping-time sigma-algebra](../../../martingale.md#stopping-time-sigma-algebra) according to $\{S=k\}$ and use the deterministic-time identity. In particular $M_{T\wedge n}=\mathbb E[M_\infty\mid\mathcal F_{T\wedge n}]$. These [conditional expectations](../../../measure-theory.md#conditional-expectation) are [uniformly integrable](../../../convergence-of-random-variables.md#uniform-integrability): for an integrable $Y$ and $Z=\mathbb E[Y\mid\mathcal G]$, the event $A=\{|Z|>K\}$ satisfies $\mathbb P(A)\leq\mathbb E|Y|/K$, and

$$
\mathbb E[|Z|;A]\leq\mathbb E[|Y|;|Y|>R]+R\mathbb E|Y|/K.
$$

First choose $R$, then $K$, uniformly in $\mathcal G$. Define $M_T=M_\infty$ on $\{T=\infty\}$. Now $M_{T\wedge n}\to M_T$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) and in [L1 space](../../../measure-theory.md#l1-space), so the bounded-time mean identities imply **$\mathbb E M_T=\mathbb E M_0$ even when $T$ can be infinite**.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

With the natural [filtration](../../../stochastic-process.md#filtration-probability-theory) $\mathcal F_n=\sigma(Z_1,\ldots,Z_n)$, the sums form a [martingale](../../../martingale.md). Put $v_n=\sum_{k\leq n}a_k^2$. [Independence](../../../random-variable.md#independent-random-variables) and the [characteristic function](../../../probability-theory.md#characteristic-function) of a [standard normal random variable](../../../probability-theory.md#standard-normal-random-variable) give

$$
\mathbb E e^{iuM_n}=e^{-u^2v_n/2}.
$$

If $M_n\to M_\infty$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) with a finite limit, [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem) gives convergence of these [characteristic functions](../../../probability-theory.md#characteristic-function) to $\mathbb E e^{iuM_\infty}$. If $v_n\to\infty$, that limit would be $1$ at zero and $0$ at every nonzero $u$. A [characteristic function](../../../probability-theory.md#characteristic-function) is continuous at zero: apply [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem) to $e^{iuM_\infty}$ as $u\to0$. This contradiction proves

$$
\boxed{\sum_{k=1}^\infty a_k^2<\infty.}
$$

This is also sufficient by the [L2-bounded martingale convergence theorem](../../../martingale.md#l2-bounded-martingale-convergence-theorem), since $\mathbb EM_n^2=v_n$. Thus the [almost sure convergence criterion for an independent Gaussian series](../../../probability-theory.md#almost-sure-convergence-criterion-for-an-independent-gaussian-series) is an equivalence.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The exact condition is again **$\sum_ka_k^2<\infty$**, with the terminal almost-sure limit used to define $M_T$ when $T=\infty$. In that case $\sup_n\mathbb EM_n^2<\infty$, and

$$
\mathbb E[|M_n|;|M_n|>R]\leq\frac{\mathbb EM_n^2}{R}
$$

proves [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability). The preceding unbounded [optional stopping](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) argument yields $\boxed{\mathbb E M_T=0}$.

For necessity, suppose $v_n\to\infty$. For every fixed $R>0$, the [normal distribution](../../../probability-theory.md#normal-distribution) of $M_n$ gives $\mathbb P(M_n\geq R)\to1/2$. Hence $\mathbb P(\sup_nM_n\geq R)\geq1/2$, and intersecting over positive integer $R$ shows $\mathbb P(\sup_nM_n=\infty)\geq1/2$. Unboundedness above is unchanged by altering finitely many of the [independent](../../../random-variable.md#independent-random-variables) $Z_k$, because that changes all sufficiently late sums by one finite constant. It is therefore a [tail event](../../../probability-theory.md#tail-event); the [Kolmogorov zero-one law](../../../probability-theory.md#kolmogorov-s-zero-one-law) makes its probability one. Consequently $T<\infty$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) and $M_T\geq1$. Its [expectation](../../../probability-theory.md#expected-value) is at least one, possibly infinite, and cannot equal zero. This proves the necessity assertion in [threshold stopping of an independent Gaussian series](../../../probability-theory.md#threshold-stopping-of-an-independent-gaussian-series).

## 2

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [almost sure submartingale convergence theorem](../../../martingale.md#almost-sure-submartingale-convergence-theorem) states that a discrete-time [submartingale](../../../martingale.md#submartingale) $Y_n$ satisfying $\sup_n\mathbb E Y_n^+<\infty$ converges [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) to a finite integrable limit. In particular, **a martingale with $\sup_n\mathbb E|M_n|<\infty$ converges almost surely to an integrable $M_\infty$**, and $\mathbb E|M_\infty|\leq\sup_n\mathbb E|M_n|$ by [Fatou's lemma](../../../measure-theory.md#fatou-s-lemma). This is the [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem). [Uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability) gives the stronger conclusion of [L1 convergence](../../../convergence-of-random-variables.md#convergence-in-l1); it is not implied by bounded first moments alone.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Take $\Omega=[0,1)$ with its [Borel sigma-algebra](../../../measure-theory.md#borel-sigma-algebra) and [Lebesgue measure](../../../measure-theory.md#lebesgue-measure) of total mass one. Let $\mathcal F_n$ be the finite [sigma-algebra](../../../measure-theory.md#sigma-algebra) generated by the half-open [dyadic intervals](../../../real-analysis.md#dyadic-interval) of length $2^{-n}$. Set $X_0=f(1)-f(0)$ if the indexing begins at one. Each $X_n$ is [adapted](../../../stochastic-process.md#adapted-process) to this [filtration](../../../stochastic-process.md#filtration-probability-theory), and if $L$ is a [Lipschitz constant](../../../real-analysis.md#lipschitz-constant) of $f$, then $|X_n|\leq L$, so every coordinate is integrable.

On a parent interval $[u,u+2^{-n})$, [conditional expectation](../../../measure-theory.md#conditional-expectation) averages the two equally likely child values. Their average is

$$
\frac12\,2^{n+1}\bigl(f(u+2^{-n-1})-f(u)+f(u+2^{-n})-f(u+2^{-n-1})\bigr)
=2^n\bigl(f(u+2^{-n})-f(u)\bigr)=X_n.
$$

Thus **$\mathbb E[X_{n+1}\mid\mathcal F_n]=X_n$**, establishing the [dyadic slope martingale](../../../martingale.md#dyadic-slope-martingale). One can equivalently include $1$ as a separate null atom without changing any [probability law](../../../probability-theory.md#probability-distribution).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The [dyadic slope martingale](../../../martingale.md#dyadic-slope-martingale) is uniformly bounded by $L$. The [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem) gives an almost-sure limit $\dot f$, and [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem) gives [L1 convergence](../../../convergence-of-random-variables.md#convergence-in-l1). Define $\dot f=0$ on the null exceptional set and at the endpoint. This gives a [measurable](../../../measure-theory.md#measurability) representative with $|\dot f|\leq L$ everywhere.

If $a,b$ are [dyadic rationals](../../../arithmetic.md#dyadic-rational), then for every sufficiently fine grid the integral telescopes:

$$
\int_a^b X_n(x)\,dx=\sum_{[u,v)\subset[a,b)}\bigl(f(v)-f(u)\bigr)=f(b)-f(a).
$$

Pass to the limit by [L1 convergence](../../../convergence-of-random-variables.md#convergence-in-l1). For arbitrary endpoints choose dyadic $a_j\to a$, $b_j\to b$ with $a_j\leq b_j$. The error in the integrals is at most $L(|a_j-a|+|b_j-b|)$, and [Lipschitz continuity](../../../real-analysis.md#lipschitz-continuity) controls the error in the endpoint values by the same expression. Therefore

$$
\boxed{\int_a^b\dot f(x)\,dx=f(b)-f(a)\quad(0\leq a\leq b\leq1),\qquad\|\dot f\|_\infty\leq L.}
$$

This constructs the bounded integral density directly, without assuming in advance that a [Lipschitz function](../../../real-analysis.md#lipschitz-continuity) has an [almost everywhere](../../../measure-theory.md#almost-everywhere) derivative.

## 3

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

For each sample point put $A_n=\max_{0\leq k<2^n}|X_{(k+1)2^{-n}}-X_{k2^{-n}}|$. First take $s<t$ in the [dyadic rationals](../../../arithmetic.md#dyadic-rational), set $h=t-s$, and choose $N\geq0$ with $2^{-N}\leq h<2^{1-N}$. The left grid approximations $s_N=2^{-N}\lfloor2^Ns\rfloor$ and $t_N=2^{-N}\lfloor2^Nt\rfloor$ are at most two grid steps apart, so $|X_{t_N}-X_{s_N}|\leq2A_N$.

For either endpoint $r$, successive left approximations $r_n,r_{n+1}$ are equal or one step apart on the level-$(n+1)$ grid. Since $r$ is dyadic these approximations eventually equal $r$ exactly. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) therefore gives

$$
|X_t-X_s|\leq2\sum_{n\geq N}A_n
\leq2^{-N\alpha}\,2\sum_{n\geq N}2^{n\alpha}A_n
\leq h^\alpha K_\alpha.
$$

The second inequality is valid also for $\alpha=0$. Thus **the required bound holds simultaneously for every dyadic pair** whenever $K_\alpha$ is finite; if it is infinite the inequality holds in the extended sense. For $s=t$ the left side is zero. This is [dyadic increment chaining](../../../stochastic-process.md#dyadic-increment-chaining), with the stated constant two.

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

For a maximum of finitely many nonnegative quantities, its $p$th power is at most the sum of their $p$th powers. Hence the increment assumption gives

$$
\mathbb EA_n^p\leq\sum_{k=0}^{2^n-1}\mathbb E|X_{(k+1)2^{-n}}-X_{k2^{-n}}|^p
\leq C^p2^{n(1-p\beta)},\qquad
\|A_n\|_p\leq C2^{-n(\beta-1/p)}.
$$

By the [triangle inequality](../../../topological-analysis.md#triangle-inequality) in the [Lp norm](../../../real-analysis.md#lp-norm), the partial sums defining $K_\alpha$ have norms bounded by a geometric series. [Monotone convergence](../../../measure-theory.md#monotone-convergence-theorem) of their $p$th powers gives

$$
\boxed{\|K_\alpha\|_p\leq\frac{2C}{1-2^{-(\beta-1/p-\alpha)}}<\infty.}
$$

In particular $K_\alpha$ is finite [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), so the preceding pathwise estimate has a common probability-one domain for all dyadic pairs.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

First construct a centred [Gaussian process](../../../stochastic-process.md#gaussian-process) on the countable dyadic set with [covariance function](../../../stochastic-process.md#covariance-function) $\mathbb E(B_sB_t)=\min(s,t)$. These consistent finite-dimensional [normal distributions](../../../probability-theory.md#normal-distribution) exist because, for coefficients $a_j$,

$$
\sum_{i,j}a_ia_j\min(t_i,t_j)=\int_0^1\left(\sum_ja_j\mathbf1_{\{u\leq t_j\}}\right)^2du\geq0;
$$

the [Kolmogorov extension theorem](../../../stochastic-process.md#kolmogorov-extension-theorem) realizes them on one [probability space](../../../probability-theory.md#probability-space). Every increment has the [normal distribution](../../../probability-theory.md#normal-distribution) $N(0,|t-s|)$, so for every finite $p\geq1$,

$$
\|B_t-B_s\|_p=(\mathbb E|Z|^p)^{1/p}|t-s|^{1/2}.
$$

Use the preceding estimate with $\beta=1/2$, $p>2$ and $0<\alpha<1/2-1/p$. It yields an [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) [Hölder continuous](../../../sobolev-space.md#holder-condition) extension from the dense dyadic set to $[0,1]$. Approximate arbitrary times by dyadic times; continuity of the paths and of the Gaussian [covariance function](../../../stochastic-process.md#covariance-function) preserves all finite-dimensional laws. Disjoint increments are jointly Gaussian with zero cross-covariances, hence [independent](../../../random-variable.md#independent-random-variables), with the required variances. Together with $B_0=0$ and continuity, this constructs [Brownian motion](../../../brownian-motion.md).

For any $\alpha<1/2$, choose $p$ large enough. Taking a countable increasing sequence of exponents tending to $1/2$ gives **simultaneous Hölder regularity of every order $\alpha<1/2$** on a common probability-one set; the same argument on each compact time interval gives local [Brownian Hölder regularity](../../../brownian-motion.md#brownian-holder-regularity). This method does not give the endpoint exponent. In fact that endpoint fails: if a path had a finite $1/2$-[Hölder seminorm](../../../sobolev-space.md#holder-seminorm) $K$, all its $2^n$ adjacent normalized increments at level $n$ would have magnitude at most $K$. These are [independent](../../../random-variable.md#independent-random-variables) standard [normal random variables](../../../probability-theory.md#gaussian-random-variable), so for a fixed integer $m$ the probability that their maximum is at most $m$ is $\mathbb P(|Z|\leq m)^{2^n}\to0$. The event of a finite $K$ is contained in the union over $m$ of events with this bound at every level, each of probability zero. Thus **Brownian paths are not $1/2$-Hölder continuous on $[0,1]$ almost surely**.

## 4

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Write $u(z)=|z|^{2-d}$. For a radial function $r^{2-d}$, the [Laplacian](../../../calculus.md#laplacian) is

$$
u''(r)+\frac{d-1}{r}u'(r)=(2-d)(1-d)r^{-d}+(d-1)(2-d)r^{-d}=0.
$$

Thus $u$ is a [harmonic function](../../../partial-differential-equation.md#harmonic-function) off zero. Fix $R>|x|$ and stop [Brownian motion](../../../brownian-motion.md) when it reaches either sphere of radius $\varepsilon$ or $R$, at time $S_R$. This exit time is finite: stopping the [martingale](../../../martingale.md) $|B_t|^2-dt$ at $S_R\wedge t$ yields $d\mathbb E(S_R\wedge t)\leq R^2-|x|^2$, and [monotone convergence](../../../measure-theory.md#monotone-convergence-theorem) applies. By [Itô's formula](../../../stochastic-calculus.md#ito-s-lemma), $u(B_{t\wedge S_R})$ is a bounded [martingale](../../../martingale.md). [Optional stopping](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) and [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem) therefore give

$$
u(x)=q_R\varepsilon^{2-d}+(1-q_R)R^{2-d},\qquad
q_R=\mathbb P_x(T_\varepsilon<T_R)=\frac{|x|^{2-d}-R^{2-d}}{\varepsilon^{2-d}-R^{2-d}}.
$$

The events $\{T_\varepsilon<T_R\}$ increase to $\{T_\varepsilon<\infty\}$ as $R\to\infty$: a continuous path up to any finite hitting time is bounded. Since $d\geq3$, $R^{2-d}\to0$, proving the [Brownian hitting probability of a ball](../../../brownian-motion.md#brownian-hitting-probability-of-a-ball)

$$
\boxed{\mathbb P_x(T_\varepsilon<\infty)=(\varepsilon/|x|)^{d-2}.}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

To keep the normalization visible, denote the integral defining the printed constant by $A_d$. Substituting $r=|y|^2/(2s)$ gives, for $y\ne0$,

$$
\int_0^\infty p(s,0,y)\,ds=A_d|y|^{2-d},\qquad
A_d=\frac{\Gamma(d/2-1)}{2\pi^{d/2}}.
$$

This is the [Newtonian potential of the Brownian heat kernel](../../../diffusion-equation.md#newtonian-potential-of-the-brownian-heat-kernel). The singularity at zero is locally integrable in dimension $d$, since its radial integral behaves like $\int_0^1r^{2-d}r^{d-1}dr=1/2$. All integrands are nonnegative, so [Tonelli's theorem](../../../measure-theory.md#tonelli-theorem) permits both orders of integration.

Integrating in $s$ first gives

$$
I=A_d\int_{\mathbb R^d}p(t,x,y)|y|^{2-d}\,dy.
$$

Integrating in $y$ first uses the [Gaussian heat kernel](../../../diffusion-equation.md#gaussian-heat-kernel) [convolution](../../../fourier-analysis.md#convolution). Completing the square in $|y-x|^2/t+|y|^2/s$ gives

$$
\int_{\mathbb R^d}p(t,x,y)p(s,0,y)\,dy
=(2\pi(t+s))^{-d/2}e^{-|x|^2/(2(t+s))}=p(t+s,0,x).
$$

Consequently $I=\int_t^\infty p(r,0,x)dr$, and the actual identity is

$$
\boxed{\int_{\mathbb R^d}p(t,x,y)|y|^{2-d}\,dy
=A_d^{-1}\int_t^\infty p(r,0,x)\,dr.}
$$

The original PDF uses $A_d$ rather than $A_d^{-1}$ as the multiplier while defining its constant to equal $A_d$. That formula is false. For example $A_3=1/(2\pi)$, so the required multiplier in dimension three is $2\pi$. Equivalently, as $t\downarrow0$ at $x\ne0$, the left side tends to $|x|^{2-d}$, whereas the printed right side tends to $A_d^2|x|^{2-d}$. One can retain the printed form only by defining its multiplier as $c_d=A_d^{-1}$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Continue with $A_d$ equal to the integral defined in the PDF and $u(z)=|z|^{2-d}$. Until the [Brownian motion](../../../brownian-motion.md) hits the radius-$\varepsilon$ ball, $u(B_s)$ is a bounded [local martingale](../../../martingale.md#local-martingale), hence a true [martingale](../../../martingale.md). At the finite [stopping time](../../../martingale.md#stopping-time) $t\wedge T_\varepsilon$, [optional stopping](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) gives

$$
u(x)=\varepsilon^{2-d}\mathbb P_x(T_\varepsilon\leq t)+\mathbb E_x[u(B_t);T_\varepsilon>t].
$$

Rearranging,

$$
\varepsilon^{2-d}\mathbb P_x(T_\varepsilon\leq t)
=u(x)-\mathbb E_xu(B_t)+\mathbb E_x[u(B_t);T_\varepsilon\leq t].
$$

The fixed random variable $u(B_t)$ is integrable by the [Gaussian heat kernel](../../../diffusion-equation.md#gaussian-heat-kernel) and the local-integrability calculation above. Also $\mathbb P_x(T_\varepsilon\leq t)\leq(\varepsilon/|x|)^{d-2}\to0$. For any $R>0$, the final [expectation](../../../probability-theory.md#expected-value) is at most

$$
\mathbb E_x[u(B_t);u(B_t)>R]+R\mathbb P_x(T_\varepsilon\leq t).
$$

First send $\varepsilon\downarrow0$, then $R\to\infty$, proving that it vanishes. The identities from part (b) give

$$
u(x)=A_d^{-1}\int_0^\infty p(s,0,x)ds,\qquad
\mathbb E_xu(B_t)=A_d^{-1}\int_t^\infty p(s,0,x)ds.
$$

Subtracting yields the [small-ball Brownian hitting asymptotic](../../../brownian-motion.md#small-ball-brownian-hitting-asymptotic)

$$
\boxed{\lim_{\varepsilon\downarrow0}\varepsilon^{2-d}\mathbb P_x(T_\varepsilon\leq t)
=A_d^{-1}\int_0^t p(s,0,x)\,ds.}
$$

Thus the constant in this printed limit requires exactly the same reciprocal correction as in part (b). For $d=3$ the multiplier is $2\pi$, not $1/(2\pi)$. The argument proves the corrected finite-time limit directly, rather than inferring it from the eventual hitting probability alone.

## 5

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Let $R=|U|$. Uniform volume measure on the unit ball gives $\mathbb P(R\leq r)=r^n$, $0\leq r\leq1$, hence radius density $nr^{n-1}$. Conditional on $R=r>0$, [independence](../../../random-variable.md#independent-random-variables) leaves $W$ a standard [Brownian motion](../../../brownian-motion.md). Its exit time from the radius-$r$ ball is finite: applying [optional stopping](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) to $|W_t|^2-nt$ stopped at that exit and then letting $t\to\infty$ gives $\mathbb E\tau_r=r^2/n$.

The [probability law](../../../probability-theory.md#probability-distribution) of the exit point is invariant under every [orthogonal transformation](../../../linear-algebra.md#orthogonal-transformation), because both [Brownian motion](../../../brownian-motion.md) and the centred sphere are invariant under those transformations. The unique invariant probability on that sphere is normalized surface measure; for $n=1$ it is the equally weighted pair $\{-r,r\}$. This is also the conditional angular law of $U$ given $|U|=r$. Mixing these identical conditional laws against $nr^{n-1}dr$ proves the [uniform ball sampling by Brownian stopping](../../../brownian-motion.md#uniform-ball-sampling-by-brownian-stopping) identity

$$
\boxed{W_T\stackrel{d}=U.}
$$

The event $R=0$ has probability zero and causes no difficulty. [Independence](../../../random-variable.md#independent-random-variables) of $R$ permits its value to be included in the initial [filtration](../../../stochastic-process.md#filtration-probability-theory), making $T$ a [stopping time](../../../martingale.md#stopping-time).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Allow $g_D$ to take the value $+\infty$. Fix a closed ball $\overline{B(z,r)}\subset D$, independently choose a radius $R$ with density $ns^{n-1}/r^n$ on $(0,r)$, and let $S$ be the first time the [Brownian motion](../../../brownian-motion.md) from $z$ reaches that radius. Conditional on $R=s$, the [Strong Markov property](../../../markov-process.md#strong-markov-property) at $S$ decomposes the remaining [Brownian exit time](../../../brownian-motion.md#brownian-exit-time) from $D$. Since $S<T_D$ and the conditional exit time has mean $s^2/n$, [Tonelli's theorem](../../../measure-theory.md#tonelli-theorem) and part (a) give the [Brownian exit-time ball averaging identity](../../../brownian-motion.md#brownian-exit-time-ball-averaging-identity)

$$
g_D(z)=\mathbb E_zS+\mathbb E_zg_D(W_S)
=\frac{r^2}{n+2}+\frac1{|B(z,r)|}\int_{B(z,r)}g_D(w)\,dw.
$$

This identity is valid in the extended nonnegative reals; no finiteness was assumed to derive it.

If $g_D(z)<\infty$, the integral over $B(z,r)$ is finite. For any $y\in B(z,r)$ choose $\rho>0$ with $\overline{B(y,\rho)}\subset B(z,r)$. The same identity at $y$ has a finite right side because its integral is over a subset of the integrable ball. Thus $g_D(y)<\infty$. The set $F=\{z\in D:g_D(z)<\infty\}$ is therefore open relative to $D$.

It is also relatively closed. If $z_j\in F$ converges to $y\in D$, choose $r>0$ with $\overline{B(y,3r)}\subset D$. For large $j$, $|z_j-y|<r$, and $\overline{B(z_j,2r)}\subset D$. The preceding argument shows that every point in $B(z_j,2r)$, including $y$, belongs to $F$. Hence $F$ is closed in $D$. Since $F$ is nonempty and $D$ is [connected](../../../geometry-and-topology.md#connected-space), **$g_D(y)<\infty$ for every $y\in D$**. This proves [finiteness propagation of Brownian mean exit times](../../../brownian-motion.md#finiteness-propagation-of-brownian-mean-exit-times) without assuming beforehand that $g_D$ solves a smooth [Poisson equation](../../../partial-differential-equation.md#poisson-equation).

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Start at $x=(x_1,\ldots,x_n)$ with all $x_i>0$, and let $\tau_i$ be the first zero of the $i$th coordinate. The orthant exit time is $T=\min_i\tau_i$. The coordinate processes are [independent](../../../random-variable.md#independent-random-variables), so

$$
\mathbb P_x(T>t)=\prod_{i=1}^n\mathbb P_{x_i}(\tau_i>t)
=\prod_{i=1}^n\left[2\Phi(x_i/\sqrt t)-1\right].
$$

Here the [Brownian reflection principle](../../../brownian-motion.md#reflection-principle-wiener-process) gives $\mathbb P_a(\tau\leq t)=2\mathbb P(B_t\leq-a)$; $\Phi$ is the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution) function. Since $\Phi(z)-1/2=z/\sqrt{2\pi}+o(z)$ as $z\to0$,

$$
\mathbb P_x(T>t)\sim(2/\pi)^{n/2}(x_1\cdots x_n)t^{-n/2}\quad(t\to\infty).
$$

The [tail integral formula for expectation](../../../probability-theory.md#tail-integral-formula-for-expectation), $\mathbb E_xT=\int_0^\infty\mathbb P_x(T>t)dt$, has a bounded integrand on $(0,1)$ and converges at infinity exactly when $n/2>1$. Therefore the [Brownian exit-time expectation in an orthant](../../../brownian-motion.md#brownian-exit-time-expectation-in-an-orthant) gives

$$
\boxed{g_{D_1}=\infty,\qquad g_{D_2}=\infty,\qquad g_{D_3}<\infty\text{ everywhere in }D_3.}
$$

The divergence for $n=2$ is logarithmic; almost-sure finiteness of the exit time does not imply a finite [expectation](../../../probability-theory.md#expected-value).

## 6

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

For $0<\delta<1$, define the compensated small-jump [Poisson integral](../../../partial-differential-equation.md#poisson-integral)

$$
Y_t^\delta=\int_{(0,t]\times\{\delta<|y|\leq1\}}y\,(\mu-\nu)(dy,ds).
$$

This is an ordinary compensated finite-intensity sum. [Independent](../../../random-variable.md#independent-random-variables) [Poisson random variables](../../../discrete-probability-distribution.md#poisson-distribution) give mean zero and the [L2 construction of compensated Poisson integrals](../../../probability-theory.md#l2-construction-of-compensated-poisson-integrals) gives, for $0<\eta<\delta$,

$$
\mathbb E|Y_t^\eta-Y_t^\delta|^2=t\int_{\{\eta<|y|\leq\delta\}}y^2K(dy)=2ct(\delta-\eta).
$$

Thus $Y_t^\delta$ is [Cauchy](../../../real-analysis.md#cauchy-sequence) in [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space) as $\delta\downarrow0$, defining the first integral. It is not the difference of two separately convergent integrals. On a compact time interval $[0,L]$, the [Doob L2 maximal inequality](../../../martingale.md#doob-l2-maximal-inequality) bounds the squared supremum of the same difference by $8cL(\delta-\eta)$. Hence the truncated [martingales](../../../martingale.md) are Cauchy in the expected squared supremum norm. A sufficiently rapidly decreasing sequence of cutoffs converges uniformly [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence); its limit has [càdlàg](../../../calculus.md#cadlag) paths, so the construction also supplies a consistent process.

For large jumps, $K(\{|y|>1\})=2c<\infty$. There are only finitely many such atoms before any fixed time, [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), and each atom has a finite mark. The uncompensated large-jump integral is therefore a finite random sum, even though its absolute first moment is infinite. The two terms are well-defined for these different reasons.

There is also a literal signed-integral defect in the PDF: $\int yK(dy)$ on either symmetric region is not $+\infty$. Its positive and negative parts both have infinite mass, so the ordinary signed [Lebesgue integral](../../../measure-theory.md#lebesgue-integral) is undefined. The correct divergence statement is

$$
\int_{0<|y|\leq1}|y|K(dy)=\int_{|y|>1}|y|K(dy)=\infty.
$$

A symmetric principal value may be zero, but is not an ordinary signed integral. **Square-integrable compensation defines the small jumps; finite activity defines the large jumps.**

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

For a finite-intensity [Poisson random measure](../../../probability-theory.md#poisson-random-measure), [independence](../../../random-variable.md#independent-random-variables) of counts gives the exponential [characteristic function](../../../probability-theory.md#characteristic-function) formula. Apply it to the cutoff construction from part (a), including the deterministic compensation, and pass to the [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space) limit of the small jumps. The compensated integrand is $O(y^2)$ at zero and bounded on the large-jump region, so its integral converges absolutely:

$$
\mathbb E e^{iuX_t}=\exp\left\{t\int_{\mathbb R\setminus\{0\}}\left(e^{iuy}-1-iuy\mathbf1_{\{|y|\leq1\}}\right)c|y|^{-2}dy\right\}.
$$

Symmetry makes the absolutely integrable imaginary part zero. Substituting $z=|u|y$ in the real part and using the specified normalization gives

$$
2ct\int_0^\infty\frac{\cos(uy)-1}{y^2}dy
=-2ct|u|\int_0^\infty\frac{1-\cos z}{z^2}dz=-t|u|.
$$

Thus **$\mathbb E e^{iuX_1}=e^{-|u|}$**, and this construction is the standard [Cauchy process](../../../stochastic-process.md#cauchy-process). To calculate the density, its integrable [characteristic function](../../../probability-theory.md#characteristic-function) permits [Fourier inversion](../../../fourier-analysis.md#fourier-inversion-theorem):

$$
f_{X_1}(x)=\frac1{2\pi}\int_{\mathbb R}e^{-|u|}e^{-iux}du
=\frac1\pi\operatorname{Re}\int_0^\infty e^{-(1+ix)u}du
=\boxed{\frac1{\pi(1+x^2)}}.
$$

This is the standard [Cauchy distribution](../../../probability-theory.md#cauchy-distribution). The normalization also gives $c=1/\pi$: integration by parts turns $\int_0^\infty(1-\cos z)z^{-2}dz$ into $\int_0^\infty\sin z\,dz/z=\pi/2$. For completeness, with exponential damping the latter integral equals $\arctan(1/\eta)$, because its derivative in frequency $b$ is $\int_0^\infty e^{-\eta z}\cos(bz)dz=\eta/(\eta^2+b^2)$ and its value at $b=0$ is zero. Let $\eta\downarrow0$; integration by parts bounds the undamped and damped tails uniformly by a constant divided by the lower cutoff, justifying the limit.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Disjoint time strips of the [Poisson random measure](../../../probability-theory.md#poisson-random-measure) are [independent](../../../random-variable.md#independent-random-variables), and its intensity is translation invariant in time. The construction and its limits therefore give [independent increments](../../../stochastic-process.md#independent-increments) and [stationary increments](../../../stochastic-process.md#stationary-increments), with

$$
\mathbb E e^{iu(X_t-X_s)}=e^{-(t-s)|u|}\qquad(0\leq s<t).
$$

For the scaling actually printed in the original PDF,

$$
\mathbb E e^{iu\alpha X_{\alpha t}}=e^{-\alpha^2t|u|}.
$$

For example, $\alpha=2$, $t=1$, $u=1$ gives $e^{-4}$ rather than $e^{-1}$. Thus **the requested equality of process laws is false unless $\alpha=1$**.

The intended [self-similarity of a Cauchy process](../../../stochastic-process.md#self-similarity-of-a-cauchy-process) rescales space and time in opposite directions:

$$
\boxed{\left(\alpha^{-1}X_{\alpha t}\right)_{t\geq0}\stackrel{d}=(X_t)_{t\geq0}}
\qquad\text{or equivalently}\qquad
\boxed{\left(\alpha X_{t/\alpha}\right)_{t\geq0}\stackrel{d}=(X_t)_{t\geq0}}.
$$

Indeed, for $0\leq s<t$,

$$
\mathbb E\exp\left[iu\alpha^{-1}(X_{\alpha t}-X_{\alpha s})\right]
=\exp\left[-\alpha(t-s)|u|/\alpha\right]=e^{-(t-s)|u|}.
$$

The transformed process retains [independent increments](../../../stochastic-process.md#independent-increments). For any ordered times, the joint [characteristic function](../../../probability-theory.md#characteristic-function) of its successive increments is therefore the same product as for $X$; cumulative summation proves equality of all [finite-dimensional distributions](../../../stochastic-process.md#finite-dimensional-distribution). Both constructions have [càdlàg](../../../calculus.md#cadlag) paths, so these distributions also determine their laws on the usual [path space](../../../geometry-and-topology.md#path-space). This derives the corrected invariance and explicitly diagnoses the false printed assertion.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
