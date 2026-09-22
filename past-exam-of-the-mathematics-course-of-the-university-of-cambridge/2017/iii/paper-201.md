# Paper 201

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_201.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_201.pdf)

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
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
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

Relative to a [probability space](../../../probability-theory.md#probability-space) $(\Omega,\mathcal F,\mathbb P)$ and a [filtration](../../../stochastic-process.md#filtration-probability-theory) $(\mathcal F_n)$, the real [stochastic process](../../../stochastic-process.md) $(M_n)$ is a [martingale](../../../martingale.md) if it is [adapted](../../../stochastic-process.md#adapted-process), each $M_n$ is an [integrable random variable](../../../probability-theory.md#integrable-random-variable), and

$$
\boxed{\mathbb E[M_{n+1}\mid\mathcal F_n]=M_n\quad\text{almost surely for every }n\geq0.}
$$

Here [adapted](../../../stochastic-process.md#adapted-process) means $M_n$ is $\mathcal F_n$-measurable, and integrability means $\mathbb E|M_n|<\infty$. By the [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation), the equivalent multi-step condition is $\mathbb E[M_j\mid\mathcal F_i]=M_i$ for all $i\leq j$. The [filtration](../../../stochastic-process.md#filtration-probability-theory) is part of the definition; specifying only the marginal means is insufficient.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The discrete-time [Doob L2 maximal inequality](../../../martingale.md#doob-l2-maximal-inequality) states that a [square-integrable](../../../measure-theory.md#square-integrable-function) [martingale](../../../martingale.md) satisfies

$$
\boxed{\mathbb E\!\left[\max_{0\leq k\leq n}|M_k|^2\right]\leq4\mathbb E|M_n|^2.}
$$

Equivalently, the [Lp norm](../../../real-analysis.md#lp-norm) of the maximum at $p=2$ is at most $2\|M_n\|_2$. The same assertion holds for a nonnegative [square-integrable](../../../measure-theory.md#square-integrable-function) [submartingale](../../../martingale.md#submartingale). No assumption $M_0=0$ is required; for a bound in terms of fluctuations from the initial value, apply it to $(M_k-M_0)$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Use the natural [filtration](../../../stochastic-process.md#filtration-probability-theory) $\mathcal F_k=\sigma(X_1,\ldots,X_k)$ and define $M_k=S_k-mk$. The increments $X_k-m$ are centered, independent, and square integrable, so their [conditional expectations](../../../measure-theory.md#conditional-expectation) given the past are zero. Thus $(M_k)$ is a [square-integrable](../../../measure-theory.md#square-integrable-function) [martingale](../../../martingale.md) with $M_0=0$. [Independence](../../../random-variable.md#independent-random-variables) gives

$$
\mathbb E|M_n|^2=\operatorname{Var}\!\left(\sum_{j=1}^n(X_j-m)\right)=n\sigma^2.
$$

Applying the [Doob L2 maximal inequality](../../../martingale.md#doob-l2-maximal-inequality) yields

$$
\boxed{\mathbb E\!\left[\max_{0\leq k\leq n}|S_k-mk|^2\right]\leq4n\sigma^2.}
$$

This includes $\sigma^2=0$, when every centered increment vanishes [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Put $M_k=S_k-mk$ as above. Centering the [linear interpolation](../../../function.md#linear-interpolation) also interpolates the centered values: for $u\in[0,1]$,

$$
S_{k+u}-m(k+u)=(1-u)M_k+uM_{k+1}.
$$

The absolute value of this convex combination is at most the larger endpoint absolute value. For every fixed $A>0$, part (c) therefore gives

$$
\mathbb E\!\left[\sup_{0\leq t\leq A}|S_t^{(N)}-mt|^2\right]
\leq \frac{4\sigma^2\lceil NA\rceil}{N^2}\longrightarrow0.
$$

Hence there is [uniform convergence on compacts in probability](../../../stochastic-process.md#uniform-convergence-on-compacts-in-probability) to the deterministic path $h(t)=mt$, by [Markov inequality](../../../probability-inequality.md#markov-inequality). Equip $C([0,\infty),\mathbb R)$ with its standard [compact-open topology](../../../real-analysis.md#compact-open-topology), metrized by

$$
d(f,g)=\sum_{j=1}^{\infty}2^{-j}\left(1\wedge\sup_{0\leq t\leq j}|f(t)-g(t)|\right).
$$

For each finite number of terms their suprema converge to zero in probability, and the remaining tail is bounded deterministically by $\sum_{j>J}2^{-j}$. Thus $d(S^{(N)},h)\to0$ in probability. [Convergence in probability](../../../convergence-of-random-variables.md#convergence-in-probability) to a deterministic point implies [weak convergence of probability measures](../../../convergence-of-random-variables.md#weak-convergence-of-probability-measures), so the [fluid limit](../../../queueing-theory.md#fluid-limit) is

$$
\boxed{\mu_N\Longrightarrow\delta_h,\qquad h(t)=mt.}
$$

Here $\delta_h$ is the [Dirac measure](../../../measure-theory.md#dirac-measure) concentrated on that continuous path. The topology is [locally uniform convergence](../../../real-analysis.md#locally-uniform-convergence); no assertion of [uniform convergence](../../../real-analysis.md#uniform-convergence) over the entire unbounded half-line is needed. The interpolation is intended for integers $k\geq0$, including the initial interval $[0,1]$. If the PDF's $\mathbb Z^+$ is interpreted as strictly positive integers, that initial piece is omitted from the displayed definition and must be supplied by the same formula using $S_0=0$.

## 2

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

For the forward implication, let $(M_n)$ be a [martingale](../../../martingale.md) and let the [stopping time](../../../martingale.md#stopping-time) $T$ satisfy $0\leq T\leq N$ for a deterministic integer $N$. The stopped variable is integrable because it uses only finitely many integrable values. The pathwise identity

$$
M_T=M_0+\sum_{j=1}^{N}(M_j-M_{j-1})\mathbf1_{\{T\geq j\}}
$$

expresses it through [martingale](../../../martingale.md) increments. Since $\{T\geq j\}=\{T>j-1\}\in\mathcal F_{j-1}$, each summand has [expectation](../../../probability-theory.md#expected-value) zero by [conditional expectation](../../../measure-theory.md#conditional-expectation). Consequently

$$
\boxed{\mathbb E M_T=\mathbb E M_0.}
$$

This proves the bounded-time case of the [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) directly; no assumptions about an unbounded stopping time are being used.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

For the converse in the [characterization of a martingale by stopped expectations](../../../martingale.md#characterization-of-a-martingale-by-stopped-expectations), fix $n\geq0$ and $A\in\mathcal F_n$. Define the [bounded stopping time](../../../martingale.md#bounded-stopping-time)

$$
T_A=\begin{cases}n+1,&\omega\in A,\\ n,&\omega\notin A.\end{cases}
$$

Indeed, its only nontrivial sublevel [event](../../../probability-theory.md#event) is $\{T_A\leq n\}=A^c\in\mathcal F_n$. Applying the assumed stopped-expectation equality to $T_A$ and to the deterministic stopping time $n$ gives

$$
0=\mathbb E(M_{T_A}-M_n)=\mathbb E\bigl[\mathbf1_A(M_{n+1}-M_n)\bigr].
$$

This holds for every $A\in\mathcal F_n$. Since $M_n$ is [adapted](../../../stochastic-process.md#adapted-process) and both variables are integrable, the defining test-event property of [conditional expectation](../../../measure-theory.md#conditional-expectation) yields

$$
\boxed{\mathbb E[M_{n+1}\mid\mathcal F_n]=M_n.}
$$

Together with the given adaptation and integrability, this is exactly the [martingale](../../../martingale.md) property.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For $m\geq1$, the increments have exponential moment

$$
\mathbb E2^{X_1}=\frac67\,2^{-1}+\frac17\,2^2=1.
$$

Thus $Z_n=2^{S_n}$ is an [exponential martingale of a random walk](../../../markov-process.md#exponential-martingale-of-a-random-walk) relative to the natural [filtration](../../../stochastic-process.md#filtration-probability-theory). We justify its stopping limit. From any surviving state in $(-m,m)$, a block of $2m$ successive increments all equal to $-1$ forces an exit. The block has probability $q=(6/7)^{2m}>0$, independently of the preceding increments. The [geometric tail bound from a uniform escape probability](../../../martingale.md#geometric-tail-bound-from-a-uniform-escape-probability) gives

$$
\mathbb P(T>2m\ell)\leq(1-q)^\ell,
$$

so $T$ is finite [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) and has finite [expectation](../../../probability-theory.md#expected-value).

At the lower exit $S_T=-m$ exactly; at the upper exit $S_T$ is either $m$ or $m+1$. Before exit the same overall bound $-m\leq S_{n\wedge T}\leq m+1$ holds. Hence $Z_{n\wedge T}$ is bounded by $2^{m+1}$, uniformly in $n$. The bounded [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) gives $\mathbb E Z_{n\wedge T}=Z_0=1$, and the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) now yields

$$
\boxed{\mathbb E2^{S_T}=1.}
$$

Allowing the upper overshoot by one is essential; the terminal state need not equal $m$ on upper exit.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The mean increment is $\mathbb EX_1=-6/7+2/7=-4/7$, so $M_n=S_n+(4/7)n$ is a [martingale](../../../martingale.md). Applying the bounded [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) at $n\wedge T$ gives

$$
\mathbb E S_{n\wedge T}=-\frac47\mathbb E(n\wedge T).
$$

The terminal sums are bounded by the exit-state bounds from (b), while $n\wedge T$ increases to the integrable stopping time $T$. The [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) on the left and the [monotone convergence theorem](../../../measure-theory.md#monotone-convergence-theorem) on the right therefore prove

$$
\boxed{\mathbb E S_T=-\frac47\mathbb ET.}
$$

This is also [Wald's equation](../../../probability-theory.md#wald-s-equation) here. In fact, the stopped identity already implies $\mathbb E(n\wedge T)\leq7m/4$ from $S_{n\wedge T}\geq-m$, giving another direct finite-expectation justification.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Write $p_m=\mathbb P(S_T=m)$, $p_{m+1}=\mathbb P(S_T=m+1)$, and $q_m=p_m+p_{m+1}$. Part (b) gives

$$
1=2^{-m}(1-q_m)+2^mp_m+2^{m+1}p_{m+1},
$$

so $q_m\leq2^{-m}$. The exit-state decomposition also gives

$$
\frac{\mathbb ES_T}{m}=-1+2q_m+\frac{p_{m+1}}m\longrightarrow-1.
$$

Combining this with part (c), including the upper overshoot, yields

$$
\boxed{\frac{\mathbb ET_m}{m}\longrightarrow\frac74.}
$$

For example, the same calculation supplies the quantitative bound

$$
0\leq\frac74-\frac{\mathbb ET_m}{m}\leq\frac74\left(2+\frac1m\right)2^{-m}.
$$

The asymptotic linear growth is determined by the negative mean increment; the exponentially unlikely upper exit gives a vanishing correction.

## 3

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem) in its $L^1$-bounded form says that a [martingale](../../../martingale.md) with $\sup_n\mathbb E|M_n|<\infty$ has an integrable limit $M_\infty$ and

$$
\boxed{M_n\longrightarrow M_\infty\quad\text{almost surely},\qquad
\mathbb E|M_\infty|\leq\sup_n\mathbb E|M_n|.}
$$

The norm bound on the limit follows from [Fatou lemma](../../../measure-theory.md#fatou-s-lemma). Boundedness in $L^1$ by itself does not imply [convergence in L1](../../../convergence-of-random-variables.md#convergence-in-l1). The [uniformly integrable martingale convergence theorem](../../../martingale.md#uniformly-integrable-martingale-convergence-theorem) gives the stronger conclusion: if $(M_n)$ is [uniformly integrable](../../../convergence-of-random-variables.md#uniform-integrability), then $M_n\to M_\infty$ both [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) and in [L1 norm](../../../functional-analysis.md#l1-norm), and $M_n=\mathbb E[M_\infty\mid\mathcal F_n]$. Conversely, [convergence in L1](../../../convergence-of-random-variables.md#convergence-in-l1) implies [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability).

For the distinction, the [fair-coin doubling martingale](../../../martingale.md#fair-coin-doubling-martingale) $M_n=2^n\mathbf1_{\{\text{first }n\text{ tosses are heads}\}}$ has [expectation](../../../probability-theory.md#expected-value) one for every $n$ but converges [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) to zero. Its [L1 norm](../../../functional-analysis.md#l1-norm) remains one, so its convergence is not in [L1 norm](../../../functional-analysis.md#l1-norm). These two formulations specify exactly which hypothesis is needed in part (d).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For $1<p<\infty$, the [Lp martingale convergence theorem](../../../martingale.md#lp-martingale-convergence-theorem) states that a [martingale](../../../martingale.md) with $\sup_n\mathbb E|M_n|^p<\infty$ has a limit $M_\infty\in L^p$ such that

$$
\boxed{M_n\to M_\infty\text{ almost surely},\qquad
\|M_n-M_\infty\|_p\to0.}
$$

Moreover, $M_n=\mathbb E[M_\infty\mid\mathcal F_n]$ and $\mathbb E|M_\infty|^p\leq\sup_n\mathbb E|M_n|^p$. To see why $p>1$ matters, the [Doob Lp maximal inequality](../../../martingale.md#doob-lp-maximal-inequality) gives an integrable dominating variable $(\sup_n|M_n|)^p$. The [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem) first supplies the almost-sure limit, then the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) supplies convergence in the [Lp norm](../../../real-analysis.md#lp-norm). This maximal estimate is unavailable at $p=1$ in the required form.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Work on $([0,1],\mathcal B,dt)$ as a [probability space](../../../probability-theory.md#probability-space), with [Lebesgue measure](../../../measure-theory.md#lebesgue-measure) of total mass one. Let $\mathcal F_n$ be the [filtration](../../../stochastic-process.md#filtration-probability-theory) generated by the level-$n$ half-open dyadic cells together with the separate null cell $\{1\}$. Define the [dyadic slope martingale](../../../martingale.md#dyadic-slope-martingale) by

$$
G_n(t)=2^n\bigl[f((k+1)2^{-n})-f(k2^{-n})\bigr]
\quad\text{on }[k2^{-n},(k+1)2^{-n}).
$$

The endpoint $t=1$ may be assigned any value, since it is a null set for [Lebesgue measure](../../../measure-theory.md#lebesgue-measure). The two child slopes average to their parent slope, by telescoping the two increments. Therefore $\mathbb E[G_{n+1}\mid\mathcal F_n]=G_n$ [almost everywhere](../../../measure-theory.md#almost-everywhere), so this is a [martingale](../../../martingale.md). The [Lipschitz condition](../../../real-analysis.md#lipschitz-continuity) gives $|G_n|\leq K$ everywhere except possibly at the freely chosen endpoint, where we take zero.

Apply the [Lp martingale convergence theorem](../../../martingale.md#lp-martingale-convergence-theorem) with $p=2$. Its limit $g$ has $|g|\leq K$ [almost everywhere](../../../measure-theory.md#almost-everywhere) and $G_n\to g$ in [L1 norm](../../../functional-analysis.md#l1-norm) as well, by [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). Choose a measurable representative of $g$ and set it to zero on any exceptional null set; it is then a bounded [measurable function](../../../measure-theory.md#measurable-function) on the entire interval.

Set $f_n(x)=f(0)+\int_0^xG_n(t)dt$. Telescoping at the grid points shows that $f_n$ is the [linear interpolation](../../../function.md#linear-interpolation) of $f$ on the dyadic grid. The [Lipschitz condition](../../../real-analysis.md#lipschitz-continuity) gives $\|f_n-f\|_\infty\leq K2^{-n}\to0$. Also

$$
\sup_{0\leq x\leq1}\left|\int_0^x(G_n-g)(t)dt\right|\leq\|G_n-g\|_1\to0.
$$

The two uniform limits coincide, giving the [absolutely continuous function](../../../sobolev-space.md#absolutely-continuous-function) representation

$$
\boxed{f(x)=f(0)+\int_0^xg(t)dt\quad(0\leq x\leq1),\qquad |g(t)|\leq K.}
$$

The chosen bound holds for every $t$ after the null-set modification; the [integral](../../../calculus.md#integral) identity holds for every $x$ simultaneously.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Use the same [dyadic slope martingale](../../../martingale.md#dyadic-slope-martingale) $G_n$ and dyadic [filtration](../../../stochastic-process.md#filtration-probability-theory) as in (c). Each $G_n$ is integrable, since it takes finitely many finite values. On each dyadic cell, the absolute slope is $2^n$ times the absolute endpoint increment. Consequently the hypothesis in the PDF is exactly

$$
\int_0^1|G_n(t)|\mathbf1_{\{|G_n(t)|\geq\lambda\}}dt=V_n(f,\lambda),
\qquad
\sup_n\int_0^1|G_n|\mathbf1_{\{|G_n|\geq\lambda\}}dt\longrightarrow0.
$$

Thus $(G_n)$ is [uniformly integrable](../../../convergence-of-random-variables.md#uniform-integrability). It is also bounded in [L1 norm](../../../functional-analysis.md#l1-norm): choose a finite $\lambda_0>0$ at which the supremum of the tails is finite, and use $\|G_n\|_1\leq\lambda_0+\sup_jV_j(f,\lambda_0)$. The [uniformly integrable martingale convergence theorem](../../../martingale.md#uniformly-integrable-martingale-convergence-theorem) supplies $g\in L^1([0,1])$ with $G_n\to g$ in [L1 norm](../../../functional-analysis.md#l1-norm).

The functions $f_n(x)=f(0)+\int_0^xG_n(t)dt$ are again the dyadic [linear interpolations](../../../function.md#linear-interpolation) of $f$. Since $f$ is continuous on a compact interval, it is [uniformly continuous](../../../topological-analysis.md#uniform-continuity), and $\|f_n-f\|_\infty\leq\omega_f(2^{-n})\to0$, where $\omega_f$ is its [modulus of continuity](../../../topological-analysis.md#modulus-of-continuity). On the other hand, the [integral](../../../calculus.md#integral) of $G_n-g$ is uniformly bounded in absolute value by $\|G_n-g\|_1\to0$. Hence the [dyadic slope-tail criterion for absolute continuity](../../../sobolev-space.md#dyadic-slope-tail-criterion-for-absolute-continuity) gives

$$
\boxed{f(x)=f(0)+\int_0^xg(t)dt\quad\text{for every }x\in[0,1],\qquad g\in L^1([0,1]).}
$$

No boundedness of $g$ is asserted here; the tail condition permits integrable densities that are unbounded.

## 4

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Write $A_n=\max_{0\leq k<2^n}|\xi_{(k+1)2^{-n}}-\xi_{k2^{-n}}|$. The maximum of nonnegative numbers to the power $p$ is bounded by their sum, so the increment hypothesis gives

$$
\|A_n\|_p^p\leq\sum_{k=0}^{2^n-1}\mathbb E|\xi_{(k+1)2^{-n}}-\xi_{k2^{-n}}|^p
\leq C^p2^n2^{-np\beta}.
$$

Therefore $\|A_n\|_p\leq C2^{-n(\beta-1/p)}$. The [Minkowski inequality](../../../real-analysis.md#minkowski-inequality) and completeness of $L^p$ imply convergence of the defining series whenever

$$
\boxed{0<\alpha<\beta-\frac1p,\qquad
\|K_\alpha\|_p\leq\frac{2C}{1-2^{-(\beta-1/p-\alpha)}}.}
$$

For a fully explicit argument, the norm of every tail is at most $2C\sum_{n\geq N}2^{-n(\beta-1/p-\alpha)}$, which tends to zero. Since the summands are nonnegative, their pointwise increasing sum equals this finite $L^p$ limit and is finite [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). This is a guaranteed range; no endpoint convergence follows from the displayed summability estimate. The assumptions control increments only and do not require $\xi_0\in L^p$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Fix an exponent in the range from (a), and work on the single probability-one [event](../../../probability-theory.md#event) where $K_\alpha<\infty$ and all dyadic values are finite. We give the [dyadic increment chaining](../../../stochastic-process.md#dyadic-increment-chaining) argument. For dyadic $s<t$, put $\delta=t-s$ and choose $n\geq0$ with $2^{-n}\leq\delta<2^{1-n}$. Let $s_j=2^{-j}\lfloor2^js\rfloor$ and $t_j=2^{-j}\lfloor2^jt\rfloor$. The level-$n$ approximations are at most two grid steps apart, so their difference is bounded by $2A_n$. At each subsequent level an approximation either stays fixed or moves by one adjacent level increment. Because $s,t$ are dyadic, these approximations eventually equal $s,t$. Thus

$$
|\xi_t-\xi_s|\leq2\sum_{j\geq n}A_j
\leq2^{-n\alpha}K_\alpha\leq K_\alpha|t-s|^\alpha.
$$

The [dyadic rationals](../../../arithmetic.md#dyadic-rational) are dense in $[0,1]$, so this uniform bound gives a unique continuous extension $X$ to the entire interval, with

$$
\boxed{X_t=\xi_t\quad(t\in D),\qquad
|X_t-X_s|\leq K_\alpha|t-s|^\alpha.}
$$

All these equalities hold on that one [event](../../../probability-theory.md#event), not merely one [event](../../../probability-theory.md#event) per dyadic time. Define $X$ to be the zero path on its null complement. Each $X_t$ is measurable as the limit of the [random variables](../../../random-variable.md) at deterministic left dyadic approximations. Alternatively, their measurable [linear interpolations](../../../function.md#linear-interpolation) converge uniformly to $X$, which also shows measurability as a random element of $C([0,1])$. This is the continuous extension version of a [continuous modification](../../../stochastic-process.md#continuous-modification).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The [Gaussian process](../../../stochastic-process.md#gaussian-process) assumption and the covariance formula give a centered Gaussian increment with [variance](../../../variance.md)

$$
\mathbb E|\xi_t-\xi_s|^2=t+s-2\min(s,t)=|t-s|.
$$

For every finite $p>1$, a standard normal variable $Z$ therefore gives

$$
\|\xi_t-\xi_s\|_p=\|Z\|_p|t-s|^{1/2}.
$$

For any $0<\alpha<1/2$, choose $p>\max(2,(1/2-\alpha)^{-1})$. Then $\alpha<1/2-1/p$, so parts (a) and (b) give a [Hölder continuous function](../../../sobolev-space.md#holder-condition) of exponent $\alpha$ as an extension. To obtain one extension with every required exponent, take a countable sequence $\alpha_j\uparrow1/2$ and apply the construction with suitable $p_j$. Intersect the probability-one [events](../../../probability-theory.md#event). Their continuous extensions agree on the dense set $D$ and hence agree everywhere. For each smaller exponent choose $j$ with $\alpha<\alpha_j$; since $|t-s|\leq1$, the bound with $\alpha_j$ also implies the bound with $\alpha$. Thus

$$
\boxed{X\in C^{0,\alpha}([0,1])\quad\text{almost surely, simultaneously for every }0<\alpha<\tfrac12.}
$$

The exponent constants may depend on $\alpha$ and the sample path. This proves [Brownian Hölder regularity](../../../brownian-motion.md#brownian-holder-regularity) for the continuous Gaussian extension without making an uncountable intersection of unrelated full-probability [events](../../../probability-theory.md#event).

## 5

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Let $\tau_r=\inf\{t\geq0:|B_t|=r\}$, $\tau_R=\inf\{t\geq0:|B_t|=R\}$, and $\tau=\tau_r\wedge\tau_R$. The function $u(y)=|y|^{-1}$ is harmonic away from the origin: its [radial Laplacian](../../../partial-differential-equation.md#radial-laplacian) in dimension three is

$$
u''(\rho)+\frac2\rho u'(\rho)=\frac2{\rho^3}-\frac2{\rho^3}=0.
$$

The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) therefore makes $u(B_{t\wedge\tau})$ a [local martingale](../../../martingale.md#local-martingale), bounded between $1/R$ and $1/r$, hence a true [martingale](../../../martingale.md). The annulus exit time is finite [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). For instance, exit from the containing [open ball](../../../topology.md#open-ball) is finite because from every point in the [open ball](../../../topology.md#open-ball) a sufficiently large [Gaussian vector](../../../probability-and-statistics.md#gaussian-random-vector) increment has a uniform positive probability of leaving it in unit time; iterate the [geometric tail bound from a uniform escape probability](../../../martingale.md#geometric-tail-bound-from-a-uniform-escape-probability).

The [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) at $t\wedge\tau$, followed by the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem), gives $\mathbb Eu(B_\tau)=u(x)$. By continuity, there is no radial overshoot and the two exit [spheres](../../../geometry-and-topology.md#sphere) cannot be hit simultaneously. Writing $p=\mathbb P_x(\tau_r<\tau_R)$ gives

$$
\frac1{|x|}=\frac pr+\frac{1-p}{R},\qquad
\boxed{p=\frac{|x|^{-1}-R^{-1}}{r^{-1}-R^{-1}}.}
$$

All harmonicity and boundedness statements apply only in the annulus, which stays away from the singularity at zero.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Take a sequence $R\uparrow\infty$ with $R>|x|$. The [events](../../../probability-theory.md#event) $\{\tau_r<\tau_R\}$ increase, and their union is $\{\tau_r<\infty\}$. Indeed, if the [sphere](../../../geometry-and-topology.md#sphere) of radius $r$ is reached at a finite time, continuity makes the path bounded up to that time, so a sufficiently large outer [sphere](../../../geometry-and-topology.md#sphere) has not yet been hit. Conversely, each [event](../../../probability-theory.md#event) in the union includes a finite inner hit.

Taking the limit of part (a)'s [Brownian sphere-hitting probability in dimension three](../../../brownian-motion.md#brownian-sphere-hitting-probability-in-dimension-three) yields the sharper formula

$$
\boxed{\mathbb P_x(\tau_r<\infty)=\frac r{|x|}<1\qquad(|x|>r).}
$$

This establishes the required escape probability without presupposing the [transience of Brownian motion in dimension at least three](../../../brownian-motion.md#transience-of-brownian-motion-in-dimension-at-least-three).

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

First suppose $|x+z|\leq r$ for some lattice point $-z$. If $|x+z|=r$, the desired hit is already at time zero. If $|x+z|<r$, finite exit from that bounded [open ball](../../../topology.md#open-ball) and continuity give the required [sphere](../../../geometry-and-topology.md#sphere) hit [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence).

It remains to consider $|x+z|>r$ for every $z\in\mathbb Z^3$. At each integer time $n$, choose a nearest lattice point $-z_n$ to $B_n$ by rounding its three coordinates, with a fixed rule at ties. Then $|B_n+z_n|\leq\sqrt3/2$. Put $\delta=\min(r/2,1/4)>0$. Conditional on the past, $B_{n+1}-B_n$ is a standard three-dimensional [Gaussian vector](../../../probability-and-statistics.md#gaussian-random-vector). Its [probability density function](../../../continuous-probability-distribution.md#probability-density-function) is bounded below on the [open ball](../../../topology.md#open-ball) of radius $\delta$ centered at $-(B_n+z_n)$ by

$$
(2\pi)^{-3/2}\exp\!\left[-\tfrac12(\sqrt3/2+\delta)^2\right].
$$

Multiplying by the volume of that [open ball](../../../topology.md#open-ball) gives a constant $\varepsilon>0$, independent of $n$ and the past, such that

$$
\mathbb P\bigl(|B_{n+1}+z_n|<\delta\mid\mathcal F_n\bigr)\geq\varepsilon.
$$

The probability of avoiding all lattice-centered radius-$r$ [open balls](../../../topology.md#open-ball) at the first $N$ positive integer times is therefore at most $(1-\varepsilon)^N$, by iterated [conditional expectation](../../../measure-theory.md#conditional-expectation). Eventually the path enters one such [open ball](../../../topology.md#open-ball) [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Since the initial point was outside that particular [open ball](../../../topology.md#open-ball), continuity forces an earlier crossing of its [sphere](../../../geometry-and-topology.md#sphere). This proves [Brownian hitting of lattice spheres](../../../brownian-motion.md#brownian-hitting-of-lattice-spheres):

$$
\boxed{\mathbb P_x\!\left(\exists t\geq0,\ z\in\mathbb Z^3:\ |B_t+z|=r\right)=1.}
$$

A uniform chance of hitting some member of the periodic family replaces recurrence to any one prescribed [sphere](../../../geometry-and-topology.md#sphere); there is no contradiction with (b).

## 6

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

For $a>0$, the [Brownian reflection principle](../../../brownian-motion.md#reflection-principle-wiener-process) gives, for $t>0$,

$$
\mathbb P(H_a>t)=2\Phi(a/\sqrt t)-1\longrightarrow0,
$$

where $\Phi$ is the [standard normal distribution function](../../../probability-theory.md#standard-normal-distribution-function). Hence $H_a<\infty$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence); for $a=0$, $H_0=0$.

For $u\geq0$, use the [Exponential martingale for Brownian motion](../../../brownian-motion.md#exponential-martingale-for-brownian-motion) $Z_t=\exp(uB_t-u^2t/2)$. At $H_a\wedge t$, it is bounded by $e^{ua}$ because $B_s<a$ before the first hit and $B_{H_a}=a$ by continuity. The bounded [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) gives $\mathbb EZ_{H_a\wedge t}=1$. Its limit is $e^{ua-u^2H_a/2}$, and the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) yields $\mathbb E e^{ua-u^2H_a/2}=1$. Equivalently, the [Brownian first-passage Laplace transform](../../../markov-process.md#brownian-first-passage-laplace-transform) is

$$
\boxed{\mathbb E e^{-\lambda H_a}=e^{-a\sqrt{2\lambda}}\qquad(a,\lambda\geq0).}
$$

Taking $\lambda=u^2/2$ proves the displayed exponential identity. The cases $u=0$ and $a=0$ are included. The restriction $u\geq0$ is what gives the upper bound on the stopped exponential.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Fix a deterministic $a\geq0$. By the [Strong Markov property](../../../markov-process.md#strong-markov-property) at the finite [Brownian first-passage time](../../../markov-process.md#brownian-first-passage-time) $H_a$, the process $\widetilde B_s=B_{H_a+s}-a$ is a standard [Brownian motion](../../../brownian-motion.md) started at zero. Such a process takes positive values arbitrarily soon [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence): for every $\varepsilon>0$, the [Brownian reflection principle](../../../brownian-motion.md#reflection-principle-wiener-process) makes its maximum on $[0,\varepsilon]$ have the distribution of $|B_\varepsilon|$, so the probability that the maximum is zero is zero. Intersecting these [events](../../../probability-theory.md#event) for $\varepsilon=1/n$ gives an infimum of positive-crossing times equal to zero. Therefore

$$
\boxed{T_a=H_a\quad\text{almost surely for each fixed }a\geq0.}
$$

The infimum defining the strict crossing time need not itself be a time when $B_t>a$; continuity gives $B_{T_a}=a$. The quantifier here is fixed-level [almost sure equality](../../../convergence-of-random-variables.md#almost-sure-equality), not [indistinguishability of stochastic processes](../../../stochastic-process.md#indistinguishability-of-stochastic-processes) as the level varies.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Let $A=\max_{0\leq t\leq1}B_t$, a random level. The [Brownian reflection principle](../../../brownian-motion.md#reflection-principle-wiener-process) gives $A\overset d=|B_1|$, so $A>0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Also $A-B_1\overset d=|B_1|$: this follows by applying reflection to the reversed increment process $(B_1-B_{1-s})_{0\leq s\leq1}$, which has the law of a standard [Brownian motion](../../../brownian-motion.md). Thus $B_1<A$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) as well.

By continuity and [compactness](../../../topology.md#compact-space), $A$ is attained at some time strictly between zero and one, so $H_A<1$. It is not exceeded anywhere on $[0,1]$; since $B_1<A$, continuity even excludes an exceedance in a positive interval just after time one. Consequently $T_A>1$. Both conclusions hold on a single probability-one [event](../../../probability-theory.md#event), giving the [fixed-level versus simultaneous Brownian passage-time equality](../../../markov-process.md#fixed-level-versus-simultaneous-brownian-passage-time-equality) distinction:

$$
\boxed{\mathbb P\bigl(T_a=H_a\text{ for every }a\geq0\bigr)=0.}
$$

Thus **the simultaneous assertion is false**. Equality for each deterministic level, and even simultaneously for all rational levels, cannot be extended to all real levels by an uncountable intersection.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

Use the usual completed right-continuous [Brownian filtration](../../../brownian-motion.md#brownian-filtration). The strict passage process $(T_a)_{a\geq0}$ is finite at every level on one probability-one [event](../../../probability-theory.md#event): finiteness at all integer levels from (a) suffices by monotonicity. Also $T_0=0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) by (b).

For each fixed $a$, $T_a$ is a [stopping time](../../../martingale.md#stopping-time) with $B_{T_a}=a$. The [Strong Markov property](../../../markov-process.md#strong-markov-property) shows that the passage times above this level depend on a new independent standard [Brownian motion](../../../brownian-motion.md). Thus for $0\leq a<b$, $T_b-T_a$ is independent of the past at $T_a$ and has the same law as $T_{b-a}$. Iteration gives [independent increments](../../../stochastic-process.md#independent-increments) and [stationary increments](../../../stochastic-process.md#stationary-increments) in the level parameter. From (a) and fixed-level equality,

$$
\mathbb E e^{-\lambda T_a}=e^{-a\sqrt{2\lambda}}.
$$

For $\lambda,\eta>0$, this also proves continuity in probability at zero, since

$$
\mathbb P(T_h>\eta)\leq\frac{1-e^{-h\sqrt{2\lambda}}}{1-e^{-\lambda\eta}}\longrightarrow0.
$$

Finally, with $M_t=\sup_{s\leq t}B_s$, we have $T_a=\inf\{t:M_t>a\}$. This [strict generalized inverse of a nondecreasing function](../../../calculus.md#strict-generalized-inverse-of-a-nondecreasing-function) is right-continuous: if $a_n\downarrow a$, then for any $t>T_a$ we have $M_t>a$, and eventually $M_t>a_n$, which forces $T_{a_n}\leq t$. Monotonicity gives the reverse bound. Monotonicity and local finiteness also give finite left limits. Hence $T$ is the [Brownian first-passage subordinator](../../../stochastic-process.md#brownian-first-passage-subordinator), with [càdlàg](../../../calculus.md#cadlag) paths.

Now condition on this clock, which is independent of $W$. For a deterministic partition $0=a_0<a_1<\cdots<a_k$, write $\Delta T_j=T_{a_j}-T_{a_{j-1}}$ and $\Delta X_j=W_{T_{a_j}}-W_{T_{a_{j-1}}}$. Conditional on the clock these are independent centered Gaussian increments, with respective variances $\Delta T_j$. Consequently

$$
\mathbb E\exp\!\left(i\sum_{j=1}^ku_j\Delta X_j\right)
=\mathbb E\exp\!\left(-\frac12\sum_{j=1}^ku_j^2\Delta T_j\right)
=\prod_{j=1}^k\exp\bigl(-(a_j-a_{j-1})|u_j|\bigr).
$$

Factorization and dependence only on interval lengths prove [independent increments](../../../stochastic-process.md#independent-increments) and [stationary increments](../../../stochastic-process.md#stationary-increments) for $X$. For small $h$, $T_h\to0$ in probability, and [independence](../../../random-variable.md#independent-random-variables) and continuity of $W$ imply $W_{T_h}\to0$ in probability. For example, bound its deviation probability by $\mathbb P(T_h>\eta)+\mathbb P(\sup_{t\leq\eta}|W_t|>\varepsilon)$ and then let $h\downarrow0$ and $\eta\downarrow0$. [Stationary increments](../../../stochastic-process.md#stationary-increments) give [stochastic continuity](../../../stochastic-process.md#stochastic-continuity) at every deterministic level. Composition of the continuous path of $W$ with the nondecreasing [càdlàg](../../../calculus.md#cadlag) clock gives [càdlàg](../../../calculus.md#cadlag) paths for $X$, and $X_0=0$. Thus

$$
\boxed{(X_a)_{a\geq0}\text{ is a Lévy process}.}
$$

This is [subordination of a Lévy process](../../../stochastic-process.md#subordination-of-a-levy-process). Using strict passage times ensures the required right-continuous path choice, despite their fixed-level equality with the non-strict times.

<h3 id="6/e">e</h3>

↑ **Parent:** [6](#6)

<h4 id="6/e/solution">Solution</h4>

↑ **Parent:** [E](#6/e)

Specify the sign convention for the [Lévy characteristic exponent](../../../stochastic-process.md#characteristic-exponent-of-a-levy-process) by

$$
\mathbb E e^{iuX_a}=e^{-a\Psi(u)}.
$$

Conditioning on $T_a$ and using the [Brownian first-passage Laplace transform](../../../markov-process.md#brownian-first-passage-laplace-transform) gives

$$
\mathbb E e^{iuW_{T_a}}=\mathbb E e^{-u^2T_a/2}
=e^{-a\sqrt{u^2}}=e^{-a|u|}.
$$

Therefore

$$
\boxed{\Psi(u)=|u|.}
$$

The absolute value is essential for negative $u$. The process is the standard symmetric [Cauchy process](../../../stochastic-process.md#cauchy-process); for $a>0$, $X_a$ has the [Cauchy distribution](../../../probability-theory.md#cauchy-distribution) with location zero and scale $a$. If the exponent convention instead uses $\mathbb E e^{iuX_a}=e^{a\psi(u)}$, the answer is $\psi(u)=-|u|$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
