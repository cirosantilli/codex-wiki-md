# Paper 201

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_201.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_201.pdf)

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
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
    - [iii](#4/b/iii)
      - [Solution](#4/b/iii/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)

## 1

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For the [simple symmetric random walk](../../../probability-theory.md#simple-symmetric-random-walk), $S_n$ is a martingale and the [square-minus-time martingale of a simple symmetric random walk](../../../probability-theory.md#square-minus-time-martingale-of-a-simple-symmetric-random-walk) is

$$
M_n=S_n^2-n
$$

Indeed, conditioning on $\mathcal F_n$ and using $\mathbb E[X_{n+1}]=0$ and $X_{n+1}^2=1$ gives $\mathbb E[S_{n+1}^2\mid\mathcal F_n]=S_n^2+1$.

Apply the [optional sampling theorem for a supermartingale](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) to the bounded [stopping time](../../../martingale.md#stopping-time) $T\wedge n$:

$$
\mathbb E[S_{T\wedge n}^2]=\mathbb E[T\wedge n]\leq\mathbb E[T].
$$

Thus the stopped martingale $(S_{T\wedge n})$ is bounded in $L^2$. The [L2 martingale convergence theorem](../../../martingale.md#l2-martingale-convergence-theorem) gives convergence in $L^2$, and because $T<\infty$ almost surely its limit is $S_T$. Meanwhile the [monotone convergence theorem](../../../measure-theory.md#monotone-convergence-theorem) gives $\mathbb E[T\wedge n]\to\mathbb E[T]$. Therefore

$$
\mathbb E[S_T^2]=\mathbb E[T].
$$

Finite mean is essential. Let $T=\inf\{n\geq1:S_n=0\}$ be the first return to zero. The one-dimensional [simple symmetric random walk](../../../probability-theory.md#simple-symmetric-random-walk) is recurrent, so $T<\infty$ almost surely, but its first-return time has infinite mean. Since $S_T=0$,

$$
\boxed{\mathbb E[S_T^2]=0\ne\infty=\mathbb E[T].}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [law of the iterated logarithm for a simple symmetric random walk](../../../convergence-of-random-variables.md#law-of-the-iterated-logarithm-for-a-simple-symmetric-random-walk) states that almost surely

$$
\limsup_{n\to\infty}\frac{|S_n|}{\sqrt{2n\log\log n}}=1.
$$

Since $\sqrt{2\log\log n}$ is unbounded, $|S_n|/\sqrt n$ exceeds every fixed $c>0$ at some finite time. Hence

$$
T_c=\inf\{n\geq0:|S_n|>c\sqrt n\}<\infty
$$

almost surely.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Suppose $c>1$ and $\mathbb E[T_c]<\infty$. Part (a) would give

$$
\mathbb E[S_{T_c}^2]=\mathbb E[T_c].
$$

But $T_c\geq1$ and its defining strict inequality gives $S_{T_c}^2>c^2T_c$ almost surely. Taking expectations would yield

$$
\mathbb E[T_c]>c^2\mathbb E[T_c],
$$

which is impossible because $c^2>1$. Part (b) shows that $T_c$ is nevertheless finite almost surely. Consequently

$$
\boxed{\mathbb E[T_c]=\infty.}
$$

## 2

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

[Weak convergence of probability measures](../../../convergence-of-random-variables.md#weak-convergence-of-probability-measures) $\mu_n\to\mu$ on a [metric space](../../../topological-analysis.md#metric-space) means that

$$
\int f\,d\mu_n\longrightarrow\int f\,d\mu
$$

for every bounded continuous real function $f$. [Weak convergence of random variables](../../../convergence-of-random-variables.md#convergence-in-distribution) means weak convergence of their [probability distributions](../../../probability-theory.md#probability-distribution); equivalently,

$$
\mathbb E[f(X_n)]\longrightarrow\mathbb E[f(X)]
$$

for every bounded continuous $f$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For a bounded measurable $f$, the dual estimate for [total variation distance](../../../probability-and-statistics.md#total-variation-distance) gives

$$
\left|\int f\,d\mu_n-\int f\,d\mu\right|
\leq2\lVert f\rVert_\infty
\sup_A|\mu_n(A)-\mu(A)|.
$$

The right-hand side tends to zero, so in particular the integrals converge for every bounded continuous $f$. Thus [weak convergence of random variables](../../../convergence-of-random-variables.md#convergence-in-distribution) follows.

The converse fails. On $\mathbb R$, let $\mu_n=\delta_{1/n}$ and $\mu=\delta_0$. Continuity gives $f(1/n)\to f(0)$, so $\mu_n$ converges weakly to $\mu$. However, for $A=\{0\}$,

$$
|\mu_n(A)-\mu(A)|=1
$$

for every $n$, so there is no convergence in [total variation distance](../../../probability-and-statistics.md#total-variation-distance).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Assume first that $X_n\xrightarrow dX$. Because all variables take values in the compact interval $[-C,C]$, each monomial $x^k$ agrees there with a bounded continuous function on $\mathbb R$. The [bounded moment criterion for weak convergence](../../../convergence-of-random-variables.md#bounded-moment-criterion-for-weak-convergence) in this case begins with

$$
\mathbb E[X_n^k]\longrightarrow\mathbb E[X^k]
$$

for every natural number $k$.

Conversely, suppose all moments converge. Let $f$ be bounded and continuous. By the [Weierstrass approximation theorem](../../../functional-analysis.md#weierstrass-approximation-theorem), for every $\varepsilon>0$ there is a polynomial $P$ with

$$
\sup_{|x|\leq C}|f(x)-P(x)|\leq\varepsilon.
$$

Moment convergence implies $\mathbb E[P(X_n)]\to\mathbb E[P(X)]$, while

$$
|\mathbb E[f(X_n)-P(X_n)]|leq\varepsilon,
\qquad
|\mathbb E[f(X)-P(X)]|\leq\varepsilon.
$$

Taking the limit superior and then $\varepsilon\downarrow0$ proves $\mathbb E[f(X_n)]\to\mathbb E[f(X)]$, which is [convergence in distribution](../../../convergence-of-random-variables.md#convergence-in-distribution).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Let $g:M'\to\mathbb R$ be bounded and continuous. The composition $h=g\circ f$ is bounded and measurable, and every discontinuity point of $h$ is a discontinuity point of $f$. Thus

$$
\mathbb P(X\in D_h)\leq\mathbb P(X\in D_f)=0.
$$

The [Portmanteau theorem](../../../convergence-of-random-variables.md#portmanteau-theorem) includes the null-discontinuity criterion: if $X_n\xrightarrow dX$ and a bounded measurable function is continuous at $X$ almost surely, then its expectations converge. Hence

$$
\mathbb E[g(f(X_n))]\longrightarrow\mathbb E[g(f(X))].
$$

Since this holds for every bounded continuous $g$, it proves the [continuous mapping theorem](../../../convergence-of-random-variables.md#continuous-mapping-theorem) conclusion $f(X_n)\xrightarrow d f(X)$.

## 3

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Let $\tau=T_r\wedge T_R$. The function $z\mapsto\log|z|$ is a [harmonic function](../../../partial-differential-equation.md#harmonic-function) on the annulus $r<|z|<R$, so [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) shows that

$$
\log|B_{t\wedge\tau}|
$$

is a bounded [martingale](../../../martingale.md). By the [optional sampling theorem for a supermartingale](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) applied to this martingale,

$$
\log|x|
=\mathbb E_x[\log|B_\tau|]
=p\log r+(1-p)\log R,
$$

where $p=\mathbb P_x(T_r<T_R)$. Solving gives the [planar Brownian annulus hitting probability](../../../brownian-motion.md#planar-brownian-annulus-hitting-probability)

$$
\boxed{\mathbb P_x(T_r<T_R)
=\frac{\log R-\log|x|}{\log R-\log r}.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Each completed visit to radius $r_2$ begins a new radial excursion. By part (a), the conditional probability that the following excursion reaches radius $R$ before radius $r_1$ is

$$
q_R=\frac{\log(r_2/r_1)}{\log(R/r_1)}.
$$

The [Strong Markov property](../../../markov-process.md#strong-markov-property) at the successive stopping times $\tau_{2k}$ makes these trials independent with the same success probability. Consequently $N(R)$ has a [geometric distribution](../../../discrete-probability-distribution.md#geometric-distribution) on $\{1,2,\ldots\}$ with parameter $q_R$:

$$
\mathbb P(N(R)>k)=(1-q_R)^k.
$$

As $R\to\infty$, $q_R\to0$ and

$$
q_RN(R)\xrightarrow d\operatorname{Exp}(1),
\qquad
q_R\log R\longrightarrow\log(r_2/r_1).
$$

[Slutsky theorem](../../../statistical-inference.md#slutsky-theorem) now gives

$$
\boxed{\frac{N(R)}{\log R}
\xrightarrow d\operatorname{Exp}\!\left(\log(r_2/r_1)\right).}
$$

## 4

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The one-dimensional [Donsker invariance principle](../../../convergence-of-random-variables.md#donsker-s-theorem) says that if $X_1,X_2,\ldots$ are [IID random variables](../../../random-variable.md#independent-and-identically-distributed-random-variables) with mean zero and variance one, then the linearly interpolated process

$$
W_n(t)=\frac1{\sqrt n}\left(S_{\lfloor nt\rfloor}+(nt-\lfloor nt\rfloor)X_{\lfloor nt\rfloor+1}\right),
\qquad0\leq t\leq1,
$$

converges weakly in $C([0,1])$ with the uniform norm to standard [Brownian motion](../../../brownian-motion.md).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

The [strong law for Brownian motion](../../../brownian-motion.md#strong-law-for-brownian-motion) gives $B_t/t\to0$ almost surely. Therefore

$$
\frac{\widetilde B_t}{t}=\frac{B_t}{t}-\mu\longrightarrow-\mu<0
$$

almost surely, and hence $\widetilde B_t\to-\infty$ almost surely.

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

Let $\sigma_x=\inf\{t\geq0:\widetilde B_t=x\}$. Continuity gives $\{S\geq x\}=\{\sigma_x<\infty\}$. On this event, the [Strong Markov property](../../../markov-process.md#strong-markov-property) says that

$$
(\widetilde B_{\sigma_x+t}-x)_{t\geq0}
$$

is an independent Brownian motion with drift $-\mu$. It reaches level $y$ with probability $\mathbb P(S\geq y)$. Therefore

$$
\boxed{\mathbb P(S\geq x+y)
=\mathbb P(\sigma_x<\infty)\mathbb P(S\geq y)
=\mathbb P(S\geq x)\mathbb P(S\geq y).}
$$

<h4 id="4/b/iii">iii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/b/iii)

Under the [Cameron-Martin theorem for a linear drift](../../../brownian-motion.md#cameron-martin-theorem-for-a-linear-drift), the probability that Brownian motion with drift $-\mu$ reaches $x$ is

$$
\mathbb P(S\geq x)
=e^{-\mu x}\mathbb E\!\left[e^{-\mu^2T_x/2}\right].
$$

Using the supplied [Laplace transform](../../../analysis.md#laplace-transform) with $\lambda=\mu^2/2$ gives

$$
\mathbb E[e^{-\mu^2T_x/2}]=e^{-\mu x},
$$

and hence

$$
\mathbb P(S\geq x)=e^{-2\mu x}.
$$

This is the survival function of the [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) with rate $2\mu$.

## 5

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Planar [Brownian motion](../../../brownian-motion.md) and the initial law $\nu_{0,R}$ are invariant under every rotation about the origin. The hitting time $\tau_{0,r}$ is also rotation invariant, so the law of $B_{\tau_{0,r}}$ is invariant under every rotation of the circle of radius $r$. Planar Brownian motion hits that circle almost surely by [recurrence of planar Brownian motion](../../../brownian-motion.md#recurrence-of-planar-brownian-motion). The unique rotation-invariant probability measure on the circle is its uniform measure, and therefore

$$
\boxed{B_{\tau_{0,r}}\sim\nu_{0,r}.}
$$

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Reflection in $L$ interchanges $x$ and $y$. Relabel the two points if necessary so that $x$ lies on the side of $L$ containing the center $a$; the absolute difference is symmetric in $x$ and $y$. Couple a Brownian motion $B$ started at $x$ to one $B'$ started at $y$ by setting $B'_t=\phi(B_t)$ before $T_L$ and $B'_t=B_t$ afterwards. The [Brownian reflection coupling](../../../brownian-motion.md#brownian-reflection-coupling) has the correct marginal laws because reflection is an isometry and the [Strong Markov property](../../../markov-process.md#strong-markov-property) applies at $T_L$. Once the paths meet on $L$, they agree forever.

If the path from $x$ does not hit the target circle before $T_L$, the coupled paths meet before the relevant uncoupled hitting outcomes can differ. The [coupling inequality for total variation](../../../probability-and-statistics.md#coupling-inequality-for-total-variation) therefore gives

$$
\boxed{\left|\mathbb P_x(B_{\tau_{a,r_1}}\in A)
-\mathbb P_y(B_{\tau_{a,r_1}}\in A)\right|
\leq\mathbb P_x(\tau_{a,r_1}<T_L).}
$$

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Write

$$
H_A(z)=\mathbb P_z(B_{\tau_{a,r_1}}\in A).
$$

This is the [harmonic measure](../../../brownian-motion.md#harmonic-measure) of $A$ viewed from $z$, and is a bounded [harmonic function](../../../partial-differential-equation.md#harmonic-function) outside the closed target disc. The disc is contained in $B(0,r_2)$. In the half-plane cut out by a line $L$ through the origin, the probability of reaching $B(0,r_2)$ before $L$, from a point of modulus $R$, is $O(r_2/R)$ uniformly in the direction. One sees this by mapping the half-plane outside the disc with $z\mapsto\log(z/r_2)$ to a half-strip and solving the corresponding [Dirichlet problem](../../../analysis.md#dirichlet-problem) by a sine series.

Part (b) consequently shows that the angular oscillation of $H_A$ on a large circle tends to zero, uniformly in the Borel set $A$. The same half-strip estimate in the annulus $R-|a|\leq|z|\leq R+|a|$ shows that shifting the center of that circle by the fixed vector $a$ changes the average of $H_A$ by $o(1)$, uniformly in $A$. Hence, for every $\varepsilon>0$, all sufficiently large $R$ satisfy

$$
\left|\mathbb P_{\nu_{a,R}}(B_{\tau_{a,r_1}}\in A)
-\mathbb P_{\nu_{0,R}}(B_{\tau_{a,r_1}}\in A)\right|
\leq\varepsilon
$$

for every Borel subset $A$ of the target disc.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

By part (a), translated by $a$, starting with $B_0\sim\nu_{a,R}$ gives

$$
B_{\tau_{a,r_1}}\sim\nu_{a,r_1}.
$$

Part (c) says that the same hitting law from $\nu_{0,R}$ tends in [total variation distance](../../../probability-and-statistics.md#total-variation-distance) to $\nu_{a,r_1}$. On the other hand, every path from the circle of radius $R>r_2$ to the target disc must first hit the circle of radius $r_2$. Part (a) and the [Strong Markov property](../../../markov-process.md#strong-markov-property) show that its position there has law $\nu_{0,r_2}$ and that

$$
\mathbb P_{\nu_{0,R}}(B_{\tau_{a,r_1}}\in A)
=\mathbb P_{\nu_{0,r_2}}(B_{\tau_{a,r_1}}\in A),
$$

independently of $R$. Letting $R\to\infty$ in part (c) proves

$$
B_{\tau_{a,r_1}}\sim\nu_{a,r_1}
$$

when $B_0\sim\nu_{0,r_2}$.

## 6

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

The [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem) states that a discrete-time martingale $(X_n)$ with [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability) has an integrable random variable $X_\infty$ such that

$$
X_n\longrightarrow X_\infty
$$

almost surely and in $L^1$. Moreover, the martingale is closed by its limit:

$$
\boxed{X_n=\mathbb E[X_\infty\mid\mathcal F_n].}
$$

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

For bounded stopping times $S\wedge n\leq T\wedge n$, the [optional sampling theorem for a supermartingale](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) gives

$$
\mathbb E[X_{T\wedge n}]=\mathbb E[X_{S\wedge n}]=\mathbb E[X_0].
$$

A stopped family drawn from a uniformly integrable martingale is uniformly integrable. Since $X_{T\wedge n}\to X_T$ and $X_{S\wedge n}\to X_S$ almost surely, [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability) upgrades both convergences to $L^1$. Passing to the limit yields

$$
\boxed{\mathbb E[X_T]=\mathbb E[X_S].}
$$

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Put $\mathcal F_n=\sigma(X_0,\ldots,X_n)$ and $\tau=T_0\wedge T_y$. Before $\tau$, the integer-valued increment belongs to $\{-1,0,1\}$. The [martingale](../../../martingale.md) property gives

$$
\mathbb P(X_{n+1}-X_n=1\mid\mathcal F_n)
=\mathbb P(X_{n+1}-X_n=-1\mid\mathcal F_n).
$$

Their sum is at least $1/2$, so each conditional probability is at least $1/4$. From any state in $\{1,\ldots,y-1\}$, a run of at most $y$ upward moves reaches $y$ and has conditional probability at least $4^{-y}$. Applied in successive blocks of $y$ steps, this gives

$$
\mathbb P(\tau>ky)\leq(1-4^{-y})^k,
$$

so $\tau<\infty$ almost surely.

The stopped process $X_{n\wedge\tau}$ takes values in $[0,y]$, hence is a bounded martingale and has [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability). The [optional sampling theorem for a supermartingale](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) gives

$$
x=\mathbb E[X_\tau]
=y\mathbb P(T_y<T_0),
$$

because $X_\tau$ is zero or $y$. Therefore

$$
\boxed{\mathbb P(T_y<T_0)=\frac{x}{y}.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
