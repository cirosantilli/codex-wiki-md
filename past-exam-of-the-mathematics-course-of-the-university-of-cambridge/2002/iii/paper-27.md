# Paper 27

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper27.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper27.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)

## 1

↑ **Parent:** [Paper 27](paper-27.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use the exponent convention $\mathbb E e^{iuX_t}=e^{t\psi(u)}$. A real [Lévy process](../../../stochastic-process.md#levy-process) starts at $0$, has [stationary increments](../../../stochastic-process.md#stationary-increments) and [independent increments](../../../stochastic-process.md#independent-increments), is [stochastically continuous](../../../stochastic-process.md#stochastic-continuity), and is taken in its [càdlàg](../../../calculus.md#cadlag) version. Its [characteristic exponent of a Lévy process](../../../stochastic-process.md#characteristic-exponent-of-a-levy-process) satisfies $\psi(0)=0$ and is continuous. This convention has the opposite sign from the alternative $e^{-t\Psi(u)}$, so $\psi=-\Psi$.

For real $u$, the [exponential martingale of a Lévy process](../../../stochastic-process.md#exponential-martingale-of-a-levy-process) is integrable because $|M_t^u|=e^{-t\operatorname{Re}\psi(u)}$ is deterministic and finite. For $s\le t$, its [conditional expectation](../../../measure-theory.md#conditional-expectation) with respect to the natural [filtration](../../../stochastic-process.md#filtration-probability-theory) is

$$
\mathbb E[M_t^u\mid\mathcal F_s]
=e^{iuX_s-t\psi(u)}\mathbb E e^{iu(X_t-X_s)}
=e^{iuX_s-t\psi(u)}e^{(t-s)\psi(u)}=M_s^u.
$$

The second equality uses both [independent increments](../../../stochastic-process.md#independent-increments) and [stationary increments](../../../stochastic-process.md#stationary-increments). Thus this is a complex [martingale](../../../martingale.md), meaning that its real and imaginary parts are [martingales](../../../martingale.md).

A [probability distribution](../../../probability-theory.md#probability-distribution) is an [infinitely divisible distribution](../../../probability-theory.md#infinite-divisibility-probability) when, for every positive integer $n$, it is the distribution of a sum of $n$ [independent and identically distributed](../../../random-variable.md#independent-and-identically-distributed-random-variables) [random variables](../../../random-variable.md). Their common distribution is allowed to depend on $n$. For a [Lévy process](../../../stochastic-process.md#levy-process),

$$
X_1=\sum_{j=1}^n\bigl(X_{j/n}-X_{(j-1)/n}\bigr),
$$

and these summands are [independent](../../../random-variable.md#independent-random-variables) with the common law of $X_{1/n}$. This proves the required [infinite divisibility](../../../probability-theory.md#infinite-divisibility-probability) directly.

The [Lévy–Khintchine theorem](../../../stochastic-process.md#levy-khintchine-formula) states that a real [infinitely divisible distribution](../../../probability-theory.md#infinite-divisibility-probability) has [characteristic function](../../../probability-theory.md#characteristic-function) $e^{\psi(u)}$, where, for a unique triplet with the following fixed truncation,

$$
\boxed{\psi(u)=ibu-\frac a2u^2+\int_{\mathbb R\setminus\{0\}}
\bigl(e^{iuy}-1-iuy\mathbf1_{\{|y|<1\}}\bigr)K(dy),}
$$

with $b\in\mathbb R$, $a\ge0$, $K$ a positive measure, $K(\{0\})=0$, and $\int(1\wedge y^2)K(dy)<\infty$. Conversely every such triplet gives an [infinitely divisible distribution](../../../probability-theory.md#infinite-divisibility-probability) and a [Lévy process](../../../stochastic-process.md#levy-process), unique in law, whose time-$t$ [characteristic function](../../../probability-theory.md#characteristic-function) is $e^{t\psi(u)}$. The [Lévy measure](../../../stochastic-process.md#levy-measure) $K$ need not be finite near zero. [Taylor expansion](../../../calculus.md#taylor-expansion) makes the compensated integrand $O(y^2)$ there, while the measure is finite away from zero, so the integral is well defined. The drift parameter depends on the truncation: using $|y|\le1$ instead can alter $b$ by the contribution of atoms at $\pm1$. Here $a$ denotes [Gaussian](../../../probability-theory.md#normal-distribution) [variance](../../../variance.md), not drift.

We now prove that continuity forces $K=0$, using the suggested truncation rather than merely quoting a path classification. For $\varepsilon>0$, $\lambda_\varepsilon=K(|y|\ge\varepsilon)$ is finite. The truncated exponent is that of the [Compound Poisson process](../../../stochastic-process.md#compound-poisson-process)

$$
Y_t^\varepsilon=\sum_{j=1}^{N_t}J_j-t\int_{\varepsilon\le|y|<1}yK(dy),
$$

where $N$ has rate $\lambda_\varepsilon$ and the marks have law $K(dy)\mathbf1_{\{|y|\ge\varepsilon\}}/\lambda_\varepsilon$ when the rate is positive. The remaining exponent $\psi-\psi_\varepsilon$ also has an admissible [Lévy–Khintchine formula](../../../stochastic-process.md#levy-khintchine-formula) triplet. Hence construct independently a [Lévy process](../../../stochastic-process.md#levy-process) $Z^\varepsilon$ with that exponent. The sum $Y^\varepsilon+Z^\varepsilon$ has the same [finite-dimensional distributions](../../../stochastic-process.md#finite-dimensional-distribution) as $X$, and hence the same law on [càdlàg](../../../calculus.md#cadlag) path space. Continuity is therefore an almost-sure property of the sum if it is one of $X$.

But [independent compound Poisson jumps cannot cancel](../../../stochastic-process.md#independent-compound-poisson-jumps-cannot-cancel): conditional on the path of $Z^\varepsilon$, its jump times are [countable](../../../set-theory.md#countable-set); the [independent](../../../random-variable.md#independent-random-variables) Poisson jump times have continuous distributions and avoid them almost surely. At each jump of $Y^\varepsilon$, the sum has the same nonzero jump, of size at least $\varepsilon$. If $\lambda_\varepsilon>0$, there is positive probability of such a jump on any fixed positive-length time interval, contradicting almost-sure continuity. Thus $K(|y|\ge\varepsilon)=0$ for every $\varepsilon>0$, and taking $\varepsilon=1/n$ gives $K=0$.

The [characteristic function](../../../probability-theory.md#characteristic-function) is now $\exp[t(ibu-au^2/2)]$. If $a>0$, the process $B_t=(X_t-bt)/\sqrt a$ has continuous paths and [independent](../../../random-variable.md#independent-random-variables) centered [normal](../../../probability-theory.md#normal-distribution) increments of [variance](../../../variance.md) $t-s$, so it is standard [Brownian motion](../../../brownian-motion.md) on the original probability space. If $a=0$, the increments are deterministic, and continuity together with equality at all rational times gives $X_t=bt$ simultaneously for all $t$ almost surely. A [Brownian motion](../../../brownian-motion.md) on an enlarged space can be used in the zero-variance representation if necessary. Therefore

$$
\boxed{X_t=bt+\sqrt a\,B_t,\qquad a\ge0.}
$$

## 2

↑ **Parent:** [Paper 27](paper-27.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

In discrete time, the bounded-time [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) says that an integrable [supermartingale](../../../martingale.md#supermartingale) $X$ and bounded [stopping times](../../../martingale.md#stopping-time) $S\le T$ satisfy $\mathbb E[X_T\mid\mathcal F_S]\le X_S$. For a [martingale](../../../martingale.md) there is equality. The assertion at a possibly unbounded, almost-surely finite [stopping time](../../../martingale.md#stopping-time) $T$ also holds with $S=0$ if $\{X_{T\wedge n}:n\ge0\}$ is [uniformly integrable](../../../convergence-of-random-variables.md#uniform-integrability): then $X_T$ is integrable and $\mathbb EX_T\le\mathbb EX_0$, with equality for a [martingale](../../../martingale.md). Boundedness of $T$ or the stated integrability condition cannot in general be omitted.

For the increment hypothesis here, $\mathbb ET<\infty$ implies $T<\infty$ almost surely, and telescoping gives

$$
|X_{T\wedge n}|\le|X_0|+KT,\qquad |X_T|\le|X_0|+KT.
$$

The right-hand side is an [integrable random variable](../../../probability-theory.md#integrable-random-variable). Applying bounded-time [optional stopping](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) to $T\wedge n$ and then the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) proves

$$
\boxed{X_T\in L^1,\qquad \mathbb EX_T\le\mathbb EX_0.}
$$

This is [bounded-increment optional stopping with integrable time](../../../martingale.md#bounded-increment-optional-stopping-with-integrable-time); the same reasoning gives equality for a [martingale](../../../martingale.md).

Put $q=1-p$ and first assume $0<p<1$. Let $\tau$ be the first occurrence time of the specified seven-letter word. Its probability in a prescribed block is $r=p^4q^3>0$. Disjoint seven-flip blocks are [independent](../../../random-variable.md#independent-random-variables), and a match in one forces $\tau$ to have occurred by its end. Consequently $\mathbb P(\tau>7m)\le(1-r)^m$ and $\mathbb E\tau\le7/r<\infty$; this establishes the integrability needed for stopping before computing its value.

Start a new gambler with unit capital immediately before each flip. A gambler bets all current capital on the next required letter of the word, receives capital divided by $p$ for a correct head or by $q$ for a correct tail, and receives zero on failure. After completing all seven bets, the gambler retains the winnings without further betting. Each individual bet preserves its conditional expected capital. If $C_n$ is the total capital of all gamblers who have entered through flip $n$, then $C_n-n$ is a [martingale](../../../martingale.md).

At any time at most seven gamblers are still betting, and each one's capital is at most $L=1/(p^4q^3)$, since probabilities of shorter prefixes are at least the full-word probability. Completed winnings do not change. Thus the increments of $C_n-n$ have a deterministic bound, for example $14L+1$. The preceding optional-stopping argument therefore gives $\mathbb E(C_\tau-\tau)=0$.

At the first full match, no earlier gambler has completed the word. A surviving gambler who has placed $k$ successful bets corresponds to a suffix of the completed word which is also its length-$k$ prefix, namely a [border of a word](../../../foundations-of-mathematics.md#border-of-a-word). The only such lengths are $3$ and $7$: the shorter common string is HHT. Their capitals are $1/(p^2q)$ and $1/(p^4q^3)$, respectively. Hence $C_\tau$ is this deterministic sum and

$$
\boxed{\mathbb E\tau=\frac1{p^4(1-p)^3}+\frac1{p^2(1-p)}.}
$$

For a fair coin this is **136 flips**. This is a [waiting time for a word in independent nonuniform symbols](../../../mathematics.md#waiting-time-for-a-word-in-independent-nonuniform-symbols); the overlap contribution is essential. If $p=0$ or $p=1$, the word cannot occur because it contains both types of flip, so the expected waiting time is infinite.

## 3

↑ **Parent:** [Paper 27](paper-27.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For real $\lambda$, the [normal](../../../probability-theory.md#normal-distribution) moment-generating formula gives $\mathbb E e^{\lambda(B_t-B_s)}=e^{\lambda^2(t-s)/2}$. Using [independent increments](../../../stochastic-process.md#independent-increments) and conditioning on the Brownian [filtration](../../../stochastic-process.md#filtration-probability-theory),

$$
\mathbb E\left[e^{\lambda B_t-\lambda^2t/2}\mid\mathcal F_s\right]
=e^{\lambda B_s-\lambda^2t/2}e^{\lambda^2(t-s)/2}
=e^{\lambda B_s-\lambda^2s/2}.
$$

All terms are integrable by the same [normal](../../../probability-theory.md#normal-distribution) formula. Thus the displayed process is an [Exponential martingale for Brownian motion](../../../brownian-motion.md#exponential-martingale-for-brownian-motion).

For the interval exit time, we first show both almost-sure finiteness and finite expectation. On $\{T>n\}$, the position at time $n$ lies in $(-b,a)$. If $X_{n+1}-X_n\ge a+b$, the continuous path must exit by time $n+1$. This increment is [independent](../../../random-variable.md#independent-random-variables) of $\mathcal F_n$ and has law $N(\mu,1)$, so the conditional probability of this event is a fixed $c>0$. Therefore

$$
\mathbb P(T>n+1)\le(1-c)\mathbb P(T>n),
\qquad \mathbb P(T>n)\le(1-c)^n.
$$

This [geometric tail bound from a uniform escape probability](../../../martingale.md#geometric-tail-bound-from-a-uniform-escape-probability) implies $T<\infty$ almost surely and $\mathbb ET<\infty$.

Take $\lambda=-2\mu$. Then $e^{-2\mu X_t}=e^{-2\mu B_t-2\mu^2t}$ is the exponential [martingale](../../../martingale.md) just proved. Its stopped values lie between $e^{-2\mu a}$ and $e^{2\mu b}$. The [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) at $T\wedge t$, followed by bounded convergence, gives $\mathbb E e^{-2\mu X_T}=1$. With $v=\mathbb P(X_T=a)$ and the two possible boundary values,

$$
v e^{-2\mu a}+(1-v)e^{2\mu b}=1.
$$

Solving yields

$$
\boxed{\mathbb P(X_T=a)=\frac{1-e^{-2\mu b}}{1-e^{-2\mu(a+b)}}.}
$$

Next apply bounded-time [optional stopping](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) to $B_t$. Since $B_{T\wedge t}=X_{T\wedge t}-\mu(T\wedge t)$, we obtain $\mathbb EX_{T\wedge t}=\mu\mathbb E(T\wedge t)$. The stopped position is bounded, and the stopped time increases to an integrable $T$. Passing to the limit gives $\mu\mathbb ET=av-b(1-v)$. Therefore

$$
\boxed{\mathbb ET=\frac1\mu\left[(a+b)\frac{1-e^{-2\mu b}}{1-e^{-2\mu(a+b)}}-b\right].}
$$

As a check, letting $\mu\downarrow0$ gives the driftless formulas $v\to b/(a+b)$ and $\mathbb ET\to ab$. The expectation calculation uses a justified stopping limit, rather than assuming that [optional stopping](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) holds at every unbounded time.

## 4

↑ **Parent:** [Paper 27](paper-27.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Standard one-dimensional [Brownian motion](../../../brownian-motion.md) is a real process with $B_0=0$, continuous paths almost surely, and increments $B_t-B_s\sim N(0,t-s)$ [independent](../../../random-variable.md#independent-random-variables) of the past at time $s$, for $0\le s<t$. These conditions determine its entire [finite-dimensional distribution](../../../stochastic-process.md#finite-dimensional-distribution) family.

The [Wiener theorem](../../../brownian-motion.md#wiener-theorem) asserts that such a process exists, equivalently that there is a unique [Wiener measure](../../../brownian-motion.md#wiener-measure) on $C_0([0,\infty),\mathbb R)$ under which the coordinate process has these properties. To construct it, prescribe centered multivariate [normal](../../../probability-theory.md#normal-distribution) laws with [covariance](../../../variance.md#covariance) $\mathbb E B_sB_t=\min(s,t)$. This [covariance](../../../variance.md#covariance) is [positive semidefinite](../../../linear-algebra.md#positive-semidefinite-matrix) because

$$
\sum_{i,j}c_ic_j\min(t_i,t_j)=\int_0^\infty\left(\sum_i c_i\mathbf1_{[0,t_i]}(u)\right)^2du\ge0.
$$

The laws are consistent under removing coordinates, so the [Kolmogorov extension theorem](../../../stochastic-process.md#kolmogorov-extension-theorem) constructs the process. [Normal](../../../probability-theory.md#normal-distribution) increments have [fourth moment](../../../probability-theory.md#fourth-moment) $\mathbb E|B_t-B_s|^4=3|t-s|^2$. The [Kolmogorov continuity theorem](../../../stochastic-process.md#kolmogorov-continuity-theorem) therefore supplies a continuous modification, retaining all the prescribed finite-dimensional laws and hence the [independent](../../../random-variable.md#independent-random-variables) [normal](../../../probability-theory.md#normal-distribution) increments. Apply this on every compact time interval, taking consistent versions; continuity and equality at rational times make them agree on overlaps. The resulting law on continuous-path space is unique because evaluations at rational times generate its [Borel sigma-algebra](../../../measure-theory.md#borel-sigma-algebra). This is a proof sketch of the existence theorem, [independent](../../../random-variable.md#independent-random-variables) of the random-walk limit in Question 5.

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For every positive real $r$, a centered [normal](../../../probability-theory.md#normal-distribution) variable of [variance](../../../variance.md) $t-s$ has absolute $r$th moment $c_r|t-s|^{r/2}$, where $c_r=\mathbb E|N(0,1)|^r<\infty$. Fix $0<\alpha<1/2$ and choose $r$ large enough that $\alpha<1/2-1/r$. Then

$$
\mathbb E|B_t-B_s|^r=c_r|t-s|^{1+(r/2-1)}.
$$

The [Kolmogorov continuity theorem](../../../stochastic-process.md#kolmogorov-continuity-theorem) gives a modification with [Hölder continuity](../../../sobolev-space.md#holder-condition) of every exponent less than $(r/2-1)/r=1/2-1/r$, in particular exponent $\alpha$, on each compact interval. This modification and the given continuous [Brownian motion](../../../brownian-motion.md) agree almost surely at all rational times; continuity makes them agree everywhere simultaneously. Thus the property holds for the given trajectories, not just for another version.

Take a [countable](../../../set-theory.md#countable-set) increasing sequence of positive exponents approaching $1/2$, and intersect their probability-one events for every integer time horizon. [Hölder continuity](../../../sobolev-space.md#holder-condition) of a larger exponent implies that of every smaller positive exponent on a compact interval, after adjusting the constant. We have therefore proved the simultaneous assertion

$$
\boxed{\text{Almost surely, }B\text{ is locally }\alpha\text{-Hölder for every }0<\alpha<\tfrac12.}
$$

The compact-interval qualification matters: a single uniform Hölder constant on the entire half-line is not being asserted.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

We use [dyadic quadratic variation of Brownian motion](../../../stochastic-calculus.md#dyadic-quadratic-variation-of-brownian-motion). For fixed rational $0\le u<v$, set $\ell=v-u$ and let $Q_n$ be the sum of the squares of the $2^n$ [Brownian increments](../../../brownian-motion.md#brownian-increment) on its equal-length partition. [Independence](../../../random-variable.md#independent-random-variables) and the [normal](../../../probability-theory.md#normal-distribution) [fourth moment](../../../probability-theory.md#fourth-moment) give

$$
\mathbb EQ_n=\ell,\qquad \operatorname{Var}(Q_n)=2\ell^2\,2^{-n}.
$$

For every $\eta>0$, [Chebyshev's inequality](../../../probability-inequality.md#chebyshev-inequality) bounds $\mathbb P(|Q_n-\ell|>\eta)$ by $2\ell^2\eta^{-2}2^{-n}$, a summable sequence. The [Borel-Cantelli lemma](../../../probability-theory.md#borel-cantelli-lemmas) implies $Q_n\to\ell$ almost surely. Intersect over positive rational $\eta$ and all rational intervals to obtain one probability-one event on which every such interval has this positive quadratic-variation limit.

If a path were Hölder of exponent $\alpha>1/2$ on a nonempty open interval, choose a compact rational subinterval $[u,v]$ within it and a finite Hölder constant $C$ there. Every partition increment would have absolute value at most $C(\ell2^{-n})^\alpha$, so

$$
Q_n\le C^2\ell^{2\alpha}2^{n(1-2\alpha)}\longrightarrow0.
$$

This contradicts $Q_n\to\ell>0$. The same pathwise event excludes every exponent greater than $1/2$, without needing an uncountable intersection of events. Therefore

$$
\boxed{\text{Almost surely, no nonempty interval supports a Hölder exponent }>\tfrac12.}
$$

This is the [quadratic variation obstruction to Hölder regularity](../../../stochastic-calculus.md#quadratic-variation-obstruction-to-holder-regularity). It rules out a continuously differentiable trajectory on any interval, since a continuous derivative is bounded on smaller compact intervals and gives a [Lipschitz](../../../real-analysis.md#lipschitz-continuity) bound. By itself it does not rule out differentiability at an isolated point. The stronger [nowhere differentiability of Brownian motion](../../../brownian-motion.md#nowhere-differentiability-of-brownian-motion) can also be seen directly as follows.

On a mesh of width $h=2^{-n}$ in $[0,M]$, the probability that any specified three consecutive increments all have absolute value at most $Kh$ is at most $C K^3h^{3/2}$: each increment is $N(0,h)$ and the three are [independent](../../../random-variable.md#independent-random-variables). There are at most $M/h$ possible blocks, so the probability of any such block is at most $C M K^3h^{1/2}$, summable in $n$. By [Borel-Cantelli lemma](../../../probability-theory.md#borel-cantelli-lemmas), for every pair of positive integers $M,K$ there are eventually no such blocks. But a finite derivative at some time $t<M$ would imply $|B_s-B_t|\le C_t|s-t|$ near $t$. The three mesh increments beginning at the mesh point immediately to the left of $t$ would then all be at most $6C_th$ for all sufficiently fine meshes. Choosing an integer $K\ge6C_t$ contradicts the preceding event. Thus finite derivatives do not exist anywhere almost surely, including a finite right derivative at $0$. The Hölder estimates below $1/2$ express continuity with a roughness scale; they do not imply differentiability.

## 5

↑ **Parent:** [Paper 27](paper-27.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Write $m_l=\lfloor Nt_l\rfloor-\lfloor Nt_{l-1}\rfloor$ and $\phi(v)=\mathbb E e^{iv\xi}$. Since $\mathbb E\xi=0$ and $\mathbb E\xi^2=1$, the [characteristic function](../../../probability-theory.md#characteristic-function) expansion at zero is $\phi(v)=1-v^2/2+o(v^2)$. Indeed, $|e^{ix}-1-ix|\le x^2/2$ for real $x$, and $(e^{iv\xi}-1-iv\xi)/v^2\to-\xi^2/2$. The [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem), with dominating variable $\xi^2/2$, proves the expansion after taking expectations. Initially omit the endpoint interpolation terms. The integer-time increments involve disjoint sets of [independent](../../../random-variable.md#independent-random-variables) steps, so their joint [characteristic function](../../../probability-theory.md#characteristic-function) is

$$
\prod_{l=1}^k\phi(\lambda_l/\sqrt N)^{m_l}.
$$

Here $m_l/N\to t_l-t_{l-1}$. Taking the logarithm near $1$ gives

$$
\sum_lm_l\log\phi(\lambda_l/\sqrt N)
\longrightarrow-\frac12\sum_l\lambda_l^2(t_l-t_{l-1}).
$$

This proves the claimed limit for the integer-time approximation.

At a fixed time $t$, the omitted endpoint term is $R_N(t)=N^{-1/2}(Nt-\lfloor Nt\rfloor)\xi_{\lfloor Nt\rfloor+1}$, and $\mathbb E|R_N(t)|^2\le1/N$. A fixed linear combination of the errors in the $k$ increments therefore tends to zero in $L^1$, by the triangle inequality and [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality), even when two endpoint terms share a step. Since $|e^{ix}-e^{iy}|\le|x-y|$, restoring interpolation changes the joint [characteristic function](../../../probability-theory.md#characteristic-function) by a quantity tending to zero. Hence

$$
\boxed{\varphi^N_{t_1,\ldots,t_k}(\lambda_1,\ldots,\lambda_k)
\longrightarrow \exp\left(-\frac12\sum_{l=1}^k\lambda_l^2(t_l-t_{l-1})\right).}
$$

The limit is the joint [characteristic function](../../../probability-theory.md#characteristic-function) of [independent](../../../random-variable.md#independent-random-variables) centered [normal](../../../probability-theory.md#normal-distribution) increments with the indicated variances. By [Lévy continuity theorem](../../../probability-theory.md#levy-continuity-theorem), the increment vectors converge in distribution to [Brownian increment](../../../brownian-motion.md#brownian-increment) vectors. The value vector is obtained by the fixed invertible triangular map of cumulative sums; thus the [continuous mapping theorem](../../../convergence-of-random-variables.md#continuous-mapping-theorem) gives convergence of $(S_{t_1}^N,\ldots,S_{t_k}^N)$ to $(B_{t_1},\ldots,B_{t_k})$. This proves every required [finite-dimensional distribution](../../../stochastic-process.md#finite-dimensional-distribution) limit. The finite [fourth moment](../../../probability-theory.md#fourth-moment) is not needed for this part; it will give tightness in part (b).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

We prove [fourth-moment tightness of polygonal random walks](../../../convergence-of-random-variables.md#fourth-moment-tightness-of-polygonal-random-walks) uniformly, including intervals shorter than a mesh cell or crossing a mesh boundary. For $s<t$, let $c_j$ be the length of the overlap of $(Ns,Nt)$ with $(j-1,j)$. The interpolated increment is

$$
S_t^N-S_s^N=N^{-1/2}\sum_jc_j\xi_j,
\qquad 0\le c_j\le1,\qquad \sum_jc_j=N(t-s).
$$

Put $m_4=\mathbb E\xi^4<\infty$. Expanding the fourth power and using centered [independent](../../../random-variable.md#independent-random-variables) steps, only the terms with four equal indices or two equal pairs survive. Consequently

$$
\mathbb E|S_t^N-S_s^N|^4
=N^{-2}\left(m_4\sum_jc_j^4+6\sum_{i<j}c_i^2c_j^2\right)
=N^{-2}\left(3\left(\sum_jc_j^2\right)^2+(m_4-3)\sum_jc_j^4\right).
$$

If $m_4\le3$, the last correction is nonpositive. If $m_4>3$, use $\sum c_j^4\le(\sum c_j^2)^2$. In either case the expression is at most $\max(3,m_4)N^{-2}(\sum c_j^2)^2$. Since $c_j^2\le c_j$,

$$
\boxed{\mathbb E|S_t^N-S_s^N|^4\le\max(3,m_4)|t-s|^2,\quad\text{for all }N,s,t.}
$$

Also $S_0^N=0$ and the paths are continuous. The stated tightness criterion applies with $\gamma=4$, $\alpha=1$ and the displayed constant, so the laws $\mu_N$ are tight on $C_0([0,1],\mathbb R)$ with its uniform topology. Part (a) established all the Brownian [finite-dimensional distribution](../../../stochastic-process.md#finite-dimensional-distribution) limits. The supplied implication from tightness plus those limits now yields the [Donsker invariance principle](../../../convergence-of-random-variables.md#donsker-s-theorem):

$$
\boxed{\mu_N\Rightarrow\mu\quad\text{in }C([0,1],\mathbb R),}
$$

where $\mu$ is [Wiener measure](../../../brownian-motion.md#wiener-measure). No estimate restricted to grid endpoints would suffice by itself for the printed uniform criterion; the overlap coefficients handle every pair of times.

## 6

↑ **Parent:** [Paper 27](paper-27.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Write $Z_t=\langle\kappa_t\rangle$, where the angle brackets average only over walk paths, and use $\mathbb E$ only for the environment. Every nearest-neighbor path of length $t$ has probability $(2d)^{-t}$, so the finite path sum is exactly the walk expectation. It depends only on environment layers through time $t$, and hence is $\mathcal F_t$-measurable. Its factors lie in $[1-\varepsilon,1+\varepsilon]$, so $Z_t$ is positive and integrable at each fixed time.

For any fixed path through time $t+1$, the environment variable $h(t+1,\xi_{t+1})$ is [independent](../../../random-variable.md#independent-random-variables) of $\mathcal F_t$ and has [mean](../../../probability-theory.md#expected-value) zero. [Conditional expectation](../../../measure-theory.md#conditional-expectation) therefore removes its last factor. Summing over the $2d$ possible last steps of each length-$t$ path cancels the extra factor $2d$ in the path probability. Thus

$$
\boxed{\mathbb E[Z_{t+1}\mid\mathcal F_t]=Z_t,\qquad Z_0=1,\qquad \mathbb EZ_t=1.}
$$

This is the [positive random-environment path-weight martingale](../../../martingale.md#positive-random-environment-path-weight-martingale). It is nonnegative and bounded in $L^1$, so the [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem) gives a finite limit $\zeta\ge0$ almost surely. At this stage one can conclude $\mathbb E\zeta\le1$ by [Fatou's lemma](../../../measure-theory.md#fatou-s-lemma), but not yet equality; the second-moment bound in part (b) will prevent loss of [mean](../../../probability-theory.md#expected-value).

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

For a fixed environment, use two [independent](../../../random-variable.md#independent-random-variables) copies of the walk to express $Z_t^2=\langle\kappa_t^{(1)}\kappa_t^{(2)}\rangle$. The product is finite and nonnegative, so we can interchange the two expectations. At each time $j$, if the walks occupy different sites, the two environment signs are [independent](../../../random-variable.md#independent-random-variables) and their factors have product expectation $1$. If they coincide, both factors use the same sign and

$$
\mathbb E(1+\varepsilon h)^2=1+\varepsilon^2.
$$

Different time layers are [independent](../../../random-variable.md#independent-random-variables) even when a site is visited again. Therefore, with the simultaneous collision count $I_t=\sum_{j=1}^t\mathbf1_{\{\xi_j^{(1)}=\xi_j^{(2)}\}}$,

$$
\boxed{\mathbb EZ_t^2=\left\langle(1+\varepsilon^2)^{I_t}\right\rangle.}
$$

This is the [collision-count second moment for independent path weights](../../../martingale.md#collision-count-second-moment-for-independent-path-weights). It involves equal-time intersections, not arbitrary intersections of the two spatial ranges.

The difference walk $D_j=\xi_j^{(1)}-\xi_j^{(2)}$ has [independent](../../../random-variable.md#independent-random-variables) bounded increments symmetric about zero and a full-dimensional step distribution. It may hold at zero for one step; such a hold counts as a positive-time return. The allowed transience fact gives

$$
\rho=\mathbb P_0(D_j=0\text{ for some }j\ge1)<1.
$$

Moreover $\rho>0$ since the two first steps can be equal. Restarting the [independent increments](../../../stochastic-process.md#independent-increments) after every return to zero shows that the total positive-time return count $I_\infty$ has the zero-based [geometric distribution](../../../discrete-probability-distribution.md#geometric-distribution)

$$
\mathbb P(I_\infty=k)=(1-\rho)\rho^k,\quad k=0,1,2,\ldots.
$$

Indeed the probability of at least $k$ returns is $\rho^k$, and subtracting successive tails gives this law. Consequently, whenever $\rho(1+\varepsilon^2)<1$,

$$
\sup_t\mathbb EZ_t^2\le\left\langle(1+\varepsilon^2)^{I_\infty}\right\rangle
=\sum_{k=0}^\infty(1-\rho)[\rho(1+\varepsilon^2)]^k
=\frac{1-\rho}{1-\rho(1+\varepsilon^2)}<\infty.
$$

A sufficient small-noise condition is $0<\varepsilon<\min(1,\sqrt{(1-\rho)/\rho})$.

The [L2 martingale convergence theorem](../../../martingale.md#l2-martingale-convergence-theorem) now gives $Z_t\to\zeta$ in $L^2$ as well as almost surely. One can see the [mean](../../../probability-theory.md#expected-value) preservation directly: for $t\ge s$, the [martingale](../../../martingale.md) identity gives $\mathbb E(Z_t-Z_s)^2=\mathbb EZ_t^2-\mathbb EZ_s^2$. The [second moments](../../../probability-theory.md#second-moment) are increasing and bounded, so the sequence is Cauchy in $L^2$ and its limit is the already identified almost-sure limit. Thus

$$
\boxed{\mathbb E\zeta=\lim_t\mathbb EZ_t=1.}
$$

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

For each fixed $m\ge0$ and $T\ge m$, remove the first $m$ weight factors but retain the same walk law:

$$
Z_T^{(m)}=\left\langle\prod_{j=m+1}^T(1+\varepsilon h(j,\xi_j))\right\rangle.
$$

This quantity is measurable with respect to $\mathcal G_{m+1}=\sigma(h(j,x):j\ge m+1,x\in\mathbb Z^d)$, since the averaging over all walk positions is deterministic and involves no earlier environment variables. The bounds on each deleted factor give, pointwise for every environment,

$$
(1-\varepsilon)^mZ_T^{(m)}\le Z_T\le(1+\varepsilon)^mZ_T^{(m)}.
$$

Both constants are finite and strictly positive. Taking lower limits gives the exact identity of events

$$
\{\liminf_TZ_T=0\}=\{\liminf_TZ_T^{(m)}=0\}\in\mathcal G_{m+1}.
$$

There is no exceptional-set issue in this comparison. Choose the version of $\zeta$ to equal $\liminf_TZ_T$ when this is finite and to equal $1$ otherwise; it agrees with the almost-sure [martingale](../../../martingale.md) limit, and its zero event is precisely the left-hand event above. Since the identity holds for every $m$, $\{\zeta=0\}$ belongs to the printed [tail sigma-algebra](../../../probability-theory.md#tail-sigma-algebra) $\bigcap_{n\ge1}\mathcal G_n$. This proves the [tail event for a vanishing positive path-weight limit](../../../martingale.md#tail-event-for-a-vanishing-positive-path-weight-limit) without pretending that the whole value of $\zeta$ is tail-measurable.

The [independent](../../../random-variable.md#independent-random-variables) time layers of the environment are [independent](../../../random-variable.md#independent-random-variables) random vectors, so the [Kolmogorov zero-one law](../../../probability-theory.md#kolmogorov-s-zero-one-law) applies to their [tail sigma-algebra](../../../probability-theory.md#tail-sigma-algebra). It yields $\mathbb P(\zeta=0)\in\{0,1\}$. Under the small-noise condition from part (b), $\mathbb E\zeta=1$ and $\zeta\ge0$, so that probability cannot be $1$. Hence

$$
\boxed{\mathbb P(\zeta=0)=0,\qquad \zeta>0\text{ almost surely}.}
$$

The tail-event argument itself works for every $0<\varepsilon<1$; the deduction of positivity here uses the mean-one conclusion supplied by part (b).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
