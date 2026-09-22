# Paper 226

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20226.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20226.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
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
  - [d](#3/d)
    - [Solution](#3/d/solution)

## 1

↑ **Parent:** [Paper 226](paper-226.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For [simple random walk](../../../markov-process.md#simple-random-walk) on $\mathbb Z^d$, $d\geq3$, the [Green-function decay for simple random walk on the integer lattice](../../../markov-process.md#green-function-decay-for-simple-random-walk-on-the-integer-lattice) and the [Strong Markov property](../../../markov-process.md#strong-markov-property) give

$$
P_0(H_{\{x_k\}}<\infty)
=\frac{g(0,x_k)}{g(x_k,x_k)}
\leq C|x_k|^{2-d}
=C2^{-k(d-2)}.
$$

The series over $k$ converges, so the first of the [Borel-Cantelli lemmas](../../../probability-theory.md#borel-cantelli-lemmas) says that almost surely only finitely many of the points $x_k$ are ever hit. Moreover, $\mathbb Z^d$ is a [transient graph](../../../markov-process.md#transient-graph) for $d\geq3$, so each of those finitely many points is visited only finitely often. Therefore the [simple random walk](../../../markov-process.md#simple-random-walk) visits $A$ only finitely often almost surely:

$$
\boxed{P_0(X_n\in A\text{ for infinitely many }n)=0.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

The displayed identity is false with the printed non-strict inequality. For example, take $A=B=\{y\}$ and let $r=P_y(\widetilde H_y<\infty)\in(0,1)$. The event $L_y\leq\widetilde H_y$ says that the walk returns to $y$ at most once, so its left side is $\mu_y(1-r^2)$, whereas its right side is $e_{\{y\}}(y)=\mu_y(1-r)$.

The standard and evidently intended [last-exit decomposition for a transient random walk](../../../markov-process.md#last-exit-decomposition-for-a-transient-random-walk) has $L_B<\widetilde H_A$. Decompose that corrected event according to $n=L_B$ and $z=X_n\in B$. The [Strong Markov property](../../../markov-process.md#strong-markov-property) at time $n$ gives

$$
\mu_yP_y(L_B<\widetilde H_A,L_B\geq0)
=\sum_{n\geq0}\sum_{z\in B}
\mu_yP_y(X_n=z,\widetilde H_A>n)P_z(\widetilde H_B=\infty).
$$

Reversibility of the [random walk on a graph](../../../markov-process.md#random-walk-on-a-graph) gives the path-reversal identity

$$
\mu_yP_y(X_n=z,\widetilde H_A>n)
=\mu_zP_z(X_n=y,H_A=n).
$$

Since $e_B(z)=\mu_zP_z(\widetilde H_B=\infty)$ is the [equilibrium measure of a finite set](../../../markov-process.md#equilibrium-measure-of-a-finite-set), summing first over $n$ and then over $z$ yields

$$
\boxed{\mu_yP_y(L_B<\widetilde H_A,L_B\geq0)
=\sum_{z\in B}e_B(z)P_z(X_{H_A}=y,H_A<\infty)
=P_{e_B}(X_{H_A}=y,H_A<\infty).}
$$

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Assume $A\subset B$ and use the corrected strict identity from part (i). If a walk starts at $y\in A$ and never returns to $A$, then transience makes $L_B<\infty=\widetilde H_A$. Thus

$$
\begin{aligned}
\operatorname{cap}(A)
&=\sum_{y\in A}\mu_yP_y(\widetilde H_A=\infty)\\
&\leq\sum_{y\in A}\mu_yP_y(L_B<\widetilde H_A,L_B\geq0)\\
&=P_{e_B}(H_A<\infty)\\
&\leq\sum_{z\in B}e_B(z)
=\operatorname{cap}(B).
\end{aligned}
$$

This proves monotonicity of the [capacity of a finite set for a transient random walk](../../../markov-process.md#capacity-of-a-finite-set-for-a-transient-random-walk).

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

The inequality need not be strict. Start with the nearest-neighbour [weighted graph](../../../markov-process.md#weighted-graph) $\mathbb Z^3$, attach a new [leaf](../../../graph-theory.md#leaf-of-a-graph) $b$ only to the origin $o$, and give its edge positive weight. Take $A=\{o\}$ and $B=\{o,b\}$. A walk starting from $b$ must move to $o$ at its first non-killed step, while any walk reaching $b$ from elsewhere must first pass through $o$. Hence the [equilibrium potential of a finite set](../../../markov-process.md#equilibrium-potential-of-a-finite-set) is the same for the two sets:

$$
h_A=h_B.
$$

Using $\operatorname{cap}(C)=\mathcal E(h_C,h_C)$ for a finite set $C$ gives

$$
\operatorname{cap}(A)=\operatorname{cap}(B)
$$

despite $A\ne B$.

## 2

↑ **Parent:** [Paper 226](paper-226.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [Dirichlet energy space with zero boundary at infinity](../../../markov-process.md#dirichlet-energy-space-with-zero-boundary-at-infinity) is

$$
H_0=\overline{C_c(G)}^{\,\lVert\cdot\rVert_{H_0}},
\qquad
\lVert f\rVert_{H_0}=\mathcal E(f,f)^{1/2},
$$

where $C_c(G)$ is the vector space of finitely supported real functions on the vertices. Transience makes the [Dirichlet form of a Markov chain](../../../markov-process.md#dirichlet-form-of-a-markov-chain) positive definite on this completion.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [Strong Markov property](../../../markov-process.md#strong-markov-property) at the first visit to $0$ gives the [singleton equilibrium potential from the Green function](../../../markov-process.md#singleton-equilibrium-potential-from-the-green-function)

$$
h_x=P_x(\tau<\infty)=\frac{g(x,0)}{g(0,0)}.
$$

Let $U_n$ be an increasing exhaustion of $G$ by finite sets containing $0$, and let $g_{U_n}(x,0)$ be the [Green function of a transient weighted graph](../../../markov-process.md#green-function-of-a-transient-weighted-graph) stopped on leaving $U_n$. Each $g_{U_n}(\mathord\cdot,0)$ has finite support. The Green identity and the [Markov property](../../../markov-process.md#markov-property) give, for $m\geq n$,

$$
\mathcal E\bigl(g_{U_m}(\mathord\cdot,0)-g_{U_n}(\mathord\cdot,0),
g_{U_m}(\mathord\cdot,0)-g_{U_n}(\mathord\cdot,0)\bigr)
=g_{U_m}(0,0)-g_{U_n}(0,0).
$$

By the [monotone convergence theorem](../../../measure-theory.md#monotone-convergence-theorem), the right side tends to zero as $m,n\to\infty$, while $g_{U_n}(x,0)\uparrow g(x,0)$. Thus $g(\mathord\cdot,0)$ is an $H_0$ limit of finitely supported functions. Dividing by the positive number $g(0,0)$ proves $h\in H_0$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For the normalized [Green function of a transient weighted graph](../../../markov-process.md#green-function-of-a-transient-weighted-graph), the Green identity is

$$
\mathcal E(g(\mathord\cdot,0),f)=f(0),
\qquad f\in H_0.
$$

Taking $f=g(\mathord\cdot,0)$ and using $h=g(\mathord\cdot,0)/g(0,0)$ therefore gives

$$
\mathcal E(h,h)
=\frac{\mathcal E(g(\mathord\cdot,0),g(\mathord\cdot,0))}{g(0,0)^2}
=\frac1{g(0,0)}.
$$

This is also the [capacity of a finite set for a transient random walk](../../../markov-process.md#capacity-of-a-finite-set-for-a-transient-random-walk) $\operatorname{cap}(\{0\})$.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The field $\psi$ is centered and jointly [Gaussian](../../../stochastic-process.md#gaussian-random-field). Since the [Gaussian free field](../../../stochastic-process.md#gaussian-free-field) has covariance $\mathbb E[\varphi_x\varphi_y]=g(x,y)$ and $h_x=g(x,0)/g(0,0)$,

$$
\begin{aligned}
\mathbb E[\psi_x\psi_y]
&=g(x,y)-h_xg(0,y)-h_yg(x,0)+h_xh_yg(0,0)\\
&=g(x,y)-\frac{g(x,0)g(0,y)}{g(0,0)}.
\end{aligned}
$$

Also $\psi_0=0$ and

$$
\mathbb E[\psi_x\varphi_0]=g(x,0)-h_xg(0,0)=0.
$$

Joint Gaussianity turns this zero [covariance](../../../variance.md#covariance) into independence. Therefore $\psi$ is a [Pinned Gaussian free field](../../../stochastic-process.md#pinned-gaussian-free-field) at $0$, independent of $\varphi_0$, with covariance equal to the Green function of the walk killed on hitting $0$.

## 3

↑ **Parent:** [Paper 226](paper-226.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The family $(Y_x)$ is a [Gaussian random field](../../../stochastic-process.md#gaussian-random-field). For distinct $x,x'$ its [covariance](../../../variance.md#covariance) is

$$
\operatorname{Cov}(Y_x,Y_{x'})
=\frac1{4d^2}\bigl|\{y:y\sim x\text{ and }y\sim x'\}\bigr|.
$$

Two distinct vertices of $\mathbb Z^d$ have a common neighbour exactly when their [graph distance](../../../graph-theory.md#distance-graph-theory), equivalently their $\ell^1$ distance, is two. Since jointly [Gaussian variables](../../../probability-and-statistics.md#multivariate-normal-distribution) are independent exactly when they are uncorrelated,

$$
Y_x\text{ and }Y_{x'}\text{ are independent}
\quad\Longleftrightarrow\quad
x\ne x'\text{ and }\lVert x-x'\rVert_1\ne2.
$$

**Thus the field has finite-range dependence, even though nearest-neighbour values are independent.**

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Write $p(a)=P(Y_0\geq a)$; because $Y_0\sim N(0,1+1/(2d))$, $p(a)\to0$ as $a\to\infty$. Every [path in a graph](../../../graph-theory.md#path-in-a-graph) of length $n$ contains, by a greedy selection, at least $n/M_d$ vertices at mutual [graph distance](../../../graph-theory.md#distance-graph-theory) greater than two, where $M_d=|B_2(0)|$. The corresponding field values are jointly independent by part (a). Hence the probability that a fixed path lies in the superlevel set is at most

$$
p(a)^{n/M_d}.
$$

There are at most $(2d)^n$ length-$n$ paths from the origin. The [union bound](../../../probability-inequality.md#boole-s-inequality) therefore gives

$$
P(0\longleftrightarrow\partial B_n\text{ in }\{Y\geq a\})
\leq(2d)^np(a)^{n/M_d}.
$$

Choose a finite $a$ for which $(2d)p(a)^{1/M_d}<1$ and let $n\to\infty$. There is then no unbounded component through the origin, and translation invariance rules out an unbounded component anywhere almost surely. Thus the [critical threshold for level-set percolation](../../../site-percolation.md#critical-threshold-for-level-set-percolation) satisfies $a_c(d)<\infty$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [one-arm event](../../../probability-theory.md#one-arm-event) $A_R(a)$ depends on the field values in the finite ball $B_R$. Replace $V_x$ by $U_x+a$ for $x\in B_R$. In the new variables the event has threshold zero, while the product [normal distribution](../../../probability-theory.md#normal-distribution) density is $\prod_{x\in B_R}\varphi(U_x+a)$. Differentiating this finite-dimensional integral under the integral sign gives the Gaussian shift identity

$$
-\frac d{da}\theta_R(a)
=\sum_{x\in B_R}\mathbb E[V_x\mathbf1_{A_R(a)}].
$$

This is also an instance of [Gaussian integration by parts](../../../probability-theory.md#stein-s-lemma-probability). In particular, the asserted inequality holds, in fact with equality.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Apply the [OSSS inequality](../../../probability-theory.md#osss-inequality) to the independent coordinates $(V_x,W_x)$ and to the indicator of the [one-arm event](../../../probability-theory.md#one-arm-event) $A_R(a)$. Use the randomized [OSSS exploration of a one-arm event](../../../probability-theory.md#osss-exploration-of-a-one-arm-event): choose $k$ uniformly from $\{1,\ldots,R\}$ and reveal the variables needed to explore the superlevel cluster meeting $\partial B_k$. A coordinate can be revealed only if a nearby vertex has an open connection over the relevant distance. Translation invariance, finite-range dependence and the [union bound](../../../probability-inequality.md#boole-s-inequality) therefore give the revealment estimate

$$
\delta_x\leq\frac{C_d}{R}\sum_{k=1}^R\theta_k
$$

for both kinds of coordinates, after enlarging the explored neighbourhood by a distance depending only on $d$.

For an increasing Gaussian threshold event, the resampling influence of $V_x$ is bounded by a universal constant times $\mathbb E[V_x\mathbf1_{A_R(a)}]$. The influence of $W_x$ is bounded by the sum of the corresponding $V$ influences at the $2d$ neighbours of $x$: indeed [Gaussian integration by parts](../../../probability-theory.md#stein-s-lemma-probability) gives

$$
\mathbb E[W_x\mathbf1_{A_R(a)}]
=\frac1{2d}\sum_{z\sim x}\mathbb E[V_z\mathbf1_{A_R(a)}],
$$

first for smooth increasing approximations and then by a limit. Consequently the OSSS bound becomes

$$
\theta_R(1-\theta_R)
\leq C_d\left(\frac1R\sum_{k=1}^R\theta_k\right)
\sum_{x\in B_R}\mathbb E[V_x\mathbf1_{A_R(a)}].
$$

Part (c) identifies the final sum with $-\theta_R'(a)$. Dividing and putting $c=C_d^{-1}>0$ proves

$$
-\frac d{da}\theta_R
\geq c\,
\frac{\theta_R(1-\theta_R)}{R^{-1}\sum_{k=1}^R\theta_k}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
