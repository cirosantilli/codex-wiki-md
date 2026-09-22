# Paper 201

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_201.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_201.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
    - [iii](#1/c/iii)
      - [Solution](#1/c/iii/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
    - [iii](#2/a/iii)
      - [Solution](#2/a/iii/solution)
    - [iv](#2/a/iv)
      - [Solution](#2/a/iv/solution)
    - [v](#2/a/v)
      - [Solution](#2/a/v/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
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
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
    - [iii](#4/a/iii)
      - [Solution](#4/a/iii/solution)
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
  - [d](#5/d)
    - [Solution](#5/d/solution)
  - [e](#5/e)
    - [Solution](#5/e/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [i](#6/c/i)
      - [Solution](#6/c/i/solution)
    - [ii](#6/c/ii)
      - [Solution](#6/c/ii/solution)
  - [d](#6/d)
    - [i](#6/d/i)
      - [Solution](#6/d/i/solution)
    - [ii](#6/d/ii)
      - [Solution](#6/d/ii/solution)

## 1

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A standard [Brownian motion](../../../brownian-motion.md) is a real-valued process $(B_t)_{t\geq0}$ with $B_0=0$, almost surely continuous paths, and independent increments satisfying $B_t-B_s\sim N(0,t-s)$ for $s<t$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

For a partition of $[a,b]$, every [Riemann sum](../../../real-analysis.md#riemann-sum) $S_n=\sum_jB_{t_j}\Delta t_j$ is a centered [Gaussian random variable](../../../probability-theory.md#normal-distribution), with

$$
\operatorname{Var}S_n=\sum_{i,j}\min(t_i,t_j)\Delta t_i\Delta t_j.
$$

Path continuity gives $S_n\to\int_a^bB_sds$ almost surely, and the covariance bound $\mathbb E|B_s-B_t|^2=|s-t|$ also gives convergence in $L^2$. Hence the limit is Gaussian, centered, and passage to the limit in the displayed sums gives variance

$$
\boxed{\int_a^b\int_a^b\min(s,t)\,ds\,dt.}
$$

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Choose step functions $f_n\to f$ in $L^2[0,1]$. Part (i) shows that $\int B_sf_n(s)ds$ is centered Gaussian. Since the kernel $K(r,s)=\min(r,s)$ is bounded,

$$
\mathbb E\left|\int_0^1B_s(f_n-f)(s)ds\right|^2
=\iint(f_n-f)(r)(f_n-f)(s)K(r,s)drds\to0.
$$

The $L^2$ limit is therefore centered Gaussian, and its variance is

$$
\boxed{\int_0^1\int_0^1f(r)f(s)\min(r,s)\,dr\,ds.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

Writing $c_i(t)=\langle\mathbf1_{[0,t]},f_i\rangle_{L^2}$ gives $X_n(t)=\sum_{i=1}^n\alpha_ic_i(t)$, hence

$$
X_n(t)\sim N\left(0,\sum_{i=1}^nc_i(t)^2\right).
$$

By [Parseval identity](../../../fourier-analysis.md#parseval-identity), the variance tends to $\lVert\mathbf1_{[0,t]}\rVert_2^2=t$. Thus $X_n(t)\xrightarrow dN(0,t)$.

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

For fixed $t$, $(X_n(t))$ is a martingale with independent centered increments and

$$
\sup_n\mathbb E X_n(t)^2=\sum_{i\geq1}c_i(t)^2=t.
$$

The $L^2$ [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem) gives convergence both almost surely and in $L^2$ to a random variable $X(t)$.

<h4 id="1/c/iii">iii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/c/iii)

For real $u_1,\ldots,u_j$, the preceding series construction gives

$$
\sum_ru_rX(t_r)
=\sum_{i\geq1}\alpha_i\left\langle\sum_ru_r\mathbf1_{[0,t_r]},f_i\right\rangle.
$$

It is centered Gaussian, and [Parseval identity](../../../fourier-analysis.md#parseval-identity) makes its variance

$$
\left\lVert\sum_ru_r\mathbf1_{[0,t_r]}\right\rVert_2^2
=\sum_{r,s}u_ru_s\min(t_r,t_s).
$$

This is the variance of $\sum_ru_rB_{t_r}$. The [Cramér–Wold theorem](../../../convergence-of-random-variables.md#cramer-wold-theorem) proves equality of the two joint distributions.

## 2

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

The [Strong Markov property](../../../markov-process.md#strong-markov-property) says that for every almost surely finite stopping time $T$, the process $(B_{T+t}-B_T)_{t\geq0}$ is a standard Brownian motion independent of $\mathcal F_T$.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

The process $Y_t=B_{T-t}-B_T$ is centered Gaussian and continuous. Its covariance is

$$
\mathbb E[Y_sY_t]=\min(s,t),
$$

as follows by expanding Brownian covariances, or by reading its increments backwards. The [Gaussian-process characterization of Brownian motion](../../../brownian-motion.md#gaussian-process-characterization-of-brownian-motion) therefore shows that $(Y_t)_{0\leq t\leq T}$ has the same law as $(B_t)_{0\leq t\leq T}$.

<h4 id="2/a/iii">iii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/a/iii)

The event $\{B_T=I_T\}$ is the event that $B_{T-t}-B_T\geq0$ for every $t\leq T$. By part (ii), its probability equals the probability that Brownian motion started at zero remains nonnegative throughout $(0,T]$. The [Brownian reflection principle](../../../brownian-motion.md#reflection-principle-wiener-process) implies $\mathbb P(\min_{s\leq T}B_s\geq0)=0$. Hence $\mathbb P(B_T=I_T)=0$.

<h4 id="2/a/iv">iv</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/a/iv)

Continuity gives existence of a minimizer. If there were two, choose a rational $q$ strictly between them. Then the minima on $[0,q]$ and $[q,1]$ would coincide. Conditional on $\mathcal F_q$, the latter equals $B_q$ plus the minimum of an independent Brownian motion on $[0,1-q]$, whose distribution is continuous by the [Brownian reflection principle](../../../brownian-motion.md#reflection-principle-wiener-process). Thus equality has conditional probability zero. Taking the countable union over rational $q$ proves almost-sure uniqueness.

<h4 id="2/a/v">v</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/v/solution">Solution</h5>

↑ **Parent:** [V](#2/a/v)

Almost surely, Brownian motion has a unique minimizer on every interval with rational endpoints, by rescaling part (iv). Every local minimum is the minimum on some rational interval contained in a witnessing neighbourhood. Each rational interval contributes at most one point, and there are countably many such intervals. The set of local minima is therefore countable.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

The function $z\mapsto\log|z|$ is [harmonic](../../../partial-differential-equation.md#harmonic-function) on the annulus $\varepsilon<|z|<R$. Hence $\log|B_{t\wedge\tau_\varepsilon\wedge\tau_R}|$ is a bounded martingale by [Itô formula](../../../stochastic-calculus.md#ito-s-lemma). Optional stopping gives

$$
\log|x|=p\log\varepsilon+(1-p)\log R,
\qquad p=\mathbb P_x(\tau_\varepsilon<\tau_R).
$$

Solving yields

$$
\boxed{p=\frac{\log R-\log|x|}{\log R-\log\varepsilon}.}
$$

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

For fixed $y\ne x$, part (i), translated by $y$, and then $\varepsilon\downarrow0$ show that planar Brownian motion has probability zero of ever hitting $y$ before leaving any fixed large disk. Letting the disk radius tend to infinity shows $\mathbb P_x(y\in B([0,1]))=0$. By [Tonelli theorem](../../../measure-theory.md#tonelli-theorem),

$$
\mathbb E\lambda_2(B([0,1]))
=\int_{\mathbb R^2}\mathbb P_x(y\in B([0,1]))dy=0.
$$

The nonnegative random area is therefore zero almost surely.

## 3

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [conditional expectation](../../../measure-theory.md#conditional-expectation) $\mathbb E[X\mid\mathcal G]$ is the almost surely unique integrable, $\mathcal G$-measurable random variable $Z$ such that $\int_AZ\,d\mathbb P=\int_AX\,d\mathbb P$ for every $A\in\mathcal G$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Conditional expectation is the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) from $L^2(\mathcal F)$ onto $L^2(\mathcal G)$. The difference $X-\mathbb E[X\mid\mathcal G]$ is orthogonal to every $\mathcal G$-measurable square-integrable variable, including $\mathbb E[X\mid\mathcal G]-\mathbb E[X\mid\mathcal H]$. The [Pythagorean theorem in an inner-product space](../../../linear-algebra.md#pythagorean-theorem-in-an-inner-product-space) applied to

$$
X-\mathbb E[X\mid\mathcal H]
=(X-\mathbb E[X\mid\mathcal G])
+(\mathbb E[X\mid\mathcal G]-\mathbb E[X\mid\mathcal H])
$$

gives the identity.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Put $M=\mathbb E[Y\mid\mathcal G]$. Expanding and using $\mathbb E[YM]=\mathbb E[M^2]$ gives

$$
\mathbb E[(Y-M)^2]=\mathbb E[Y^2]-\mathbb E[M^2].
$$

If $M\stackrel d=Y$, the right side is zero. Therefore $Y=M$ almost surely.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The conditional [Jensen inequality](../../../real-analysis.md#jensen-s-inequality) states that for an integrable $X$ and convex $\phi$, whenever the terms are integrable,

$$
\phi(\mathbb E[X\mid\mathcal G])
\leq\mathbb E[\phi(X)\mid\mathcal G]
\quad\text{almost surely}.
$$

For differentiable $\phi$, the supporting-line inequality $\phi(x)\geq\phi(m)+\phi'(m)(x-m)$ with $m=\mathbb E[X\mid\mathcal G]$ gives the result after conditional expectation. Approximation by supporting affine functions proves the general convex case.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Let $M=\mathbb E[Y\mid\mathcal G]$ and choose the stated strictly convex differentiable $\phi$ with $|\phi(x)|\leq|x|$. Conditional [Jensen inequality](../../../real-analysis.md#jensen-s-inequality) gives $\phi(M)\leq\mathbb E[\phi(Y)\mid\mathcal G]$. Since $M\stackrel d=Y$, both sides have the same expectation, so equality holds almost surely. Strictness of the supporting-line inequality on $\{Y\ne M\}$ then forces $Y=M$ almost surely.

## 4

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

The almost-sure [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem) states that a supermartingale $(X_n)$ satisfying $\sup_n\mathbb E[X_n^-]<\infty$ converges almost surely to a finite random variable.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

For a nonnegative [supermartingale](../../../martingale.md#supermartingale), $X_n^-=0$, so the hypothesis of part (i) holds. Its almost-sure limit is finite.

<h4 id="4/a/iii">iii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/a/iii)

Let independent increments $D_n$ equal $-1$ with probability $1-2^{-n}$ and $2^n-1$ with probability $2^{-n}$. Then $\mathbb ED_n=0$, so $X_n=\sum_{j=1}^nD_j$ is a martingale. Since $\sum_n2^{-n}<\infty$, the [Borel-Cantelli lemmas](../../../probability-theory.md#borel-cantelli-lemmas) say that only finitely many positive jumps occur almost surely. Thereafter every increment is $-1$, and hence $X_n\to-\infty$ almost surely.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For each integer $m$, stop on first crossing below $-m$. Bounded increments ensure the stopped martingale is bounded below by $-m-C$; after adding $m+C$ it is a nonnegative supermartingale and therefore converges. Thus on the event that $(X_n)$ is bounded below, it converges finitely. Applying the same argument to $-X_n$ shows that boundedness above also forces convergence. Outside the finite-limit event the path is therefore unbounded in both directions, so its limsup is $+\infty$ and its liminf is $-\infty$. Hence $\mathbb P(A\cup B)=1$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Let $Z$ be a fair Bernoulli variable measurable at time zero and let $(S_n)$ be an independent simple symmetric random walk. Then $X_n=ZS_n$ is a martingale with increments bounded by one. On $\{Z=0\}$ it converges to zero, while on $\{Z=1\}$ the recurrence of the [simple symmetric random walk](../../../probability-theory.md#simple-symmetric-random-walk) gives limsup $+\infty$ and liminf $-\infty$. Thus $\mathbb P(A)=\mathbb P(B)=1/2$.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Set $p_n=\mathbb P(B_n\mid\mathcal F_{n-1})$, $S_n=\sum_{j\leq n}\mathbf1_{B_j}$, and $A_n=\sum_{j\leq n}p_j$. Then $M_n=S_n-A_n$ is a martingale with bounded increments and conditional variance at most $p_n$. On $\{A_\infty<\infty\}$, localization and the $L^2$ martingale convergence theorem make $M_n$ converge, so the integer-valued increasing sequence $S_n$ is finite. On $\{A_\infty=\infty\}$, applying martingale convergence to

$$
\sum_n\frac{\mathbf1_{B_n}-p_n}{1+A_n}
$$

and [Kronecker lemma](../../../real-analysis.md#kronecker-lemma) gives $M_n/A_n\to0$. Hence $S_n/A_n\to1$ and $S_n\to\infty$. This is the [Conditional Borel-Cantelli lemma](../../../probability-theory.md#conditional-borel-cantelli-lemma), and proves the two events equal almost surely.

## 5

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The sequence $X_n$ [converges in distribution](../../../convergence-of-random-variables.md#convergence-in-distribution) to $X$ when $\mathbb E f(X_n)\to\mathbb E f(X)$ for every bounded continuous function $f$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Independence makes the joint law of $(X_n,Y_n)$ the product of its marginal laws. Weak convergence of both marginals implies convergence of these product measures to the product law of independent copies $(X,Y)$. The addition map is continuous, so the [continuous mapping theorem](../../../convergence-of-random-variables.md#continuous-mapping-theorem) gives $X_n+Y_n\xrightarrow dX+Y$.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Differentiability gives $\varphi(u)=1+iau+o(u)$ at zero. By the [characteristic function of a sum of independent variables](../../../probability-theory.md#characteristic-function-of-a-sum-of-independent-variables),

$$
\mathbb E e^{itS_n/n}=\varphi(t/n)^n\longrightarrow e^{iat},
$$

the characteristic function of the constant $a$. The [Lévy continuity theorem](../../../probability-theory.md#levy-continuity-theorem) yields $S_n/n\xrightarrow d a$, and convergence in distribution to a constant is equivalent to [convergence in probability](../../../convergence-of-random-variables.md#convergence-in-probability).

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

A family $(\mu_n)$ of probability measures on a metric space is tight when for every $\eta>0$ there is a compact set $K$ such that $\sup_n\mu_n(K^c)<\eta$.

<h3 id="5/e">e</h3>

↑ **Parent:** [5](#5)

<h4 id="5/e/solution">Solution</h4>

↑ **Parent:** [E](#5/e)

Choose $0<\alpha<\varepsilon/p$. At dyadic level $m$, [Markov inequality](../../../probability-inequality.md#markov-inequality) and a union bound give

$$
\mathbb P\left(\max_k|X^n_{(k+1)2^{-m}}-X^n_{k2^{-m}}|>C2^{-m\alpha}\right)
\leq cC^{-p}2^{-m(\varepsilon-\alpha p)},
$$

uniformly in $n$. Summing over $m$ shows that, outside a set of probability at most $C_0C^{-p}$, all dyadic increments obey this bound. Chaining dyadic approximations and using continuity gives

$$
|X_t^n-X_s^n|\leq C_1C|t-s|^\alpha
$$

for all $s,t$. Since $X_0^n=0$, the paths then lie in the stated compact Hölder set by the [Arzelà-Ascoli theorem](../../../topological-analysis.md#arzela-ascoli-theorem). Taking $C$ large proves tightness.

## 6

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Every evaluation map $\pi_t$ is continuous in the uniform metric, so $\mathcal F\subseteq\mathcal B$. Conversely, for $g\in C[0,1]$,

$$
\{f:\lVert f-g\rVert_\infty<r\}
=\bigcup_{m\geq1}\bigcap_{q\in\mathbb Q\cap[0,1]}
\{f:|f(q)-g(q)|\leq r-1/m\},
$$

with the harmless restriction to $m$ for which $r-1/m>0$. Thus every open ball belongs to $\mathcal F$. Separability makes every open set a countable union of balls, so $\mathcal B\subseteq\mathcal F$ and equality follows.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Let $d(x,A)$ be the distance to the closed set $A$. Continuity gives

$$
\{T_A\leq t\}
=\left\{\inf_{s\in[0,t]}d(X_s,A)=0\right\}
=\left\{\inf_{q\in\mathbb Q\cap[0,t]}d(X_q,A)=0\right\}.
$$

Every variable in the countable infimum is $\mathcal F_t$-measurable by adaptedness, so the event belongs to $\mathcal F_t$. Hence $T_A$ is a [stopping time](../../../martingale.md#stopping-time).

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/i">i</h4>

↑ **Parent:** [C](#6/c)

<h5 id="6/c/i/solution">Solution</h5>

↑ **Parent:** [I](#6/c/i)

Almost-sure convergence plus [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability) gives $X_n\to X$ in $L^1$. Conditional expectation is an $L^1$ contraction, so

$$
\boxed{\mathbb E|\mathbb E[X_n\mid\mathcal G]-\mathbb E[X\mid\mathcal G]|
\leq\mathbb E|X_n-X|\to0.}
$$

<h4 id="6/c/ii">ii</h4>

↑ **Parent:** [C](#6/c)

<h5 id="6/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/c/ii)

Take $X_n=Y_nZ_n$ and $\mathcal G=\sigma(Y_1,Y_2,\ldots)$. Then $\mathbb P(X_n=n)=n^{-2}$, so $(X_n)$ is uniformly integrable and $X_n\to0$ almost surely by the [Borel-Cantelli lemmas](../../../probability-theory.md#borel-cantelli-lemmas). Independence and $\mathbb EZ_n=1$ give

$$
\mathbb E[X_n\mid\mathcal G]=Y_n.
$$

But the independent events $\{Y_n=1\}$ have divergent probability sum, so the second Borel-Cantelli lemma makes them occur infinitely often. Thus these conditional expectations do not converge almost surely to zero.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/i">i</h4>

↑ **Parent:** [D](#6/d)

<h5 id="6/d/i/solution">Solution</h5>

↑ **Parent:** [I](#6/d/i)

The [Skorokhod embedding theorem](../../../martingale.md#skorokhod-embedding-theorem) states that if $\mu$ is a centered probability law on $\mathbb R$ with finite second moment, there is a Brownian stopping time $T$ such that $B_T\sim\mu$, the stopped process $(B_{t\wedge T})$ is uniformly integrable, and $\mathbb ET=\int x^2\mu(dx)$.

<h4 id="6/d/ii">ii</h4>

↑ **Parent:** [D](#6/d)

<h5 id="6/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/d/ii)

Construct the times inductively. Suppose $(B_{T_0},\ldots,B_{T_n})$ has the law of $(S_0,\ldots,S_n)$. Conditional on the past, the martingale increment $S_{n+1}-S_n$ has mean zero and finite second moment. Apply the conditional form of the [Skorokhod embedding theorem](../../../martingale.md#skorokhod-embedding-theorem) to this regular conditional law, using the fresh Brownian motion $B_{T_n+t}-B_{T_n}$ supplied by the [Strong Markov property](../../../markov-process.md#strong-markov-property). This gives a stopping time increment $\tau_{n+1}$ and $T_{n+1}=T_n+\tau_{n+1}$ such that the next Brownian increment has the required conditional law. Induction proves

$$
(S_0,\ldots,S_k)\stackrel d=(B_{T_0},\ldots,B_{T_k})
$$

for every $k$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
