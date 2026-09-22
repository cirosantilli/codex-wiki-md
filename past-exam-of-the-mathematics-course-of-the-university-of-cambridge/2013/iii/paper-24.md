# Paper 24

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_24.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_24.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
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
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)

## 1

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem) says that a discrete-time [martingale](../../../martingale.md) $(M_n,\mathcal F_n)$ satisfying

$$
\sup_n\mathbb E|M_n|<\infty
$$

has an [almost sure convergence](../../../convergence-of-random-variables.md#almost-sure-convergence) limit $M_\infty$, finite [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) and in $L^1$. The theorem asserts that the limit is integrable; it does not assert [convergence in L1](../../../convergence-of-random-variables.md#convergence-in-l1). More generally, the [almost sure submartingale convergence theorem](../../../martingale.md#almost-sure-submartingale-convergence-theorem) applies to a [submartingale](../../../martingale.md#submartingale) with $\sup_n\mathbb E M_n^+<\infty$. [Uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability) is the additional condition that upgrades a [martingale](../../../martingale.md)'s convergence to [convergence in L1](../../../convergence-of-random-variables.md#convergence-in-l1).

For the requested distinction, let $(\xi_k)$ be independent fair Bernoulli variables and use their [natural filtration](../../../stochastic-process.md#natural-filtration). The [coin-doubling martingale](../../../martingale.md#coin-doubling-martingale)

$$
M_0=1,\qquad M_n=2^n\mathbf1_{\{\xi_1=\cdots=\xi_n=1\}}
$$

is a [nonnegative martingale](../../../martingale.md#nonnegative-martingale): conditionally on $\mathcal F_n$, the next factor is $2\xi_{n+1}$ with mean one, so $\mathbb E(M_{n+1}\mid\mathcal F_n)=M_n$. Also $\mathbb E|M_n|=\mathbb E M_n=1$ for every $n$, giving the required uniform $L^1$ bound. The probability that all the Bernoulli variables equal one is $\lim_n2^{-n}=0$. Therefore a zero is eventually encountered [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), after which $M_n$ stays zero. Thus

$$
\boxed{M_n\longrightarrow0\text{ almost surely},\qquad
\mathbb E|M_n-0|=1\text{ for every }n.}
$$

There can be no other $L^1$ limit, since [convergence in L1](../../../convergence-of-random-variables.md#convergence-in-l1) implies [convergence in probability](../../../convergence-of-random-variables.md#convergence-in-probability), whose limit must agree with the almost sure limit. **This [martingale](../../../martingale.md) satisfies the almost sure theorem but does not converge in $L^1$.**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Put $v=\mathbb E X_n^2$. For $c\geq0$, [conditional Jensen inequality](../../../measure-theory.md#conditional-jensen-inequality) applied to the [convex function](../../../real-analysis.md#convex-function) $x\mapsto(x+c)^2$ shows that

$$
Z_k=(X_k+c)^2
$$

is a nonnegative [submartingale](../../../martingale.md#submartingale). Its integrability follows from the square integrability of $X_k$. If $X_k\geq\lambda$, then $Z_k\geq(\lambda+c)^2$, since $c\geq0$. The [Doob maximal inequality for a nonnegative submartingale](../../../martingale.md#doob-maximal-inequality-for-a-nonnegative-submartingale) yields

$$
\mathbb P\left(\max_{1\leq k\leq n}X_k\geq\lambda\right)
\leq\frac{\mathbb E(X_n+c)^2}{(\lambda+c)^2}
=\frac{v+c^2}{(\lambda+c)^2},
$$

where zero mean removes the cross term. For completeness, the maximal inequality follows by stopping at the first crossing: on the event of a crossing at $k$, the [submartingale](../../../martingale.md#submartingale) property gives $\mathbb E[Z_n\mathbf1_{\{T=k\}}]\geq\mathbb E[Z_k\mathbf1_{\{T=k\}}]$. Sum over $k\leq n$, and use nonnegativity on the event of no crossing.

The derivative of the last ratio is

$$
\frac{d}{dc}\frac{v+c^2}{(\lambda+c)^2}
=\frac{2(c\lambda-v)}{(\lambda+c)^3}.
$$

For $v>0$, the minimum over $c\geq0$ is attained at $c=v/\lambda$. Substitution gives the [one-sided maximal inequality for a centered square-integrable martingale](../../../martingale.md#one-sided-maximal-inequality-for-a-centered-square-integrable-martingale):

$$
\boxed{\mathbb P\left(\max_{1\leq k\leq n}X_k\geq\lambda\right)
\leq\frac{v}{\lambda^2+v}.}
$$

If $v=0$, $X_n=0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) and $X_k=\mathbb E(X_n\mid\mathcal F_k)=0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) for every $k\leq n$, so the bound also holds. The optimization is the same one underlying the [Cantelli inequality](../../../probability-inequality.md#cantelli-inequality), but the [submartingale](../../../martingale.md#submartingale) argument controls the entire finite-time maximum.

## 2

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A real [Lévy process](../../../stochastic-process.md#levy-process) is a real-valued [stochastic process](../../../stochastic-process.md) $(X_t)_{t\geq0}$ with the following properties:

- $X_0=0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence).
- It has [independent increments](../../../stochastic-process.md#independent-increments): increments over disjoint ordered time intervals are independent.
- It has [stationary increments](../../../stochastic-process.md#stationary-increments): $X_{s+t}-X_s$ has the same law as $X_t$ for $s,t\geq0$.
- It has [stochastic continuity](../../../stochastic-process.md#stochastic-continuity): $X_s\to X_t$ in probability as $s\to t$.

One convention also includes [càdlàg](../../../calculus.md#cadlag) paths in the definition. Equivalently, under the intrinsic definition above one chooses the [càdlàg modification](../../../stochastic-process.md#cadlag-modification), which exists for such a [stochastic process](../../../stochastic-process.md). Thus the usual working version of a [Lévy process](../../../stochastic-process.md#levy-process) has [right-continuous](../../../calculus.md#right-continuous-function) paths with left limits. There is no assumption of finite [moments](../../../probability-theory.md#moment) or continuous paths.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Fix $u\in\mathbb R$ and let $s\to t$. For any $\delta>0$, use $|e^{ia}-e^{ib}|\leq\min(2,|a-b|)$ to obtain

$$
\begin{aligned}
|\varphi_{X_s}(u)-\varphi_{X_t}(u)|
&\leq\mathbb E|e^{iuX_s}-e^{iuX_t}|\\
&\leq |u|\delta+2\mathbb P(|X_s-X_t|>\delta).
\end{aligned}
$$

The probability tends to zero by [stochastic continuity](../../../stochastic-process.md#stochastic-continuity). Taking the limit superior and then letting $\delta\downarrow0$ proves

$$
\boxed{\varphi_{X_s}(u)\longrightarrow\varphi_{X_t}(u).}
$$

This proves [continuity of Lévy characteristic functions](../../../stochastic-process.md#continuity-of-levy-characteristic-functions) from the elementary estimate, without requiring [moments](../../../probability-theory.md#moment) or replacing [convergence in probability](../../../convergence-of-random-variables.md#convergence-in-probability) by an unjustified almost sure limit. At $t=0$, time approaches from the right. If stochastic continuity is formulated only at zero, [stationary increments](../../../stochastic-process.md#stationary-increments) give the same argument at every $t$: the absolute value of $X_s-X_t$ has the law of $|X_{|s-t|}|$. For $u=0$ the [characteristic function](../../../probability-theory.md#characteristic-function) is identically one.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For fixed $u$, write $h(t)=\varphi_{X_t}(u)$. [Independent increments](../../../stochastic-process.md#independent-increments) and [stationary increments](../../../stochastic-process.md#stationary-increments) give

$$
h(s+t)=\mathbb E\bigl[e^{iuX_s}e^{iu(X_{s+t}-X_s)}\bigr]
=h(s)h(t),\qquad h(0)=1.
$$

The preceding part gives continuity. Also $h$ never vanishes: if $h(t_0)=0$ with $t_0>0$, then $h(t_0/m)^m=0$ for every positive integer $m$, contradicting $h(t_0/m)\to1$.

Here is a direct proof of the [exponential form of Lévy characteristic functions](../../../stochastic-process.md#exponential-form-of-levy-characteristic-functions). Choose $a>0$ small enough that $|h(t)-1|<1/2$ on $[0,a]$. The principal [complex logarithm](../../../analysis.md#complex-logarithm) gives a continuous $L(t)=\log h(t)$ there, with $L(0)=0$. For $s,t\geq0$ with $s+t\leq a$, the multiplicative identity implies

$$
L(s+t)-L(s)-L(t)\in2\pi i\mathbb Z.
$$

This difference is continuous on the connected triangle of allowed $(s,t)$ and equals zero at $(0,0)$, so it is identically zero. Thus $L$ satisfies the additive [Cauchy functional equation](../../../analysis.md#cauchy-s-functional-equation) locally. Subdivision gives $L(a/m)=L(a)/m$ and $L(ka/m)=kL(a)/m$; continuity then gives $L(t)=tL(a)/a$ for every $t\in[0,a]$.

Define $\eta(u)=L(a)/a$. For any $t\geq0$, choose an integer $m$ with $t/m\leq a$; then

$$
\boxed{\varphi_{X_t}(u)=h(t)=h(t/m)^m=e^{t\eta(u)}.}
$$

The coefficient is unique: if two coefficients give the same exponential for every $t\geq0$, their derivatives at zero agree. In particular $\eta(0)=0$, and $\operatorname{Re}\eta(u)\leq0$ follows from $|h(t)|\leq1$. The [characteristic exponent of a Lévy process](../../../stochastic-process.md#characteristic-exponent-of-a-levy-process) has therefore been obtained from first principles, without invoking the [Lévy–Khintchine formula](../../../stochastic-process.md#levy-khintchine-formula).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Take two independent rate-one [Poisson processes](../../../probability-theory.md#poisson-process) $N^+$ and $N^-$, and let

$$
X_t=N_t^+-N_t^-.
$$

The [difference of independent Poisson processes](../../../stochastic-process.md#difference-of-independent-poisson-processes) starts at zero and has [stationary increments](../../../stochastic-process.md#stationary-increments) and [independent increments](../../../stochastic-process.md#independent-increments). Its paths are [càdlàg](../../../calculus.md#cadlag). For an interval of length $h$, the probability of any jump is $1-e^{-2h}\to0$, proving [stochastic continuity](../../../stochastic-process.md#stochastic-continuity). Thus $X$ is a [Lévy process](../../../stochastic-process.md#levy-process). The [characteristic function](../../../probability-theory.md#characteristic-function) of a [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) with mean $t$ is $\exp(t(e^{iu}-1))$, so [independence](../../../random-variable.md#independent-random-variables) gives

$$
\boxed{\mathbb E e^{iuX_t}
=\exp\bigl(t(e^{iu}-1)+t(e^{-iu}-1)\bigr)
=e^{2t(\cos u-1)}.}
$$

The [sample paths](../../../stochastic-process.md#sample-path) are integer-valued step functions with jumps $+1$ or $-1$. On every bounded interval there are only finitely many jumps, and independent Poisson arrival times coincide with probability zero. The combined arrival rate is two: holding times are independent exponentials of rate two, and each jump direction has probability $1/2$, independently of the holding times. This is equivalently a [Compound Poisson process](../../../stochastic-process.md#compound-poisson-process) of rate two with [Rademacher distribution](../../../probability-theory.md#rademacher-distribution) jump sizes. Its paths have [finite variation](../../../real-analysis.md#total-variation-of-a-function) on compact time intervals, although there are infinitely many jumps over the whole half-line [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence).

## 3

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use the [independent increments](../../../stochastic-process.md#independent-increments) of [Brownian motion](../../../brownian-motion.md), rather than merely checking that an [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) drift vanishes. For $0\leq s<t$, put $h=t-s$ and write $B_t=B_s+Z$, where $Z$ is independent of $\mathcal F_s$ and has [normal distribution](../../../probability-theory.md#normal-distribution) $N(0,h)$. Its first four [moments](../../../probability-theory.md#moment) are $0,h,0,3h^2$. Therefore

$$
\begin{aligned}
\mathbb E(B_t^2\mid\mathcal F_s)&=B_s^2+h,\\
\mathbb E(B_t^3\mid\mathcal F_s)&=B_s^3+3hB_s,\\
\mathbb E(B_t^4\mid\mathcal F_s)&=B_s^4+6hB_s^2+3h^2.
\end{aligned}
$$

For the cubic expression, the coefficient of $B_s$ after conditioning is $3(t-s)+\alpha(t)$, so $\alpha(t)=-3t$ makes it $\alpha(s)$. For the quartic expression, choose $\beta(t)=-6t$. Its conditioned coefficient of $B_s^2$ is then $6(t-s)-6t=-6s$. The constant term becomes

$$
3(t-s)^2-6t(t-s)+\gamma(t),
$$

which equals $3s^2$ when $\gamma(t)=3t^2$. Thus a standard choice is

$$
\boxed{\alpha(t)=-3t,\qquad\beta(t)=-6t,\qquad\gamma(t)=3t^2.}
$$

The resulting [stochastic processes](../../../stochastic-process.md) are [Hermite polynomial martingales](../../../numerical-analysis.md#space-time-hermite-polynomial) $H_3(B_t,t)$ and $H_4(B_t,t)$. They are genuine integrable [martingales](../../../martingale.md), since Gaussian [moments](../../../probability-theory.md#moment) are finite at every finite time and the displayed conditional identities establish the [martingale](../../../martingale.md) property directly.

The choice is not unique. Constants $c,d,e\in\mathbb R$ give the valid family $\alpha(t)=c-3t$, $\beta(t)=d-6t$, and $\gamma(t)=3t^2-dt+e$: these add $cB_t$ to the cubic [martingale](../../../martingale.md) and $d(B_t^2-t)+e$ to the quartic one. The boxed choice sets these harmless additions to zero.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Write $\tau=\tau_x$ and $T_t=t\wedge\tau$. Path continuity gives $|B_{T_t}|\leq x$. Stop the [martingale](../../../martingale.md) $B_s^2-s$ at the bounded [stopping time](../../../martingale.md#stopping-time) $T_t$ and apply the [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale):

$$
\mathbb E T_t=\mathbb E B_{T_t}^2\leq x^2.
$$

By the [monotone convergence theorem](../../../measure-theory.md#monotone-convergence-theorem), $\mathbb E\tau\leq x^2$, so $\tau<\infty$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Path continuity then gives $B_\tau\in\{-x,x\}$. The [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) for the bounded variables $B_{T_t}^2$ shows

$$
\boxed{\mathbb E\tau_x=x^2.}
$$

Next stop the quartic [Hermite polynomial martingale](../../../numerical-analysis.md#space-time-hermite-polynomial) from part (a), again only at $T_t$. Its [expectation](../../../probability-theory.md#expected-value) is zero, so

$$
3\mathbb E T_t^2
=6\mathbb E[T_tB_{T_t}^2]-\mathbb E B_{T_t}^4
\leq6x^2\mathbb E T_t\leq6x^4.
$$

[Monotone convergence](../../../measure-theory.md#monotone-convergence-theorem) proves $\mathbb E\tau^2\leq2x^4$, establishing the needed second-moment integrability before the final passage to the limit. Since $T_tB_{T_t}^2\leq x^2\tau$ and $B_{T_t}^4\leq x^4$, [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem) gives

$$
3\mathbb E\tau^2=6x^2\mathbb E\tau-x^4=5x^4.
$$

Consequently the [Brownian symmetric interval-exit moments](../../../brownian-motion.md#brownian-symmetric-interval-exit-moments) are

$$
\boxed{\mathbb E\tau_x^2=\frac53x^4,\qquad
\operatorname{Var}(\tau_x)=\frac23x^4.}
$$

To obtain the [Laplace transform of symmetric Brownian interval-exit time](../../../brownian-motion.md#laplace-transform-of-symmetric-brownian-interval-exit-time), put $a=\sqrt{2\lambda}$. The [Exponential martingale for Brownian motion](../../../brownian-motion.md#exponential-martingale-for-brownian-motion) shows that

$$
H_t=e^{-\lambda t}\cosh(aB_t)
=\tfrac12\bigl(e^{aB_t-a^2t/2}+e^{-aB_t-a^2t/2}\bigr)
$$

is a [martingale](../../../martingale.md) with $H_0=1$. Bounded-time stopping gives $\mathbb E H_{T_t}=1$. Its stopped values are bounded by $\cosh(ax)$, so [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem) applies as $t\to\infty$. Since $\cosh(aB_\tau)=\cosh(ax)$, it yields

$$
\boxed{\mathbb E[e^{-\lambda\tau_x}]
=\frac1{\cosh(x\sqrt{2\lambda})}\quad(\lambda>0).}
$$

Every use of stopping at $\tau$ has thus been justified through bounded stopping and an explicit integrability or domination argument.

## 4

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A [version of a stochastic process](../../../stochastic-process.md#modification-of-a-stochastic-process) means a [stochastic process](../../../stochastic-process.md) on the same probability space such that, for every fixed $t$,

$$
\mathbb P(X_t=Y_t)=1.
$$

The exceptional [null set](../../../measure-theory.md#null-set) may depend on $t$. [Indistinguishability of stochastic processes](../../../stochastic-process.md#indistinguishability-of-stochastic-processes) means that there is one [null set](../../../measure-theory.md#null-set) outside which $X_t=Y_t$ for all $t\geq0$ simultaneously.

For an example separating the definitions, let $U$ have [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) on $(0,1)$, and set

$$
X_t=0,\qquad Y_t=\mathbf1_{\{t=U\}},\qquad t\geq0.
$$

For every fixed $t$, $\mathbb P(U=t)=0$, so $Y$ is a [version of a stochastic process](../../../stochastic-process.md#modification-of-a-stochastic-process) with original [stochastic process](../../../stochastic-process.md) $X$. But for every sample outcome the [stochastic processes](../../../stochastic-process.md) differ at its time $t=U$. Hence

$$
\boxed{\mathbb P(X_t=Y_t\text{ for every }t\geq0)=0.}
$$

The spike path of $Y$ is not [right-continuous](../../../calculus.md#right-continuous-function) at $U$, which explains why the next part's regularity assumption rules out this example.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For each nonnegative rational $q$, equality of the two versions gives $\mathbb P(X_q=Y_q)=1$. Intersect these countably many full-probability events with the full-probability event on which both paths are [càdlàg](../../../calculus.md#cadlag). Call the resulting event $A$; then $\mathbb P(A)=1$.

Fix $\omega\in A$ and any real $t\geq0$. Choose rational numbers $q_n>t$ decreasing to $t$. [Right continuity](../../../calculus.md#right-continuous-function) gives

$$
X_t(\omega)=\lim_nX_{q_n}(\omega)
=\lim_nY_{q_n}(\omega)=Y_t(\omega).
$$

The same event $A$ works for every $t$, because the argument is pathwise after $\omega$ is fixed. **The [stochastic processes](../../../stochastic-process.md) are therefore [indistinguishable](../../../stochastic-process.md#indistinguishability-of-stochastic-processes).** This proves that [càdlàg versions are indistinguishable](../../../stochastic-process.md#cadlag-versions-are-indistinguishable); the left limits are not needed for this implication, since [right continuity](../../../calculus.md#right-continuous-function) alone suffices.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Relative to a [filtration](../../../stochastic-process.md#filtration-probability-theory) $(\mathcal F_t)$, [progressive measurability](../../../stochastic-process.md#progressive-measurability) means that, for every $T<\infty$, the map

$$
[0,T]\times\Omega\longrightarrow\mathbb R,\qquad (t,\omega)\longmapsto X_t(\omega)
$$

is measurable for the [product sigma-algebra](../../../probability-theory.md#product-sigma-algebra) $\mathcal B([0,T])\otimes\mathcal F_T$ and the [Borel sigma-algebra](../../../measure-theory.md#borel-sigma-algebra) on $\mathbb R$.

Fix $T>0$ and divide $[0,T]$ into $2^m$ equal subintervals with mesh $h_m=T/2^m$. Define

$$
X^{(m)}_t=
\sum_{k=1}^{2^m}X_{kh_m}\mathbf1_{[(k-1)h_m,kh_m)}(t)
+X_T\mathbf1_{\{T\}}(t).
$$

Since $X$ is [adapted](../../../stochastic-process.md#adapted-process), every [random variable](../../../random-variable.md) $X_{kh_m}$ is $\mathcal F_{kh_m}$-measurable, hence $\mathcal F_T$-measurable. Each approximation is consequently $\mathcal B([0,T])\otimes\mathcal F_T$-measurable. For $t<T$, its sampling time lies strictly to the right of $t$, tends to $t$, and never exceeds $T$. [Right continuity](../../../calculus.md#right-continuous-function) implies $X^{(m)}_t\to X_t$; at $T$ equality is exact. Thus $X$ is the pointwise limit of measurable functions on this product space. As $T$ was arbitrary, **$X$ is [progressively measurable](../../../stochastic-process.md#progressive-measurability)**. This is the theorem that [right-continuous adapted processes are progressively measurable](../../../stochastic-process.md#right-continuous-adapted-processes-are-progressively-measurable).

The right-endpoint approximations need not themselves be adapted at their intermediate times. What the proof requires is their joint measurability with respect to the single terminal sigma-algebra $\mathcal F_T$. The proof uses the pathwise [càdlàg](../../../calculus.md#cadlag) convention. If path regularity is assumed only [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), under a completed filtration setting the [stochastic process](../../../stochastic-process.md) to zero on its common exceptional null event gives an [indistinguishable](../../../stochastic-process.md#indistinguishability-of-stochastic-processes) [progressively measurable](../../../stochastic-process.md#progressive-measurability) version. Arbitrary values on that null event need not make the original [stochastic process](../../../stochastic-process.md) [progressively measurable](../../../stochastic-process.md#progressive-measurability): even with a complete filtration, a null sample point may be assigned a non-Borel time function. This is why [almost sure path regularity does not ensure progressive measurability](../../../stochastic-process.md#almost-sure-path-regularity-does-not-ensure-progressive-measurability).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Fix $t$ and put $\sigma=t\wedge\tau$. The [stopping time](../../../martingale.md#stopping-time) property implies that $\sigma$ is an $\mathcal F_t$-measurable [random variable](../../../random-variable.md) with values in $[0,t]$: for $s<t$,

$$
\{\sigma\leq s\}=\{\tau\leq s\}\in\mathcal F_s\subseteq\mathcal F_t,
$$

and for $s\geq t$ the event is the whole space. By part (c), the restriction of $X$ to $[0,t]\times\Omega$ is $\mathcal B([0,t])\otimes\mathcal F_t$-measurable.

The evaluation map $\omega\mapsto(\sigma(\omega),\omega)$ is measurable from $(\Omega,\mathcal F_t)$ to this product space: the inverse image of a measurable rectangle $A\times C$ is $\{\sigma\in A\}\cap C$. Composing it with the jointly measurable [stochastic process](../../../stochastic-process.md) gives an $\mathcal F_t$-measurable [random variable](../../../random-variable.md)

$$
X^\tau_t=X_{t\wedge\tau}.
$$

Since this holds for every fixed $t$, **the [stopped process](../../../martingale.md#stopped-process) is adapted**. If path regularity holds only [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), first apply the proof to its pathwise regular representative; with a completed filtration, the original stopped variable differs only on a null event and is also $\mathcal F_t$-measurable. The [adaptedness of a stopped right-continuous process](../../../stochastic-process.md#adaptedness-of-a-stopped-right-continuous-process) requires neither boundedness of $\tau$ nor a [martingale](../../../martingale.md) assumption; $\tau=\infty$ is harmless because $t\wedge\tau\leq t$.

## 5

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The [Skorokhod embedding of a centered random walk](../../../martingale.md#skorokhod-embedding-of-a-centered-random-walk) states that a [random walk](../../../markov-process.md#random-walk) with independent identically distributed centered steps of finite [variance](../../../variance.md) $\sigma^2$ can be realized on an appropriate probability space as

$$
S_n=B_{T_n},\qquad 0=T_0\leq T_1\leq T_2\leq\cdots,
$$

where $B$ is a standard [Brownian motion](../../../brownian-motion.md) and the $T_n$ are finite [stopping times](../../../martingale.md#stopping-time). More precisely, the stopped positions have the same joint law as the given [random walk](../../../markov-process.md#random-walk), and the pairs

$$
(T_n-T_{n-1},\,B_{T_n}-B_{T_{n-1}}),\qquad n\geq1,
$$

may be chosen independent and identically distributed. Their spatial component has the step law, and $\mathbb E(T_n-T_{n-1})=\sigma^2$. Repeating the one-step [Skorokhod embedding theorem](../../../martingale.md#skorokhod-embedding-theorem) with the [Strong Markov property](../../../markov-process.md#strong-markov-property) gives this formulation. In the present normalization, the mean time increment is one, and the [strong law of large numbers](../../../convergence-of-random-variables.md#strong-law-of-large-numbers) gives $T_n/n\to1$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence).

The [Donsker invariance principle](../../../convergence-of-random-variables.md#donsker-s-theorem) states that the linearly interpolated diffusively rescaled [random walk](../../../markov-process.md#random-walk)

$$
W_n(t)=\frac{S_{\lfloor nt\rfloor}
+(nt-\lfloor nt\rfloor)X_{\lfloor nt\rfloor+1}}{\sqrt n},
\qquad 0\leq t\leq1,\qquad S_0=0,
$$

converges weakly as a random element of $C[0,1]$, equipped with the [uniform norm](../../../functional-analysis.md#supremum-norm), to standard [Brownian motion](../../../brownian-motion.md) restricted to $[0,1]$. At $t=1$ the fractional term is zero. The only step assumptions needed here are zero mean, unit [variance](../../../variance.md), and independent identical distributions; a higher moment or bounded support is not required. This is a [functional central limit theorem](../../../convergence-of-random-variables.md#donsker-s-theorem), concerning the entire interpolated path rather than only its endpoint.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Let $W_n$ be the interpolation in part (a). The operation

$$
I:C[0,1]\longrightarrow\mathbb R,\qquad I(f)=\int_0^1f(t)\,dt
$$

is continuous, since $|I(f)-I(g)|\leq\|f-g\|_\infty$. By the [Donsker invariance principle](../../../convergence-of-random-variables.md#donsker-s-theorem) and the [continuous mapping theorem](../../../convergence-of-random-variables.md#continuous-mapping-theorem),

$$
I(W_n)\xrightarrow{\ d\ }\int_0^1B_t\,dt.
$$

The exact trapezoidal integral of the linear interpolation is

$$
I(W_n)=\frac1{n^{3/2}}
\left(\sum_{k=1}^{n-1}S_k+\frac12S_n\right).
$$

Therefore the statistic in question differs from $I(W_n)$ by $S_n/(2n^{3/2})$. Using [independence](../../../random-variable.md#independent-random-variables), zero means, and unit variances gives

$$
\mathbb E\left[\left(\frac{S_n}{2n^{3/2}}\right)^2\right]
=\frac{n}{4n^3}=\frac1{4n^2}\longrightarrow0.
$$

This error tends to zero in $L^2$, hence in probability. The [Slutsky theorem](../../../statistical-inference.md#slutsky-theorem) now proves the [integrated random-walk limit](../../../convergence-of-random-variables.md#integrated-random-walk-limit):

$$
\boxed{\frac1{n^{3/2}}\sum_{k=1}^nS_k
\xrightarrow{\ d\ }\int_0^1B_t\,dt.}
$$

The limiting law can also be made explicit. The time integral is a Gaussian [random variable](../../../random-variable.md), as a mean-square limit of linear combinations of a [Gaussian process](../../../stochastic-process.md#gaussian-process). It is centered, and the [covariance](../../../variance.md#covariance) identity $\mathbb E(B_sB_t)=\min(s,t)$ gives

$$
\operatorname{Var}\left(\int_0^1B_t\,dt\right)
=\int_0^1\int_0^1\min(s,t)\,ds\,dt
=2\int_0^1\int_0^t s\,ds\,dt=\frac13.
$$

Thus the terminal value of [integrated Brownian motion](../../../brownian-motion.md#integrated-brownian-motion) here has law **$N(0,1/3)$**.

## 6

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Sample [Brownian motion](../../../brownian-motion.md) at integer times and put $Z_n=B_n/\sqrt n$. Every $Z_n$ has [normal distribution](../../../probability-theory.md#normal-distribution) $N(0,1)$, although the $Z_n$ are correlated. Let

$$
L=\limsup_{n\to\infty}Z_n.
$$

For every fixed integer $m$,

$$
L=\limsup_{n\to\infty}\frac{B_n-B_m}{\sqrt n},
$$

because $B_m/\sqrt n\to0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). The right-hand expression depends only on the future [independent increments](../../../stochastic-process.md#independent-increments) $B_{j}-B_{j-1}$ with $j>m$. Thus $\{L\geq a\}$ is, up to a [null set](../../../measure-theory.md#null-set), a [tail event](../../../probability-theory.md#tail-event) of those [independent increments](../../../stochastic-process.md#independent-increments), and its probability is zero or one by the [Kolmogorov zero-one law](../../../probability-theory.md#kolmogorov-s-zero-one-law).

For any finite real $a$, every $Z_n$ exceeds $a$ with the same positive probability $p_a=\mathbb P(N(0,1)\geq a)$. For each $N$,

$$
\mathbb P\left(\bigcup_{n\geq N}\{Z_n\geq a\}\right)\geq p_a.
$$

Taking the decreasing intersection over $N$ shows that $Z_n\geq a$ infinitely often with probability at least $p_a$. This event implies $L\geq a$, so $\mathbb P(L\geq a)>0$. The zero-one law makes it one. Intersecting over positive integers $a$ gives $L=+\infty$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). The continuous-time limit superior is at least the one along integers, hence

$$
\boxed{\limsup_{t\to\infty}\frac{B_t}{\sqrt t}=+\infty
\quad\text{almost surely}.}
$$

This proves that [Brownian fluctuations exceed the square-root scale](../../../brownian-motion.md#brownian-fluctuations-exceed-the-square-root-scale) without needing the lower bound in the law of the iterated logarithm.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

For $t>e$, put $\Phi(t)=\sqrt{2t\log\log t}$. Fix $a>1$ and $\varepsilon>0$, and set

$$
E_n=\left\{\sup_{0\leq s\leq a^n}B_s
\geq(1+\varepsilon)\Phi(a^n)\right\}
$$

for $n$ large enough that $a^n>e$. The [Brownian reflection principle](../../../brownian-motion.md#reflection-principle-wiener-process) and the Gaussian tail estimate give

$$
\begin{aligned}
\mathbb P(E_n)
&=2\mathbb P\left(B_{a^n}\geq(1+\varepsilon)\Phi(a^n)\right)\\
&\leq2\exp\bigl(-(1+\varepsilon)^2\log\log(a^n)\bigr)\\
&=2(n\log a)^{-(1+\varepsilon)^2}.
\end{aligned}
$$

Since $(1+\varepsilon)^2>1$, the sum of these probabilities is finite. The [Borel-Cantelli first lemma](../../../probability-theory.md#borel-cantelli-first-lemma) implies that, [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), for all sufficiently large $n$,

$$
\sup_{s\leq a^n}B_s<(1+\varepsilon)\Phi(a^n).
$$

Now take $t\in[a^{n-1},a^n]$. The function $\Phi$ is increasing for $t>e$, so

$$
\frac{B_t}{\Phi(t)}
\leq(1+\varepsilon)\frac{\Phi(a^n)}{\Phi(a^{n-1})}.
$$

Here the positive upper bound for $B_t$ can first be divided by $\Phi(t)$, and the denominator can then be bounded below by $\Phi(a^{n-1})$; this remains valid even when $B_t<0$. Moreover,

$$
\frac{\Phi(a^n)}{\Phi(a^{n-1})}
=\sqrt{a\,\frac{\log(n\log a)}{\log((n-1)\log a)}}
\longrightarrow\sqrt a.
$$

Thus, for each fixed pair $(a,\varepsilon)$,

$$
\limsup_{t\to\infty}\frac{B_t}{\Phi(t)}
\leq(1+\varepsilon)\sqrt a
\quad\text{almost surely}.
$$

Use the countable choices $a_m=1+1/m$ and $\varepsilon_m=1/m$, intersect their probability-one events, and let $m\to\infty$. This proves the [Brownian upper law of the iterated logarithm](../../../convergence-of-random-variables.md#brownian-upper-law-of-the-iterated-logarithm):

$$
\boxed{\limsup_{t\to\infty}\frac{B_t}{\sqrt{2t\log\log t}}
\leq1\quad\text{almost surely}.}
$$

Only large times are involved. The hint's related monotonicity assertion for $\Phi(t)/t$ is also valid eventually: the derivative of $2\log\log t/t$ is $2(1/\log t-\log\log t)/t^2$, which is negative for $t\geq e^e$. No monotonicity at the small-time edge of the logarithmic expression is required.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
