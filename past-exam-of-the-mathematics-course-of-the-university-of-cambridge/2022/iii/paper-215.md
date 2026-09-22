# Paper 215

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_215.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_215.pdf)

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

## 1

↑ **Parent:** [Paper 215](paper-215.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A stopping time $T$ is a [strong stationary time](../../../markov-process.md#strong-stationary-time) if

$$
\mathbb P_x(X_T=y,T=t)=\pi(y)\mathbb P_x(T=t)
$$

for every $x,y,t$. Thus $X_T\sim\pi$ and is independent of $T$. The [separation distance](../../../markov-process.md#separation-distance) is

$$
s(t)=\max_{x,y}\left\{1-\frac{P^t(x,y)}{\pi(y)}\right\}.
$$

For any strong stationary time,

$$
\begin{aligned}
P^t(x,y)
&\geq\mathbb P_x(X_t=y,T\leq t)\\
&=\sum_{j\leq t}\sum_z
\mathbb P_x(T=j,X_j=z)P^{t-j}(z,y)\\
&=\pi(y)\mathbb P_x(T\leq t).
\end{aligned}
$$

**Hence $1-P^t(x,y)/\pi(y)\leq\mathbb P_x(T>t)$, and maximizing proves the claim.**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Observe the lazy walk on $\mathbb Z_{2^k}$ only after every second genuine jump. Two independent nearest-neighbor signs have sum $-2,0,2$ with probabilities $1/4,1/2,1/4$. Division by two therefore produces one step of the lazy simple random walk on $\mathbb Z_{2^{k-1}}$. The [Strong Markov property](../../../markov-process.md#strong-markov-property) at successive jump times proves

$$
\boxed{\left(\frac{X_{T_j^{(k)}}^{(k)}}2\right)_{j\geq0}
\overset d=
\left(X_j^{(k-1)}\right)_{j\geq0}.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

At $T_{\tau_{k-1}}^{(k)}$, part b and the strong-stationarity assumption make $X^{(k)}/2$ uniform on $\mathbb Z_{2^{k-1}}$ and independent of the stopping index. One further lazy step either stays or moves by one, each parity occurring with probability one half; conditional on the even residue already selected, this chooses uniformly between its two lifts to $\mathbb Z_{2^k}$. Thus

$$
\tau_k=T_{\tau_{k-1}}^{(k)}+1
$$

has a uniform terminal state independent of $\tau_k$, and is a [strong stationary time](../../../markov-process.md#strong-stationary-time).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Take $\tau_0=0$ and apply part c recursively. A lazy walk makes a genuine jump with probability $1/2$, so the expected time required for $2j$ jumps is $4j$. Using the stated independence,

$$
\mathbb E_0\tau_k
=4\mathbb E_0\tau_{k-1}+1.
$$

The initial value zero solves this recurrence as

$$
\boxed{\mathbb E_0\tau_k=\frac{4^k-1}{3}.}
$$

## 2

↑ **Parent:** [Paper 215](paper-215.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

One step of the [Glauber dynamics](../../../statistical-physics.md#glauber-dynamics) chooses a vertex $v$ uniformly and resamples its spin from its conditional [Ising model](../../../statistical-physics.md#ising-model) distribution given all other spins. If the proposed new spin is $x$ and $S_v(\sigma)=\sum_{w\sim v}\sigma(w)$, its update probability is

$$
\boxed{\frac1n
\frac{e^{\beta xS_v(\sigma)}}
{e^{\beta S_v(\sigma)}+e^{-\beta S_v(\sigma)}}
=\frac{1+\tanh\{\beta xS_v(\sigma)\}}{2n}.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The worst-case distance to stationarity is

$$
d(t)=\max_\sigma\|P^t(\sigma,\cdot)-\pi_\beta\|_{\rm TV}.
$$

The [Path coupling theorem](../../../markov-process.md#path-coupling-theorem) says that if a coupling contracts an integer-valued path metric by a factor $\alpha<1$ for every adjacent pair, then

$$
d(t)\leq\operatorname{diam}(\Omega)\alpha^t.
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Couple two configurations differing at one vertex $u$ by choosing the same update vertex and the same uniform random number for the heat-bath update. Updating $u$ removes the disagreement. Updating a nonneighbor of $u$ cannot create one. At a neighbor $v$, the two conditional plus-spin probabilities differ by at most $\tanh\beta$, using the supplied identity. Since $u$ has at most $\Delta$ neighbors, the expected Hamming distance after one step is at most

$$
1-\frac1n+\frac{\Delta\tanh\beta}{n}
=1-\frac{1-\Delta\tanh\beta}{n}.
$$

The Hamming diameter is $n$, so the [Path coupling theorem](../../../markov-process.md#path-coupling-theorem) gives

$$
\boxed{d(t)\leq n\left(1-\frac{1-\Delta\tanh\beta}{n}\right)^t.}
$$

## 3

↑ **Parent:** [Paper 215](paper-215.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For a reversible transition matrix $P$ on $L^2(\pi)$, the [spectral gap](../../../linear-operator-theory.md#spectral-gap) is

$$
\gamma=1-\max\{\lambda:\lambda<1\text{ is an eigenvalue of }P\}.
$$

Equivalently for a lazy chain,

$$
\gamma=\inf_{\operatorname{Var}_\pi f>0}
\frac{\mathcal E_P(f,f)}{\operatorname{Var}_\pi f}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For reversible chains $P,\widetilde P$ with stationary laws $\pi,\widetilde\pi$, assign to every directed $\widetilde P$-edge $(x,y)$ a path $\Gamma_{xy}$ of $P$-edges. If

$$
A=\max_{e=(u,v)}
\frac1{\pi(u)P(u,v)}
\sum_{\Gamma_{xy}\ni e}
\widetilde\pi(x)\widetilde P(x,y)|\Gamma_{xy}|
$$

and $\widetilde\pi(x)\leq a\pi(x)$, the [Canonical paths comparison theorem](../../../markov-process.md#canonical-paths-comparison-theorem) gives $\gamma(P)\geq\gamma(\widetilde P)/(aA)$, with equivalent conventions absorbing $a$ into the congestion.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let $B=2\mathbb Z_{2n}^d$. The chain induced on $B$ by the lazy walk on $A$ has uniform stationary distribution, and an excursion from one even vertex can return there or reach only one of its $2d$ even lattice neighbors at displacement $\pm2e_i$. Its transition conductances are bounded above by constants depending only on $d$. Testing its Dirichlet quotient with

$$
f(2x)=\cos(\pi x_1/n)
$$

therefore gives

$$
\gamma_B\leq\frac{c_d}{n^2}.
$$

Indeed neighboring values differ by $O(n^{-1})$, while the variance of $f$ is bounded below uniformly. The supplied trace-chain theorem gives $\gamma_B\geq\gamma^{(2n)}(A)$, and hence

$$
\boxed{\gamma^{(2n)}(A)\leq\frac{c_d}{n^2}.}
$$

## 4

↑ **Parent:** [Paper 215](paper-215.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For stationary edge flow $Q(x,y)=\pi^G(x)P(x,y)$, the [bottleneck ratio](../../../markov-process.md#conductance-of-a-markov-chain) is

$$
\Phi_*^G
=\min_{0<\pi^G(S)\leq1/2}
\frac{Q(S,S^c)}{\pi^G(S)}.
$$

Using $f=\mathbf1_S$ in the variational characterization,

$$
\gamma^G
\leq\frac{\mathcal E(f,f)}{\operatorname{Var}_{\pi^G}f}
=\frac{Q(S,S^c)}{\pi^G(S)\pi^G(S^c)}
\leq2\frac{Q(S,S^c)}{\pi^G(S)}.
$$

Taking the infimum gives $\gamma^G\leq2\Phi_*^G$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Put $B_r=B(x,s+r)$. Every transition leaving $B_r$ enters $B_{r+1}$, and stationarity bounds its flow by the stationary mass newly reached:

$$
\pi^G(B_{r+1}\setminus B_r)\geq Q(B_r,B_r^c).
$$

While $\pi^G(B_r)\leq1/2$, the definition of $\Phi_*^G$ therefore gives

$$
\pi^G(B_{r+1})
\geq(1+\Phi_*^G)\pi^G(B_r).
$$

Iteration for $r=0,\ldots,t-1$ proves the formula.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Choose vertices $x,y$ at distance $d_G$, put $r=\lfloor(d_G-1)/4\rfloor$ and $R=\lfloor(d_G-1)/2\rfloor$. The radius-$R$ balls about $x$ and $y$ are disjoint, so one has stationary mass at most $1/2$; call its center $z$. Apply part b from radius $r$ to radius $R$:

$$
\frac12\geq\pi^G(B(z,R))
\geq\pi_*^G(1+\Phi_*^G)^{R-r}.
$$

Here the exponent should be $R-r$, and $R-r\geq(d_G-2)/4$. Therefore

$$
\Phi_*^G
\leq(2\pi_*^G)^{-4/(d_G-2)}-1.
$$

Since the [relaxation time](../../../markov-process.md#relaxation-time) is $t_{\rm rel}^G=1/\gamma^G$, part a yields

$$
\boxed{t_{\rm rel}^G
\geq
\frac1{2\Phi_*^G}
\geq
\frac1{2\{(2\pi_*^G)^{-4/(d_G-2)}-1\}}.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
