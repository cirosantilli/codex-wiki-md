# Paper 201

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_201.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_201.pdf)

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
  - [d](#2/d)
    - [Solution](#2/d/solution)
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
  - [d](#6/d)
    - [Solution](#6/d/solution)

## 1

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Put $q=1-p$. Since

$$
\mathbb E\!\left[\lambda^{S_{n+1}}\mid\mathcal F_n\right]
=\lambda^{S_n}\left(p\lambda+q\lambda^{-1}\right),
$$

the [martingale](../../../martingale.md) condition is

$$
p\lambda^2-\lambda+q=0
=(\lambda-1)(p\lambda-q).
$$

The root in $(0,1)$ is therefore

$$
\boxed{\lambda=\frac{1-p}{p}.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $\tau=T_a\wedge T_b$. The walk exits the finite interval $[a,b]$ almost surely, and the stopped martingale $\phi(S_{n\wedge\tau})$ is bounded between $\lambda^b$ and $\lambda^a$. The [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) and [bounded convergence theorem](../../../measure-theory.md#bounded-convergence-theorem) give

$$
1=\phi(0)=\mathbb E[\phi(S_\tau)]
=\lambda^a\mathbb P(T_a<T_b)
+\lambda^b\mathbb P(T_b<T_a).
$$

Solving for the first probability gives the [biased gambler's ruin probability](../../../markov-process.md#biased-gambler-s-ruin-probability)

$$
\boxed{\mathbb P(T_a<T_b)
=\frac{\lambda^b-1}{\lambda^b-\lambda^a}
=\frac{\phi(b)-\phi(0)}{\phi(b)-\phi(a)}.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

As $b\to\infty$, the events $\{T_a<T_b\}$ increase to $\{T_a<\infty\}$: every path that reaches $a$ has a finite maximum before doing so. Since $\lambda^b\to0$,

$$
\boxed{\mathbb P(T_a<\infty)=\lambda^{-a}.}
$$

Similarly, as $a\to-\infty$, the events $\{T_b<T_a\}$ increase to $\{T_b<\infty\}$, and

$$
\mathbb P(T_b<T_a)
=\frac{1-\lambda^a}{\lambda^b-\lambda^a}
\longrightarrow1.
$$

Hence

$$
\boxed{\mathbb P(T_b<\infty)=1.}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The [strong law of large numbers](../../../convergence-of-random-variables.md#strong-law-of-large-numbers) gives

$$
\frac{S_n}{n}\longrightarrow\mathbb E[X_1]=2p-1>0
\qquad\text{almost surely}.
$$

Because $0<\lambda<1$, it follows that $\lambda^{S_n}\to0$ almost surely. If this martingale were [uniformly integrable](../../../convergence-of-random-variables.md#uniform-integrability), almost-sure convergence would imply convergence in $L^1$, and therefore

$$
\mathbb E[\lambda^{S_n}]\longrightarrow0.
$$

But the martingale has constant expectation $\mathbb E[\lambda^{S_n}]=1$. This contradiction proves that

$$
\boxed{(\phi(S_n))_{n\geq0}\text{ is not uniformly integrable}.}
$$

## 2

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Write $v_m=\operatorname{Var}(X_m)=\sigma_m^2$. Independence and $\mathbb E[X_{n+1}]=0$ give

$$
\begin{aligned}
\mathbb E[(S_{n+1}+c)^2\mid\mathcal F_n]
&=(S_n+c)^2
+2(S_n+c)\mathbb E[X_{n+1}]
+\mathbb E[X_{n+1}^2]\\
&=(S_n+c)^2+v_{n+1}\\
&\geq(S_n+c)^2.
\end{aligned}
$$

Thus

$$
\boxed{((S_n+c)^2)_{n\geq0}\text{ is a submartingale}.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Put $V=\operatorname{Var}(S_n)=\sum_{m=1}^nv_m$. If $\max_{m\leq n}S_m\geq x$, then

$$
\max_{m\leq n}(S_m+c)^2\geq(x+c)^2.
$$

The [Doob maximal inequality for a nonnegative submartingale](../../../martingale.md#doob-maximal-inequality-for-a-nonnegative-submartingale) therefore gives

$$
\mathbb P\left(\max_{m\leq n}S_m\geq x\right)
\leq\frac{\mathbb E[(S_n+c)^2]}{(x+c)^2}
=\frac{V+c^2}{(x+c)^2}.
$$

The right side is minimized at $c=V/x$, and substitution gives

$$
\boxed{\mathbb P\left(\max_{1\leq m\leq n}S_m\geq x\right)
\leq\frac{\operatorname{Var}(S_n)}
{\operatorname{Var}(S_n)+x^2}.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $V_n=\operatorname{Var}(S_n)=\sum_{m=1}^nv_m$. Then

$$
\begin{aligned}
\mathbb E[S_{n+1}^2-V_{n+1}\mid\mathcal F_n]
&=S_n^2+v_{n+1}-V_n-v_{n+1}\\
&=S_n^2-V_n.
\end{aligned}
$$

Consequently

$$
\boxed{(S_n^2-\operatorname{Var}(S_n))_{n\geq0}
\text{ is a martingale}.}
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Let

$$
\tau=\min\bigl(\{m\leq n:|S_m|>x\}\cup\{n\}\bigr).
$$

Because $|X_m|\leq K$, one always has $|S_\tau|\leq x+K$: this is clear if no crossing occurs, and at the first crossing the overshoot is at most one increment. Apply the [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) to the martingale from part (c):

$$
\mathbb E[S_\tau^2]=\mathbb E[V_\tau]\leq(x+K)^2.
$$

On the event $\{\max_{m\leq n}|S_m|\leq x\}$ one has $\tau=n$, so $V_\tau=V_n$. Since $V_\tau\geq0$ everywhere,

$$
V_n\mathbb P\left(\max_{m\leq n}|S_m|\leq x\right)
\leq\mathbb E[V_\tau]
\leq(x+K)^2.
$$

Hence

$$
\boxed{\mathbb P\left(\max_{1\leq m\leq n}|S_m|\leq x\right)
\leq\frac{(x+K)^2}{\operatorname{Var}(S_n)}.}
$$

## 3

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Since $X_1$ is uniform on $\{-1,1\}$,

$$
\psi(\lambda)
=\log\mathbb E[e^{\lambda X_1}]
=\log\left(\frac{e^\lambda+e^{-\lambda}}2\right)
=\log\cosh\lambda.
$$

For $|x|<1$, the supremum in the [Legendre transform of a cumulant-generating function](../../../probability-theory.md#legendre-transform-of-a-cumulant-generating-function) is attained where

$$
x=\psi'(\lambda)=\tanh\lambda,
\qquad
\lambda=\frac12\log\frac{1+x}{1-x}.
$$

Substitution gives the [Rademacher large-deviation rate function](../../../probability-theory.md#rademacher-large-deviation-rate-function)

$$
\boxed{\psi^*(x)
=\frac{(1+x)\log(1+x)+(1-x)\log(1-x)}2}
$$

for $|x|\leq1$, with $0\log0=0$; it is $+\infty$ for $|x|>1$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

By the definition of [exponential tilting](../../../probability-theory.md#exponential-tilting),

$$
\mathbb P(A_n)
=\mathbb E_\lambda\!\left[
e^{-\lambda S_n+n\psi(\lambda)}\mathbf1_{A_n}
\right].
$$

On $A_n$ one has $S_n\leq cn$, so for $\lambda\geq0$,

$$
e^{-\lambda S_n+n\psi(\lambda)}
\geq e^{-\lambda cn+n\psi(\lambda)}.
$$

Therefore

$$
\boxed{\mathbb P(A_n)
\geq e^{-\lambda cn+n\psi(\lambda)}
\mathbb P_\lambda(A_n).}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Fix $a<b<c<1$ and choose

$$
\lambda=\operatorname{arctanh}b.
$$

Under $\mathbb P_\lambda$, the increments remain independent and identically distributed, with mean $\psi'(\lambda)=b$. The [strong law of large numbers](../../../convergence-of-random-variables.md#strong-law-of-large-numbers) therefore gives

$$
\mathbb P_\lambda(an\leq S_n\leq cn)\longrightarrow1.
$$

Part (b) implies

$$
\liminf_{n\to\infty}\frac1n\log\mathbb P(S_n\geq an)
\geq-\lambda c+\psi(\lambda).
$$

Let $c\downarrow b$ and then $b\downarrow a$. Since $\lambda b-\psi(\lambda)=\psi^*(b)$ and $\psi^*$ is continuous on $[0,1)$,

$$
\boxed{\liminf_{n\to\infty}\frac1n
\log\mathbb P(S_n\geq an)\geq-\psi^*(a).}
$$

The same argument includes $a=0$ by taking $b\downarrow0$.

## 4

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

An $\mathbb R^d$-valued process $(X_t)_{t\geq0}$ is a [Brownian motion](../../../brownian-motion.md) started at $x$ when:

- $X_0=x$ almost surely;
- its sample paths are almost surely continuous;
- increments over disjoint time intervals are independent; and
- for $0\leq s<t$, $X_t-X_s$ has the centered [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution) with covariance matrix $(t-s)I_d$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The paths of $UX_t$ are continuous, and linear transformation preserves independence of increments. Moreover,

$$
U(X_t-X_s)\sim N\!\left(0,(t-s)UI_dU^T\right)
=N(0,(t-s)I_d)
$$

because $U$ is an [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix). Thus all defining properties are preserved, proving the [orthogonal invariance of Brownian motion](../../../brownian-motion.md#orthogonal-invariance-of-brownian-motion):

$$
\boxed{(UX_t)_{t\geq0}\text{ is Brownian motion in }\mathbb R^d.}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Fix a closed ball $\overline B(x,r)\subset D$ and let $\tau$ be its first exit time. By the [Strong Markov property](../../../markov-process.md#strong-markov-property), conditioning at $\tau$ gives

$$
\phi(x)=\mathbb E_x[\phi(X_\tau)].
$$

The [orthogonal invariance of Brownian motion](../../../brownian-motion.md#orthogonal-invariance-of-brownian-motion) implies that $X_\tau$ is uniformly distributed on the sphere $\partial B(x,r)$. Hence

$$
\phi(x)=\frac1{|\partial B(x,r)|}
\int_{\partial B(x,r)}\phi(y)\,dS(y).
$$

Thus $\phi$ has the [mean value property](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions) on every ball compactly contained in $D$. Since $0\leq\phi\leq1$, the mean-value characterization of [harmonic functions](../../../partial-differential-equation.md#harmonic-function) yields

$$
\boxed{\Delta\phi=0\quad\text{in }D.}
$$

This function is the [harmonic measure](../../../brownian-motion.md#harmonic-measure) of $A$ viewed from $x$.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The required boundary values on the real axis are zero to the left of the origin and one to the right. The bounded harmonic function with those values is the [upper-half-plane harmonic measure of the positive half-axis](../../../brownian-motion.md#upper-half-plane-harmonic-measure-of-the-positive-half-axis),

$$
\boxed{\phi(x,y)
=\frac12+\frac1\pi\arctan\frac{x}{y}
=1-\frac1\pi\arg(x+iy),\qquad y>0.}
$$

Indeed, $\arg z$ is harmonic in the upper half-plane, and the displayed function tends to $1$ on the positive half-axis and to $0$ on the negative half-axis. The uniqueness of bounded solutions of the [Dirichlet problem](../../../analysis.md#dirichlet-problem) identifies it with the Brownian exit probability.

## 5

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Planar Brownian motion is recurrent. More explicitly, the [planar Brownian annulus hitting probability](../../../brownian-motion.md#planar-brownian-annulus-hitting-probability) gives

$$
\mathbb P_x(T_1<T_R)
=\frac{\log R-\log|x|}{\log R}
\longrightarrow1
\qquad(R\to\infty)
$$

when $|x|>1$. Thus the unit disc is hit almost surely from every starting point. Applying the [Strong Markov property](../../../markov-process.md#strong-markov-property) after each departure and return shows that such returns occur after arbitrarily large times. Therefore

$$
\boxed{\{t\geq0:|X_t|\leq1\}\text{ is almost surely unbounded}.}
$$

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

By the [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) and the planar [Brownian transition density](../../../brownian-motion.md#brownian-transition-density),

$$
\mathbb E[A_t]
=\int_0^t\mathbb E[f(X_s)]\,ds.
$$

For $s\geq1$,

$$
\mathbb E[f(X_s)]
=\int_{\mathbb R^2}f(y)\frac1{2\pi s}
e^{-|y-X_0|^2/(2s)}\,dy
\leq\frac1{2\pi s},
$$

while for $0\leq s\leq1$ it is at most $\|f\|_\infty$. Hence

$$
\mathbb E[A_t]\leq\|f\|_\infty+\frac{\log t}{2\pi}
$$

for $t\geq1$, and consequently

$$
\boxed{\mathbb E[A_t/t]\longrightarrow0.}
$$

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Because $f$ is a continuous probability density, there are a point $z$, a radius $r>0$, and $\epsilon>0$ such that

$$
f\geq\epsilon\quad\text{on }B(z,r).
$$

By the [recurrence of planar Brownian motion](../../../brownian-motion.md#recurrence-of-planar-brownian-motion), the smaller disc $B(z,r/2)$ is visited at arbitrarily large times. Starting anywhere in that smaller disc, Brownian continuity and compactness give a uniform probability $\delta>0$ of staying in $B(z,r)$ for a fixed time $u>0$.

Apply the [Strong Markov property](../../../markov-process.md#strong-markov-property) at successive visits separated by at least $u$. The conditional probability of each stay event is at least $\delta$, so the conditional [Borel-Cantelli lemma](../../../probability-theory.md#borel-cantelli-lemmas) gives infinitely many successful stays almost surely. Every success adds at least $\epsilon u$ to $A_t$. Since $A_t$ is nondecreasing,

$$
\boxed{A_t\longrightarrow\infty\quad\text{almost surely}.}
$$

## 6

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

The count $N_t=M(0,t]$ is a rate-$\lambda$ [Poisson process](../../../probability-theory.md#poisson-process). Over a time interval $(s,t]$, the increment

$$
X_t-X_s=\sum_{n=N_s+1}^{N_t}g(Y_n)
$$

depends only on the Poisson points and marks in that interval. Disjoint intervals give independent increments, and the distribution depends only on $t-s$. The paths are càdlàg step functions, $X_0=0$, and

$$
\mathbb P(X_{t+h}\ne X_t)\leq\mathbb P(N_{t+h}-N_t\geq1)
=1-e^{-\lambda h}\longrightarrow0.
$$

Thus $X$ is stochastically continuous and

$$
\boxed{(X_t)_{t\geq0}\text{ is a compound Poisson process, hence a Lévy process}.}
$$

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

For $g\geq0$, the [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) and conditioning on $N_t$ give

$$
\mathbb E[X_t\mid N_t]
=N_t\mathbb E[g(Y_1)]
=N_t\int_0^1g(y)\,dy.
$$

Since $\mathbb E[N_t]=\lambda t$,

$$
\boxed{\mathbb E[X_t]
=\lambda t\int_0^1g(y)\,dy,}
$$

with both sides allowed to be $+\infty$.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

A martingale must be integrable. On the event $\{N_t=1\}$, $X_t=g(Y_1)$, so integrability of $X_t$ forces

$$
\int_0^1|g(y)|\,dy<\infty.
$$

For $s<t$, independent increments give

$$
\mathbb E[X_t-X_s\mid\mathcal F_s]
=\lambda(t-s)\int_0^1g(y)\,dy.
$$

Therefore the necessary and sufficient condition is

$$
\boxed{g\in L^1[0,1]
\quad\text{and}\quad
\int_0^1g(y)\,dy=0.}
$$

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

The joint process is a two-dimensional [Compound Poisson process](../../../stochastic-process.md#compound-poisson-process) whose [Lévy measure](../../../stochastic-process.md#levy-measure) is

$$
\nu(B)=\lambda\,\operatorname{Leb}
\{y\in[0,1]:(g_1(y),g_2(y))\in B\}.
$$

Two coordinates of a Lévy process are independent exactly when its Lévy measure charges only the coordinate axes and its Gaussian covariance has no cross term. Here there is no Gaussian part, so independence is equivalent to

$$
g_1(y)g_2(y)=0
\quad\text{for almost every }y.
$$

Since $g_1g_2$ is continuous, this is equivalent to pointwise vanishing. Conversely, when the product vanishes, the mark sets where $g_1$ and $g_2$ are nonzero are disjoint; independent thinning of the [Poisson random measure](../../../probability-theory.md#poisson-random-measure) gives independent coordinate processes. Hence

$$
\boxed{(X_t^{g_1})_{t\geq0}\text{ and }(X_t^{g_2})_{t\geq0}
\text{ are independent}
\iff g_1(y)g_2(y)=0\ \text{for every }y\in[0,1].}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
