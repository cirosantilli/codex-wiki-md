# Paper 201

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_201.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_201.pdf)

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
  - [f](#1/f)
    - [Solution](#1/f/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
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
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)
  - [d](#6/d)
    - [i](#6/d/i)
      - [Solution](#6/d/i/solution)
    - [ii](#6/d/ii)
      - [Solution](#6/d/ii/solution)
    - [iii](#6/d/iii)
      - [Solution](#6/d/iii/solution)
    - [iv](#6/d/iv)
      - [Solution](#6/d/iv/solution)

## 1

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For an integrable [random variable](../../../random-variable.md) $X$ and a sub-sigma-algebra $\mathcal G\subseteq\mathcal F$, the [conditional expectation](../../../measure-theory.md#conditional-expectation) $Y=\mathbb E[X\mid\mathcal G]$ is an integrable, $\mathcal G$-measurable random variable satisfying

$$
\int_GY\,d\mathbb P=\int_GX\,d\mathbb P
$$

for every $G\in\mathcal G$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Conditional expectation is unique up to [almost sure equality](../../../convergence-of-random-variables.md#almost-sure-equality). If $Y$ and $Z$ both satisfy the definition, then for every $G\in\mathcal G$,

$$
\int_G(Y-Z)\,d\mathbb P=0.
$$

The events $\{Y>Z\}$ and $\{Z>Y\}$ belong to $\mathcal G$. Testing on them, or first on $\{Y-Z\geq1/k\}$ and $\{Z-Y\geq1/k\}$, shows that both have probability zero. Hence $Y=Z$ almost surely.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

If $G\in\mathcal G\cap\mathcal H$, independence makes $G$ independent of itself, so

$$
\mathbb P(G)=\mathbb P(G)^2.
$$

Thus every event in $\mathcal G\cap\mathcal H$ has probability zero or one. The intersection is trivial modulo null sets, and the [independent sigma-algebras have trivial intersection](../../../measure-theory.md#independent-sigma-algebras-have-trivial-intersection) result gives

$$
\boxed{\mathbb E[X\mid\mathcal G\cap\mathcal H]=\mathbb E[X]}
$$

almost surely.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Put $S=X_1+X_2$. By symmetry,

$$
\mathbb E[X_1\mid S]=\mathbb E[X_2\mid S].
$$

Their sum is $S$, which is measurable with respect to $\mathcal G=\sigma(S)$, so

$$
2\mathbb E[X_1\mid\mathcal G]
=\mathbb E[X_1+X_2\mid\mathcal G]
=S.
$$

Therefore

$$
\boxed{\mathbb E[X_1\mid\mathcal G]=\frac{X_1+X_2}{2}}.
$$

This also follows from the [Gaussian conditional expectation](../../../statistical-modelling.md#gaussian-conditional-expectation) formula because $\operatorname{Cov}(X_1,S)/\operatorname{Var}(S)=1/2$.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

If $\mathcal G\subseteq\mathcal H$, then $\mathbb E[X\mid\mathcal G]$ is already $\mathcal H$-measurable, so

$$
\mathbb E[\mathbb E[X\mid\mathcal G]\mid\mathcal H]
=\mathbb E[X\mid\mathcal G]
=\mathbb E[X\mid\mathcal G\cap\mathcal H].
$$

If $\mathcal H\subseteq\mathcal G$, the [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation) gives

$$
\mathbb E[\mathbb E[X\mid\mathcal G]\mid\mathcal H]
=\mathbb E[X\mid\mathcal H]
=\mathbb E[X\mid\mathcal G\cap\mathcal H].
$$

Finally, if $\mathcal G$ and $\mathcal H$ are independent, the $\mathcal G$-measurable variable $\mathbb E[X\mid\mathcal G]$ is independent of $\mathcal H$. Its conditional expectation given $\mathcal H$ is its mean $\mathbb E[X]$. Part c shows that the right side is also $\mathbb E[X]$.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

The equation fails for general nonnested sigma-algebras. On the four-point space $\Omega=\{1,2,3,4\}$ with uniform probability, let

$$
A=\{1,2\},\qquad B=\{1,2,3\},
\qquad \mathcal G=\sigma(A),\qquad\mathcal H=\sigma(B),
$$

and take $X=\mathbf1_A$. The intersection $\mathcal G\cap\mathcal H$ is trivial, so

$$
\mathbb E[X\mid\mathcal G\cap\mathcal H]=\frac12.
$$

But $X$ is $\mathcal G$-measurable and

$$
\mathbb E[\mathbb E[X\mid\mathcal G]\mid\mathcal H]
=\mathbb E[X\mid\mathcal H]
=\frac23\mathbf1_B,
$$

which is zero on $B^c$ and is not almost surely $1/2$. This exhibits the failure of [iterated conditional expectation over nonnested sigma-algebras](../../../measure-theory.md#iterated-conditional-expectation-over-nonnested-sigma-algebras).

## 2

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For a finite horizon $N$, let $U_N[a,b]$ be the number of completed upcrossings by time $N$. Use the predictable strategy that holds one unit of the process after a visit below $a$ until the next visit above $b$. For a [supermartingale](../../../martingale.md#supermartingale), the expected gain of this nonnegative predictable [martingale transform](../../../martingale.md#martingale-transform) is nonpositive. Pathwise, the completed trades earn at least $(b-a)U_N[a,b]$, while an unfinished final trade can lose at most $(X_N-a)^-$. Hence

$$
(b-a)U_N[a,b]\leq (X_N-a)^-+(H\mathbin\cdot X)_N.
$$

Taking expectations and using $X_N\geq0$ gives the [Doob upcrossing inequality](../../../martingale.md#doob-upcrossing-inequality)

$$
(b-a)\mathbb E U_N[a,b]
\leq\mathbb E(X_N-a)^-
\leq a.
$$

As $N\to\infty$, monotone convergence yields

$$
\boxed{\mathbb E U[a,b]\leq\frac a{b-a}}.
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For every rational $0\leq a<b$, part a implies $U[a,b]<\infty$ almost surely. The intersection of these probability-one events over the countable collection of rational pairs still has probability one. On this event, if

$$
\liminf_nX_n<\limsup_nX_n,
$$

some rational interval $[a,b]$ lies strictly between them, forcing infinitely many upcrossings, a contradiction. Thus $X_n$ has an extended limit almost surely.

The limit cannot be $+\infty$ on a set of positive probability: [Fatou lemma](../../../measure-theory.md#fatou-s-lemma) and the [supermartingale](../../../martingale.md#supermartingale) property give

$$
\mathbb E[\liminf_nX_n]
\leq\liminf_n\mathbb E X_n
\leq\mathbb E X_0<\infty.
$$

Nonnegativity excludes $-\infty$. Therefore $X_n$ converges almost surely to a finite random variable, proving the [almost sure supermartingale convergence theorem](../../../martingale.md#almost-sure-supermartingale-convergence-theorem) in this case.

## 3

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

If $\xi_k=S_k-S_{k-1}$, then

$$
\mu=\mathbb E\xi_k=p-(1-p)=2p-1.
$$

The centered increments $\xi_k-\mu$ are independent of the past and have mean zero, so

$$
\boxed{M_n=S_n-\mu n}
$$

is a [martingale](../../../martingale.md).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The increment variance is

$$
\operatorname{Var}(\xi_k)=1-(2p-1)^2=4p(1-p),
$$

so independence gives

$$
\operatorname{Var}(S_n)=4np(1-p).
$$

Linear interpolation makes the supremum of the absolute centered process occur at an integer time. The [Doob L2 maximal inequality](../../../martingale.md#doob-l2-maximal-inequality) therefore gives

$$
\begin{aligned}
\mathbb E\sup_{0\leq t\leq1}|S_t^{(n)}-\mu t|^2
&=\frac1{n^2}\mathbb E\max_{0\leq k\leq n}|M_k|^2\\
&\leq\frac4{n^2}\mathbb E M_n^2
=\frac{16p(1-p)}n
\leq\boxed{\frac4n}.
\end{aligned}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The moment-generating function of one increment is

$$
\mathbb E e^{\theta\xi_1}=pe^\theta+(1-p)e^{-\theta}.
$$

Thus with

$$
\boxed{\psi(\theta)=\log(pe^\theta+(1-p)e^{-\theta})},
$$

independence gives

$$
\mathbb E[Z_{n+1}\mid\mathcal F_n]
=Z_n e^{-\psi(\theta)}\mathbb E e^{\theta\xi_{n+1}}
=Z_n.
$$

This is the [exponential martingale of a biased simple random walk](../../../probability-theory.md#exponential-martingale-of-a-biased-simple-random-walk).

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Let

$$
T=\inf\{k\leq n:S_k-\mu k\geq\varepsilon n\}\wedge n.
$$

On $A$, one has $T\leq n$, $S_T\geq\mu T+\varepsilon n$, and convexity of $\psi$ gives $\psi(\theta)-\mu\theta\geq0$. Hence for $\theta>0$,

$$
Z_T
=e^{\theta(S_T-\mu T)-(\psi(\theta)-\mu\theta)T}
\geq e^{(\theta(\mu+\varepsilon)-\psi(\theta))n}.
$$

The [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) applies because $T$ is bounded, so $\mathbb EZ_T=1$. Therefore

$$
\boxed{\mathbb P(A)\leq e^{-(\theta(\mu+\varepsilon)-\psi(\theta))n}}.
$$

Optimize over $\theta>0$ for the upper deviation and apply the same argument with $\theta<0$ to the lower deviation. Since the supremum of the linearly interpolated centered walk is attained at grid points, the [Legendre transform of a cumulant-generating function](../../../probability-theory.md#legendre-transform-of-a-cumulant-generating-function)

$$
\psi^*(x)=\sup_{\theta\in\mathbb R}(\theta x-\psi(\theta))
$$

and the [union bound](../../../probability-inequality.md#boole-s-inequality) give

$$
\boxed{
\mathbb P\left(\sup_{0\leq t\leq1}|S_t^{(n)}-\mu t|\geq\varepsilon\right)
\leq e^{-n\psi^*(\mu+\varepsilon)}+e^{-n\psi^*(\mu-\varepsilon)}.}
$$

## 4

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A process $(X_t)_{t\geq0}$ is [Brownian motion](../../../brownian-motion.md) in $\mathbb R^d$ when $X_0=0$, its paths are almost surely continuous, and for $0\leq t_0<\cdots<t_k$ the increments $X_{t_j}-X_{t_{j-1}}$ are independent centered [Gaussian vectors](../../../probability-and-statistics.md#multivariate-normal-distribution) with covariance $(t_j-t_{j-1})I_d$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The paths of $UX_t$ are continuous and start at zero. Its increments are independent because they are deterministic functions of the independent increments of $X$. They are centered Gaussian, and orthogonality gives

$$
\operatorname{Cov}(U(X_t-X_s))
=U((t-s)I_d)U^T
=(t-s)I_d.
$$

**Thus $UX$ is Brownian motion. This is the [orthogonal invariance of Brownian motion](../../../brownian-motion.md#orthogonal-invariance-of-brownian-motion).**

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Apply the orthogonal transformation

$$
D_t=\frac{A_t^+-A_t^-}{\sqrt2},
\qquad
C_t=\frac{A_t^++A_t^-}{\sqrt2}.
$$

The processes $D$ and $C$ are independent one-dimensional Brownian motions, with $D_0=\sqrt2a$ and $C_0=0$. The meeting time is the first time $D$ hits zero, which is almost surely finite by one-dimensional Brownian recurrence.

The [Brownian reflection principle](../../../brownian-motion.md#reflection-principle-wiener-process) gives the first-passage density from $x>0$ to zero as

$$
\frac{x}{\sqrt{2\pi u^3}}e^{-x^2/(2u)}.
$$

Substituting $x=\sqrt2a$ gives the [meeting time of two independent Brownian motions](../../../brownian-motion.md#meeting-time-of-two-independent-brownian-motions) density

$$
\boxed{f_T(u)=\frac a{\sqrt{\pi u^3}}e^{-a^2/u}},
\qquad u>0.
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

At the meeting time,

$$
A_T^+=A_T^-=\frac{C_T}{\sqrt2}.
$$

The process $C$ is independent of $T$, so conditional on $T=u$ the meeting position is $N(0,u/2)$. Independently, $B_t-B_u$ is $N(0,t-u)$. Therefore

$$
Z_t\mid\{T=u\}\sim N(0,t-u/2).
$$

For $0<s\leq t$, integrate this conditional [Gaussian distribution](../../../probability-theory.md#normal-distribution) against the density from part c:

$$
\boxed{
\mathbb P(T\leq s,\ Z_t\leq z)
=\int_0^s
\Phi\left(\frac z{\sqrt{t-u/2}}\right)
\frac a{\sqrt{\pi u^3}}e^{-a^2/u}\,du.}
$$

## 5

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The random-walk form of the [Skorokhod embedding theorem](../../../martingale.md#skorokhod-embedding-theorem) says the following. If $S_n=Y_1+\cdots+Y_n$, where the $Y_i$ are independent and identically distributed with

$$
\mathbb EY_i=0,
\qquad
\mathbb EY_i^2=\sigma^2<\infty,
$$

then on a space carrying a Brownian motion $B$ there are stopping times

$$
0=T_0\leq T_1\leq\cdots
$$

such that $(B_{T_n})_{n\geq0}$ has the same law as $(S_n)_{n\geq0}$, and the increments $T_n-T_{n-1}$ are independent and identically distributed with mean $\sigma^2$.

To prove the one-step statement, first note that every centered distribution is a mixture of centered two-point distributions. Indeed, match the equal-mass size-biased measures $x\,\mathbb P(Y\in dx)$ on $(0,\infty)$ and $|x|\,\mathbb P(Y\in dx)$ on $(-\infty,0)$. This produces a random pair $(L,R)$ of positive numbers such that, conditionally on $(L,R)$, $Y$ has values $-L,R$ with probabilities

$$
\frac R{L+R},\qquad\frac L{L+R},
$$

and $\mathbb E[LR]=\mathbb EY^2=\sigma^2$. Include the atom at zero by taking the stopping time zero.

Choose $(L,R)$ independently of $B_t$ and stop Brownian motion on first leaving $(-L,R)$. The [Brownian exit from an interval](../../../brownian-motion.md#brownian-exit-from-an-interval) formulas give the displayed two-point probabilities and conditional mean stopping time $LR$. Thus $B_T$ has the law of $Y$ and $\mathbb ET=\sigma^2$.

Starting from $T_0=0$, repeat this construction after each $T_{n-1}$. The [Strong Markov property](../../../markov-process.md#strong-markov-property) makes the new Brownian increments independent copies of the first embedding, proving the [Skorokhod embedding of a centered random walk](../../../martingale.md#skorokhod-embedding-of-a-centered-random-walk).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

By the [strong law of large numbers](../../../convergence-of-random-variables.md#strong-law-of-large-numbers),

$$
\frac{T_n}{n}\longrightarrow\sigma^2
$$

almost surely. Brownian scaling and a maximal inequality show that changing Brownian time by $o(n)$ changes its value by $o_{\mathbb P}(\sqrt n)$; explicitly, first restrict to $|T_n-n\sigma^2|\leq\delta n$, bound the Brownian maximum over a time interval of length $2\delta n$, and then let $\delta\downarrow0$. Consequently

$$
\frac{B_{T_n}-B_{n\sigma^2}}{\sqrt n}\longrightarrow0
$$

in probability.

But

$$
\frac{B_{n\sigma^2}}{\sqrt n}\sim N(0,\sigma^2)
$$

for every $n$. Since $B_{T_n}$ has the law of $S_n$, [Slutsky theorem](../../../statistical-inference.md#slutsky-theorem) proves the [Central limit theorem from the Skorokhod embedding](../../../martingale.md#central-limit-theorem-from-the-skorokhod-embedding):

$$
\boxed{\frac{S_n}{\sqrt n}\ \xrightarrow{d}\ N(0,\sigma^2)}.
$$

## 6

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

A real [Lévy process](../../../stochastic-process.md#levy-process) satisfies $X_0=0$ almost surely, has stationary independent increments, is [stochastically continuous](../../../stochastic-process.md#stochastic-continuity), and is taken in its almost surely càdlàg version.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

The [Lévy–Khintchine theorem](../../../stochastic-process.md#levy-khintchine-formula) states that there is a unique triplet $(a,b,K)$, where $a\in\mathbb R$, $b\geq0$, and $K$ is a measure on $\mathbb R\setminus\{0\}$ satisfying

$$
\int_{\mathbb R}(1\wedge x^2)K(dx)<\infty,
$$

such that

$$
\boxed{
\mathbb E e^{iuX_t}
=\exp\left\{t\left(iua-\frac12bu^2
+\int_{\mathbb R\setminus\{0\}}
(e^{iux}-1-iux\mathbf1_{\{|x|\leq1\}})K(dx)
\right)\right\}.}
$$

Conversely every such triplet is the characteristic triplet of a Lévy process.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Let $B$ be Brownian motion and let $N(ds,dx)$ be an independent [Poisson random measure](../../../probability-theory.md#poisson-random-measure) with intensity $ds\,K(dx)$. Writing $\widetilde N=N-ds\,K(dx)$ for its compensated version, the [Lévy–Itô decomposition](../../../stochastic-process.md#levy-ito-decomposition) constructs

$$
\boxed{
X_t=at+\sqrt b B_t
+\int_0^t\!\int_{|x|\leq1}x\,\widetilde N(ds,dx)
+\int_0^t\!\int_{|x|>1}x\,N(ds,dx).}
$$

The four terms are independent drift, Gaussian, compensated small-jump and compound-Poisson large-jump components.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/i">i</h4>

↑ **Parent:** [D](#6/d)

<h5 id="6/d/i/solution">Solution</h5>

↑ **Parent:** [I](#6/d/i)

Almost surely differentiable paths must be continuous, so the jump measure must vanish: $K=0$. A nonzero Brownian component has almost surely nowhere-differentiable paths, so also $b=0$. Conversely, if $b=0$ and $K=0$, then $X_t=at$ is differentiable. Thus

$$
\boxed{b=0\text{ and }K=0}.
$$

<h4 id="6/d/ii">ii</h4>

↑ **Parent:** [D](#6/d)

<h5 id="6/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/d/ii)

The Brownian and drift components are continuous. Any nonzero Lévy measure produces jumps: a set bounded away from zero with positive finite $K$-measure gives a nontrivial compound Poisson component, and increasing such sets detects every nonzero $K$. Hence paths are almost surely continuous exactly when

$$
\boxed{K=0}.
$$

<h4 id="6/d/iii">iii</h4>

↑ **Parent:** [D](#6/d)

<h5 id="6/d/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#6/d/iii)

The compensated small-jump integral is integrable after localization and has mean zero, while the number of large jumps on a compact time interval is finite. Its absolute first moment is finite exactly when the large-jump sizes have finite first moment. Thus $(X_t)$ is integrable exactly when

$$
\boxed{\int_{|x|>1}|x|\,K(dx)<\infty}.
$$

<h4 id="6/d/iv">iv</h4>

↑ **Parent:** [D](#6/d)

<h5 id="6/d/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#6/d/iv)

The Brownian component has finite variance $bt$, and the compensated jump integral has variance

$$
t\int x^2K(dx)
$$

when this integral is finite. Conversely, a finite second moment forces the jump measure to have a finite second moment. Therefore $(X_t^2)$ is integrable exactly when

$$
\boxed{\int_{\mathbb R}x^2K(dx)<\infty}.
$$

These four equivalences are the [Path and moment criteria from a Lévy triplet](../../../stochastic-process.md#path-and-moment-criteria-from-a-levy-triplet).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
