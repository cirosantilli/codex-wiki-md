# Paper 36

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper36.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper36.pdf)

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
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
    - [iii](#3/b/iii)
      - [Solution](#3/b/iii/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

In the [SI model](../../../mathematical-biology.md#si-model), one infection reduces the susceptible count by one, and the total event rate is $\lambda X(t)Y(t)/n=n\,b(X_n(t))$, where $b(u)=\lambda u(1-u)$. The [Poisson time-change representation of a Markov chain](../../../markov-process.md#poisson-time-change-representation-of-a-markov-chain) therefore gives

$$
X_n(t)=a-\frac1nN_n\left(n\int_0^t b(X_n(s))\,ds\right),
$$

where $N_n$ is a unit-rate [Poisson process](../../../probability-theory.md#poisson-process). Subtracting its clock from its count gives

$$
\boxed{\varepsilon_n(t)=\frac1n\left[
N_n\left(n\int_0^t b(X_n(s))\,ds\right)
-n\int_0^t b(X_n(s))\,ds\right]}.
$$

Thus $X_n(t)=a-\int_0^t b(X_n(s))\,ds-\varepsilon_n(t)$. The clock stops when the susceptible count reaches zero, so the representation also includes the absorbing state.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Fix $T>0$ and put $K=\lambda T/4$. Since $0\leq X_n\leq1$, the clock in part (a) is at most $nK$ on $[0,T]$. The [Poisson maximal concentration bound](../../../probability-theory.md#poisson-maximal-concentration-bound) gives, for every $\delta>0$,

$$
\mathbb P\left(\sup_{t\leq T}|\varepsilon_n(t)|>\delta\right)
\leq2\exp\left[-nK\,h(\delta/K)\right],
\qquad h(u)=(1+u)\log(1+u)-u.
$$

Here $h(u)>0$ for $u>0$, so the probabilities are summable in $n$. The [Borel-Cantelli lemma](../../../probability-theory.md#borel-cantelli-lemmas), first for positive rational $\delta$ and then for all $\delta$, yields $\sup_{t\leq T}|\varepsilon_n(t)|\to0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). No independence between the processes for different population sizes is required.

The deterministic [SI model](../../../mathematical-biology.md#si-model) solves the [logistic equation](../../../differential-equation.md#logistic-differential-equation) $x'=-\lambda x(1-x)$ with $x(0)=a$, giving

$$
\boxed{x(t)=\frac{ae^{-\lambda t}}{1-a+ae^{-\lambda t}}}.
$$

On $[0,1]$, $b$ is [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity) with constant $\lambda$. Subtracting the two integral equations gives

$$
|X_n(t)-x(t)|\leq\sup_{s\leq T}|\varepsilon_n(s)|
+\lambda\int_0^t|X_n(s)-x(s)|\,ds.
$$

The [Gronwall inequality](../../../probability-and-statistics.md#gronwall-inequality) implies

$$
\sup_{t\leq T}|X_n(t)-x(t)|
\leq e^{\lambda T}\sup_{t\leq T}|\varepsilon_n(t)|
\longrightarrow0
\quad\text{almost surely}.
$$

This is the [uniform almost-sure fluid limit of the SI model](../../../mathematical-biology.md#uniform-almost-sure-fluid-limit-of-the-si-model). One can take the intersection of the probability-one events for integer $T$ to obtain the conclusion on every finite interval. Use population sizes with $an$ integral; if the initial susceptible count is rounded, the extra initial error is at most $1/n$ and the same [Gronwall inequality](../../../probability-and-statistics.md#gronwall-inequality) proof applies.

<a id="1/b/image-susceptible-fractions-in-stochastic-si-epidemics-approach-the-deterministic-fluid-limit"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-36-si-fluid-limit.png)

**[Figure 1](#1/b/image-susceptible-fractions-in-stochastic-si-epidemics-approach-the-deterministic-fluid-limit). Susceptible fractions in stochastic SI epidemics approach the deterministic fluid limit**.

## 2

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Write $q=1-p$. A disconnected [graph](../../../graph.md) has a [connected component of a graph](../../../graph.md#component-graph-theory) of size $1\leq s\leq\lfloor n/2\rfloor$. For a fixed $s$-element [vertex set](../../../graph.md#vertex-set) $S$, all $s(n-s)$ [edges](../../../graph-theory.md#edge-of-a-graph) between $S$ and its complement must be absent. Their independent absence has probability $q^{s(n-s)}$. The [union bound](../../../probability-inequality.md#boole-s-inequality) gives

$$
\mathbb P(G(n,p)\text{ disconnected})
\leq\sum_{s=1}^{\lfloor n/2\rfloor}\binom ns q^{s(n-s)}
\leq\boxed{\sum_{s=1}^{\lfloor n/2\rfloor}
\left(nq^{n/2}\right)^s}.
$$

Set $r_n=nq^{n/2}$. Since $p$ is fixed in $(0,1)$, $r_n\to0$. For large $n$, the final sum is at most the [geometric series](../../../real-analysis.md#geometric-series) $r_n/(1-r_n)$, which tends to zero. Hence the [binomial random graph](../../../graph-theory.md#binomial-random-graph) is [connected](../../../geometry-and-topology.md#connected-space) with probability tending to one, as in [connectivity of a fixed-density binomial random graph](../../../graph-theory.md#connectivity-of-a-fixed-density-binomial-random-graph).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

For a nonnegative integer-valued [random variable](../../../random-variable.md), $\mathbf1_{\{X>0\}}\leq X$ pointwise. Taking [expectations](../../../probability-theory.md#expected-value) gives

$$
\boxed{\mathbb P(X>0)\leq\mathbb E X}.
$$

This is the indicator form of the [Markov inequality](../../../probability-inequality.md#markov-inequality).

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Let $I_{ij}$ be the [indicator random variable](../../../probability-theory.md#indicator-random-variable) that the unordered [vertex](../../../graph.md#vertex-graph-theory) pair $\{i,j\}$ has no [common neighbour](../../../graph-theory.md#common-neighbour). For each of the other $n-2$ [vertices](../../../graph.md#vertex-graph-theory), the two required [edges](../../../graph-theory.md#edge-of-a-graph) are both present with probability $p^2$. The edge pairs for different candidate neighbours are disjoint sets of independent random choices. Thus $\mathbb E I_{ij}=(1-p^2)^{n-2}$. [Linearity of expectation](../../../probability-theory.md#linearity-of-expectation) yields

$$
\boxed{\mathbb E X=\binom n2(1-p^2)^{n-2}},
$$

the [missing common-neighbour count in a binomial random graph](../../../graph-theory.md#missing-common-neighbour-count-in-a-binomial-random-graph).

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

If $X=0$, every pair of [vertices](../../../graph.md#vertex-graph-theory) has a [common neighbour](../../../graph-theory.md#common-neighbour), so every pair has [graph distance](../../../graph-theory.md#distance-graph-theory) at most two. In particular the [graph](../../../graph.md) is [connected](../../../geometry-and-topology.md#connected-space) and its [graph diameter](../../../graph-theory.md#graph-diameter) is at most two. By the [Markov inequality](../../../probability-inequality.md#markov-inequality) and part (ii),

$$
\mathbb P(\operatorname{diam}G(n,p)>2)
\leq\mathbb P(X>0)
\leq\binom n2(1-p^2)^{n-2}\longrightarrow0.
$$

We include disconnected graphs among those with diameter greater than two. Therefore

$$
\boxed{\mathbb P(\operatorname{diam}G(n,p)\leq2)\longrightarrow1},
$$

by [diameter bound for a fixed-density binomial random graph](../../../graph-theory.md#diameter-bound-for-a-fixed-density-binomial-random-graph).

## 3

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Each unordered triple of [vertices](../../../graph.md#vertex-graph-theory) is a [triangle in a graph](../../../graph.md#triangle-in-a-graph) with probability $p^3$. Consequently the [triangle count in a binomial random graph](../../../graph-theory.md#triangle-count-in-a-binomial-random-graph) satisfies $\mathbb E X=\binom n3p^3\leq(np)^3/6$. If $np\to0$, the [Markov inequality](../../../probability-inequality.md#markov-inequality) gives $\mathbb P(X>0)\leq\mathbb E X\to0$. Hence

$$
\boxed{\mathbb P(X=0)\longrightarrow1},
$$

the sparse direction of the [triangle-existence threshold in a binomial random graph](../../../graph-theory.md#triangle-existence-threshold-in-a-binomial-random-graph).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Count each unordered triple once. For a three-element [vertex set](../../../graph.md#vertex-set) $S$, let $I_S$ indicate that its three [edges](../../../graph-theory.md#edge-of-a-graph) are present. Then $X=\sum_{|S|=3}I_S$ and

$$
\mathbb E X^2=\sum_{S,T}\mathbb E[I_SI_T].
$$

If $|S\cap T|=\ell$, their edge sets have $\binom\ell2$ edges in common, so their union contains $6-\binom\ell2$ distinct [edges](../../../graph-theory.md#edge-of-a-graph). Independence gives $\mathbb E[I_SI_T]=p^{6-\binom\ell2}$. There are $\binom n3\binom3\ell\binom{n-3}{3-\ell}$ such ordered pairs: choose $S$, its shared vertices, and the remaining vertices of $T$. Thus

$$
\boxed{\mathbb E X^2=
\binom n3\sum_{\ell=0}^3
\binom3\ell\binom{n-3}{3-\ell}
p^{6-\binom\ell2}}.
$$

This overlap count is the basis of [triangle variance in a binomial random graph](../../../graph-theory.md#triangle-variance-in-a-binomial-random-graph).

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

When $\mu=\mathbb E X>0$, the event $X=0$ implies $|X-\mu|\geq\mu$. The [Chebyshev inequality](../../../probability-inequality.md#chebyshev-inequality) therefore gives

$$
\boxed{\mathbb P(X=0)\leq
\frac{\operatorname{Var}(X)}{(\mathbb E X)^2}}.
$$

This is the [second moment method](../../../probability-inequality.md#second-moment-method) for proving that a nonnegative count is positive.

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

Two distinct [triangles in a graph](../../../graph.md#triangle-in-a-graph) with at most one common [vertex](../../../graph.md#vertex-graph-theory) use disjoint [edges](../../../graph-theory.md#edge-of-a-graph), so their [indicator random variables](../../../probability-theory.md#indicator-random-variable) are independent and have zero [covariance](../../../variance.md#covariance). A pair sharing an edge has covariance $p^5-p^6$. The count from part (i) gives

$$
\operatorname{Var}(X)
=\binom n3p^3(1-p^3)
+3\binom n3(n-3)p^5(1-p).
$$

With $\mu=\binom n3p^3$, the [triangle variance in a binomial random graph](../../../graph-theory.md#triangle-variance-in-a-binomial-random-graph) therefore satisfies

$$
\frac{\operatorname{Var}(X)}{\mu^2}
\leq\frac1{\binom n3p^3}
+\frac{3(n-3)}{\binom n3p}
=O((np)^{-3})+O((n^2p)^{-1}).
$$

Both terms tend to zero when $np\to\infty$, because $n^2p=n(np)\to\infty$. Applying part (ii) proves

$$
\boxed{\mathbb P(X>0)\longrightarrow1},
$$

completing the [triangle-existence threshold in a binomial random graph](../../../graph-theory.md#triangle-existence-threshold-in-a-binomial-random-graph).

## 4

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Take the initial removed set to be empty, as required by the displayed equality in this [discrete SIR epidemic on a graph](../../../mathematical-biology.md#discrete-sir-epidemic-on-a-graph). If initially removed individuals are allowed, add their indicators $Y_i(0)$ to the final-removal count; an isolated initially removed [vertex](../../../graph.md#vertex-graph-theory) already shows why this correction is necessary. Condition on a fixed initial infection vector.

Given the history through time $k$, the [union bound](../../../probability-inequality.md#boole-s-inequality) over currently infected [neighbours](../../../graph-theory.md#neighbour-of-a-vertex) gives

$$
\mathbb E[X_i(k+1)\mid\mathcal F_k]
\leq\beta\sum_jA_{ij}X_j(k).
$$

Write $u(k)=\mathbb E X(k)$. Taking [expectations](../../../probability-theory.md#expected-value) and iterating this componentwise inequality for the nonnegative [adjacency matrix of a graph](../../../graph-theory.md#adjacency-matrix) gives $u(k)\leq(\beta A)^kX(0)$.

A [vertex](../../../graph.md#vertex-graph-theory) is infected at most once, and an infection lasts exactly one step before permanent removal. Hence $Y_i(\infty)=\sum_{k\geq0}X_i(k)$ under the stated initial convention. The [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) now gives

$$
\boxed{\mathbb P(Y_i(\infty)=1)
=\mathbb P(i\text{ is ever infected})
\leq\sum_{k=0}^\infty\sum_j
\beta^k(A^k)_{ij}X_j(0)}.
$$

The [walk count from powers of an adjacency matrix](../../../graph-theory.md#walk-count-from-powers-of-an-adjacency-matrix) explains the terms: all possible transmission [walks](../../../graph-theory.md#walk-in-a-graph) are counted, including [walks](../../../graph-theory.md#walk-in-a-graph) that overcount because removal prevents reinfection. This is the [adjacency-matrix bound for a discrete SIR epidemic](../../../mathematical-biology.md#adjacency-matrix-bound-for-a-discrete-sir-epidemic).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Put $Z=\sum_iY_i(\infty)$ and $\mathbf1=(1,\ldots,1)^T$. Sum the bounds in part (a) over the [vertices](../../../graph.md#vertex-graph-theory), using [linearity of expectation](../../../probability-theory.md#linearity-of-expectation) and the [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) for the nonnegative series:

$$
\boxed{\mathbb E Z\leq
\mathbf1^T\sum_{k=0}^\infty(\beta A)^kX(0)}.
$$

The bound remains valid if the series diverges, although it then gives no finite estimate. When the [spectral radius](../../../analysis.md#spectral-radius) of $\beta A$ is less than one, the series is a [Neumann series](../../../banach-algebra.md#neumann-series), giving the [resolvent bound for a discrete SIR epidemic](../../../mathematical-biology.md#resolvent-bound-for-a-discrete-sir-epidemic).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Because $A$ is a real [symmetric matrix](../../../linear-algebra.md#symmetric-matrix), the [spectral theorem](../../../hilbert-space.md#spectral-theorem) gives $\|A\|_2=\rho(A)$. For $\beta\rho<1$, the [Neumann series](../../../banach-algebra.md#neumann-series) satisfies

$$
R=(I-\beta A)^{-1}=\sum_{k=0}^\infty(\beta A)^k,
\qquad \|R\|_2\leq\frac1{1-\beta\rho}.
$$

Let $m=\sum_iX_i(0)$ be the initial infected count. Since its entries are [indicator random variables](../../../probability-theory.md#indicator-random-variable), $\|X(0)\|_2=\sqrt m$, while $\|\mathbf1\|_2=\sqrt n$. The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) and the [operator norm](../../../continuous-dual-space.md#operator-norm) bound yield

$$
\boxed{\mathbb E Z\leq
\frac{\sqrt{nm}}{1-\beta\rho}}.
$$

Thus a sufficient asymptotic condition for a small outbreak is

$$
\boxed{\frac{\sqrt{m/n}}{1-\beta\rho}\longrightarrow0}.
$$

For example, it holds when $m=o(n)$ and $\beta\rho\leq1-\eta$ for a fixed $\eta>0$. For any fixed $\delta>0$, the [Markov inequality](../../../probability-inequality.md#markov-inequality) then gives

$$
\mathbb P(Z\geq\delta n)\leq
\frac{\sqrt{m/n}}{\delta(1-\beta\rho)}\longrightarrow0.
$$

This is the [spectral condition for a small discrete SIR outbreak](../../../mathematical-biology.md#spectral-condition-for-a-small-discrete-sir-outbreak). A uniform gap and few initial infections are needed for this conclusion; the finite-population condition $\beta\rho<1$ alone does not control an asymptotically vanishing gap or an initially macroscopic infected set.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
