# Paper 215

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_215.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_215.pdf)

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

## 1

↑ **Parent:** [Paper 215](paper-215.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For [probability distributions](../../../probability-theory.md#probability-distribution) on a finite [set](../../../set.md), the [total variation distance](../../../probability-and-statistics.md#total-variation-distance) is

$$
\|\mu-\nu\|_{\mathrm{TV}}=\max_{A\subseteq S}|\mu(A)-\nu(A)|=\frac12\sum_{z\in S}|\mu(z)-\nu(z)|.
$$

The equality follows by taking $A=\{z:\mu(z)\geq\nu(z)\}$: the positive and negative parts of $\mu-\nu$ have the same mass, since its total mass is zero.

Use the [stationary distribution](../../../markov-process.md#stationary-distribution) identity $\pi P^t=\pi$. For each initial state $x$,

$$
P^t(x,\cdot)-\pi=\sum_y\pi(y)\bigl(P^t(x,\cdot)-P^t(y,\cdot)\bigr).
$$

The [triangle inequality](../../../topological-analysis.md#triangle-inequality) for [total variation distance](../../../probability-and-statistics.md#total-variation-distance), followed by the definition of the [pairwise mixing diameter](../../../markov-process.md#pairwise-mixing-diameter), gives

$$
\|P^t(x,\cdot)-\pi\|_{\mathrm{TV}}\leq\sum_y\pi(y)\bar d(t)=\bar d(t).
$$

Taking the maximum over $x$ proves $\boxed{d(t)\leq\bar d(t)}$. This particular inequality only needs a [stationary distribution](../../../markov-process.md#stationary-distribution); it does not require an [irreducible Markov chain](../../../markov-process.md#irreducible-markov-chain) or an [aperiodic Markov chain](../../../markov-process.md#aperiodic-markov-chain).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

A [coupling of probability distributions](../../../probability-and-statistics.md#coupling) is a [joint probability distribution](../../../probability-theory.md#joint-probability-distribution) of [random variables](../../../random-variable.md) $(X,Y)$ with the specified [marginal distributions](../../../probability-theory.md#marginal-distribution): $\mathbb P(X\in A)=\mu(A)$ and $\mathbb P(Y\in A)=\nu(A)$. No [independence](../../../random-variable.md#independent-random-variables) is required.

For every [set](../../../set.md) $A$, the difference of the two indicator functions vanishes when $X=Y$. Consequently

$$
|\mu(A)-\nu(A)|=\left|\mathbb E\bigl(\mathbf1_A(X)-\mathbf1_A(Y)\bigr)\right|\leq\mathbb P(X\ne Y).
$$

Maximizing over $A$ gives the [coupling inequality for total variation](../../../probability-and-statistics.md#coupling-inequality-for-total-variation):

$$
\boxed{\|\mu-\nu\|_{\mathrm{TV}}\leq\mathbb P(X\ne Y).}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $R$ interchange the two [complete graphs](../../../graph-theory.md#complete-graph), sending $v_i$ to $v_i'$ and fixing $w$. This [involution](../../../group-theory.md#involution) preserves the [transition matrix](../../../markov-process.md#stochastic-matrix) of the [simple random walk](../../../markov-process.md#simple-random-walk). A [mirror coupling under an involution](../../../probability-and-statistics.md#mirror-coupling-under-an-involution) starts $X$ at $v_i$, keeps $Y_t=R(X_t)$ until the [hitting time](../../../markov-process.md#first-passage-time) $\tau$ of $w$, and then makes the two walks move identically. Each coordinate has the correct [transition probabilities](../../../markov-process.md#transition-probability), and they coalesce precisely at $\tau$. The [coupling inequality for total variation](../../../probability-and-statistics.md#coupling-inequality-for-total-variation) gives

$$
\boxed{\|P^t(v_i,\cdot)-P^t(v_i',\cdot)\|_{\mathrm{TV}}\leq\mathbb P_{v_i}(\tau>t).}
$$

There is a genuine error in the printed [expected hitting time](../../../markov-process.md#expected-hitting-time) bound, as well as an unspecified initial law. For $n\geq2$, write $a=\mathbb E_{v_1}\tau$ and $b=\mathbb E_{v_i}\tau$ for $i\ne1$. From every clique vertex there is a positive chance of reaching $w$ within two steps, uniformly over the finite state space for each fixed $n$, so $\tau$ has finite [expected value](../../../probability-theory.md#expected-value). [First-step analysis](../../../analysis.md#first-step-analysis), using the [degree of a vertex](../../../graph-theory.md#degree-graph-theory) $n$ at $v_1$ and $n-1$ at the other clique vertices, gives

$$
a=1+\frac{n-1}{n}b,\qquad b=1+\frac{a+(n-2)b}{n-1}.
$$

Solving these [linear equations](../../../linear-algebra.md#linear-equation) yields

$$
\boxed{a=n^2-n+1,\qquad b=n^2,\qquad \mathbb E_w\tau=0.}
$$

In particular even the attachment vertex exceeds the printed bound by one. The valid uniform replacement is $\max_x\mathbb E_x\tau\leq n^2$, the [hitting time of the bridge vertex between two cliques](../../../markov-process.md#hitting-time-of-the-bridge-vertex-between-two-cliques) formula.

We must also handle arbitrary starting states, including $w$, before applying the mirror argument. Identify related vertices and consider the [lumped Markov chain](../../../markov-process.md#lumped-markov-chain) $Z$ on $\{1,\ldots,n,w\}$. Its [transition matrix](../../../markov-process.md#stochastic-matrix) $Q$ has $Q(1,j)=1/n$ for $j\ne1$, $Q(1,w)=1/n$, $Q(i,j)=1/(n-1)$ for $i\ne1$ and $j\ne i$, and $Q(w,1)=1$, with all other entries zero. Here the row for $i\ne1$ only ranges over $j\in\{1,\ldots,n\}$.

For $n\geq3$ and $j\in\{2,\ldots,n\}$, direct two-step calculation gives

$$
\begin{aligned}
Q^2(w,j)&=1/n, &Q^2(1,j)&=(n-2)/(n(n-1)),\\
Q^2(i,i)&=(n-2)/(n-1)^2+1/(n(n-1)),\quad&i\geq2,\\
Q^2(i,j)&=(n-3)/(n-1)^2+1/(n(n-1)),\quad&i,j\geq2,\ i\ne j.
\end{aligned}
$$

All these entries are at least $1/(2n)$. Thus $Q^2(z,\cdot)\geq\alpha\nu(\cdot)$ for every $z$, where $\nu$ is the [uniform distribution on a finite set](../../../discrete-probability-distribution.md#discrete-uniform-distribution) $\{2,\ldots,n\}$ and $\alpha=(n-1)/(2n)\geq1/3$. This is a [Doeblin condition](../../../statistical-inference.md#doeblin-s-condition). At each two-step block couple the two quotient endpoints to the same sample from $\nu$ with probability $\alpha$, using the residual [probability distributions](../../../probability-theory.md#probability-distribution) otherwise. The first successful block has [expected value](../../../probability-theory.md#expected-value) at most $1/\alpha$, so the alignment time $A$ has $\mathbb E A\leq6$. Lift each endpoint [coupling of probability distributions](../../../probability-and-statistics.md#coupling) to the original walks by their conditional two-step path laws; this preserves every marginal path law. The success test uses fresh block randomness and so permits restarting the walks with their original [transition matrix](../../../markov-process.md#stochastic-matrix) at the aligned endpoints.

At alignment the original walks are equal or related. Use identical transitions in the first case and the [mirror coupling under an involution](../../../probability-and-statistics.md#mirror-coupling-under-an-involution) in the second. The resulting [coalescing coupling](../../../probability-and-statistics.md#coalescing-coupling) has coalescence time $T$ satisfying $\mathbb E T\leq6+n^2$ for every pair of initial states. Therefore [Markov inequality](../../../probability-inequality.md#markov-inequality) and the [pairwise mixing diameter](../../../markov-process.md#pairwise-mixing-diameter) imply

$$
d(t)\leq\bar d(t)\leq\sup_{x,y}\mathbb P_{x,y}(T>t)\leq\frac{n^2+6}{t},\qquad
\boxed{t_{\mathrm{mix}}(1/4)\leq\lceil4(n^2+6)\rceil=O(n^2).}
$$

For the hint's particular starting states, the quotient one-step laws from two different clique indices have a common component of mass at least $1-2/n$: for two ordinary indices it is $(n-2)/(n-1)$; for one attachment index it is $(n-2)/n$. A [maximal coupling](../../../probability-and-statistics.md#maximal-coupling) therefore aligns those indices with probability $1-O(1/n)$, as suggested. The two-step argument above additionally covers $w$.

The nonlazy walk is an [aperiodic Markov chain](../../../markov-process.md#aperiodic-markov-chain) for $n\geq3$, because the connected [graph](../../../graph.md) contains a [triangle](../../../geometry-and-topology.md#triangle). For $n=1,2$ it is a [periodic Markov chain](../../../markov-process.md#periodic-markov-chain) on a [bipartite graph](../../../graph-theory.md#bipartite-graph); each bipartition class has stationary mass $1/2$, and the walk stays on a single class at each time. Hence $d(t)\geq1/2$ and the $1/4$ [mixing time](../../../markov-process.md#mixing-time-of-a-markov-chain) is infinite. The asymptotic conclusion is valid for $n\geq3$.

## 2

↑ **Parent:** [Paper 215](paper-215.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For a finite [irreducible Markov chain](../../../markov-process.md#irreducible-markov-chain) that is an [aperiodic Markov chain](../../../markov-process.md#aperiodic-markov-chain), set

$$
d_n(t)=\max_x\|P_n^t(x,\cdot)-\pi_n\|_{\mathrm{TV}},\qquad
\boxed{t_{\mathrm{mix}}^{(n)}(\alpha)=\min\{t\in\mathbb Z_{\geq0}:d_n(t)\leq\alpha\}.}
$$

Here $\pi_n$ is its unique [stationary distribution](../../../markov-process.md#stationary-distribution), and the distance is [total variation distance](../../../probability-and-statistics.md#total-variation-distance). Applying a [Markov kernel](../../../markov-process.md#markov-kernel) contracts [total variation distance](../../../probability-and-statistics.md#total-variation-distance), so $d_n(t)$ is nonincreasing and the minimum is finite.

Use the [ratio definition of cutoff](../../../markov-process.md#ratio-definition-of-cutoff): a family has [cutoff for Markov chains](../../../markov-process.md#cutoff-for-markov-chains) if, for every fixed $0<\varepsilon<1/2$,

$$
\boxed{\frac{t_{\mathrm{mix}}^{(n)}(\varepsilon)}{t_{\mathrm{mix}}^{(n)}(1-\varepsilon)}\longrightarrow1,}
$$

with the denominator positive eventually. Thus the transition between any two fixed distance levels takes negligible time compared with the [mixing time](../../../markov-process.md#mixing-time-of-a-markov-chain) scale. By monotonicity and squeezing, this also gives $t_{\mathrm{mix}}^{(n)}(\alpha)/t_{\mathrm{mix}}^{(n)}(\beta)\to1$ for any fixed $\alpha,\beta\in(0,1)$.

Some definitions of [cutoff for Markov chains](../../../markov-process.md#cutoff-for-markov-chains) additionally require the [mixing time](../../../markov-process.md#mixing-time-of-a-markov-chain) to diverge. That extra requirement cannot be built into the definition here: the final request in part (d) explicitly asks for a bounded-time counterexample. The ratio convention is the one consistent with that request.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Take the real [inner product](../../../linear-algebra.md#inner-product)

$$
\langle f,g\rangle_\pi=\sum_{x\in S}\pi(x)f(x)g(x).
$$

The [stationary distribution](../../../markov-process.md#stationary-distribution) is strictly positive for an [irreducible Markov chain](../../../markov-process.md#irreducible-markov-chain). [Detailed balance](../../../markov-process.md#detailed-balance) gives $\langle Pf,g\rangle_\pi=\langle f,Pg\rangle_\pi$, so $P$ is a [self-adjoint operator](../../../linear-operator-theory.md#self-adjoint-operator). Choose a real [orthonormal eigenbasis](../../../linear-operator-theory.md#orthonormal-eigenbasis) $f_1,\ldots,f_m$, where $m=|S|$, $Pf_j=\lambda_jf_j$, $f_1\equiv1$, $\lambda_1=1$, and $\pi(f_j)=0$ for $j\geq2$.

For fixed $y$, apply the [spectral decomposition](../../../linear-operator-theory.md#spectral-decomposition) to $g_y(z)=\mathbf1_{\{y\}}(z)/\pi(y)$. Its coefficient against $f_j$ is $f_j(y)$, whereas $(P^tg_y)(x)=P^t(x,y)/\pi(y)$. Thus the [spectral kernel expansion of a reversible chain](../../../markov-process.md#spectral-kernel-expansion-of-a-reversible-chain) is

$$
\boxed{\frac{P^t(x,y)}{\pi(y)}=\sum_{j=1}^{m}\lambda_j^t f_j(x)f_j(y).}
$$

This holds for all integers $t\geq0$; at $t=0$ each multiplier is one, including when $\lambda_j=0$. Negative [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are allowed, and retain their signs for odd $t$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $m\geq2$ be the number of states and put

$$
r=\max_{2\leq j\leq m}|\lambda_j|,\qquad
\boxed{\gamma_*=1-r,\qquad t_{\mathrm{rel}}=\gamma_*^{-1}.}
$$

The [absolute L2 spectral gap of a reversible Markov chain](../../../statistical-inference.md#absolute-l2-spectral-gap-of-a-reversible-markov-chain) is $\gamma_*$; in this question the [relaxation time](../../../markov-process.md#relaxation-time) means the [absolute relaxation time](../../../markov-process.md#absolute-relaxation-time). For a nonlazy [reversible Markov chain](../../../markov-process.md#reversible-markov-chain), it may differ from the reciprocal of the ordinary [spectral gap](../../../linear-operator-theory.md#spectral-gap) $1-\lambda_2$. For a finite [irreducible Markov chain](../../../markov-process.md#irreducible-markov-chain) that is an [aperiodic Markov chain](../../../markov-process.md#aperiodic-markov-chain), $r<1$.

For $r>0$, choose a real [eigenfunction](../../../linear-operator-theory.md#eigenfunction) $f$ whose [eigenvalue](../../../linear-operator-theory.md#eigenvalue) has modulus $r$, and an initial state $x$ maximizing $|f(x)|=\|f\|_\infty$. It has $\pi(f)=0$, and the definition of [total variation distance](../../../probability-and-statistics.md#total-variation-distance) implies

$$
r^t\|f\|_\infty=|P^tf(x)-\pi(f)|\leq2\|f\|_\infty\|P^t(x,\cdot)-\pi\|_{\mathrm{TV}}.
$$

This is the [eigenvalue lower bound for total variation mixing](../../../markov-process.md#eigenvalue-lower-bound-for-total-variation-mixing), $d(t)\geq r^t/2$. At $t=t_{\mathrm{mix}}(\varepsilon)$, for $0<\varepsilon<1/2$,

$$
t\geq\frac{\log(1/(2\varepsilon))}{-\log r}\geq\frac{r}{1-r}\log\frac1{2\varepsilon}.
$$

The second inequality follows from $-r\log r\leq1-r$, the supplied inequality with $x=1-r$. Since $r/(1-r)=t_{\mathrm{rel}}-1$,

$$
\boxed{(t_{\mathrm{rel}}-1)\log\frac1{2\varepsilon}\leq t_{\mathrm{mix}}(\varepsilon).}
$$

When $r=0$ the left side is zero, so no logarithm of zero is needed. For $\varepsilon\geq1/2$ the left side is nonpositive and the conclusion is automatic. A one-state chain has [mixing time](../../../markov-process.md#mixing-time-of-a-markov-chain) zero; with the convention $\gamma_*=1$ the bound is again trivial.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Use the [ratio definition of cutoff](../../../markov-process.md#ratio-definition-of-cutoff) from part (a), and write $T_n=t_{\mathrm{mix}}^{(n)}(1/4)$. In the [reversible Markov chain](../../../markov-process.md#reversible-markov-chain) setting of the preceding parts let $\gamma_n=1-\lambda_{2,n}$ and $\gamma_{*,n}=1-\max_{j\geq2}|\lambda_{j,n}|$. In particular $\gamma_{*,n}\leq\gamma_n$.

If $\gamma_nT_n$ did not tend to infinity, there would be a subsequence and $B>0$ for which $\gamma_nT_n\leq B$. Along it part (c) implies, for every fixed $0<\varepsilon<1/2$,

$$
\frac{t_{\mathrm{mix}}^{(n)}(\varepsilon)}{T_n}
\geq\left(\frac1{\gamma_{*,n}T_n}-\frac1{T_n}\right)\log\frac1{2\varepsilon}
\geq\left(\frac1B-\frac1{T_n}\right)\log\frac1{2\varepsilon}.
$$

Since $T_n\to\infty$, choose fixed $\varepsilon$ so small that $\log(1/(2\varepsilon))>B$. The lower limit of this ratio is then greater than one, contradicting [cutoff for Markov chains](../../../markov-process.md#cutoff-for-markov-chains). Thus the [Peres product condition](../../../markov-process.md#peres-product-condition) holds:

$$
\boxed{\gamma_nT_n\longrightarrow\infty.}
$$

In fact the argument with $\gamma_{*,n}$ proves the stronger absolute-gap product condition. Part (d) does not repeat the [reversible Markov chain](../../../markov-process.md#reversible-markov-chain) hypothesis; the ordinary real ordering of [eigenvalues](../../../linear-operator-theory.md#eigenvalue) above uses that hypothesis. If arbitrary chains are intended, define the [spectral gap](../../../linear-operator-theory.md#spectral-gap) explicitly: the [eigenvalue lower bound for total variation mixing](../../../markov-process.md#eigenvalue-lower-bound-for-total-variation-mixing) works for complex [eigenfunctions](../../../linear-operator-theory.md#eigenfunction) too, and proves the same assertion for $\gamma_*$ or for $1-\max_{j\geq2}\operatorname{Re}\lambda_j$, which is at least $\gamma_*$. No real ordering of complex [eigenvalues](../../../linear-operator-theory.md#eigenvalue) is implicit.

For the requested counterexample take nonlazy [simple random walk](../../../markov-process.md#simple-random-walk) on the [complete graph](../../../graph-theory.md#complete-graph) $K_n$, $n\geq3$. Let $\Pi$ have every row equal to the [uniform distribution on a finite set](../../../discrete-probability-distribution.md#discrete-uniform-distribution), and let $a=-1/(n-1)$. Then

$$
P=\Pi+a(I-\Pi),\quad P^t=\Pi+a^t(I-\Pi),\quad
\boxed{d_n(t)=\left(1-\frac1n\right)(n-1)^{-t}.}
$$

Thus $d_n(0)\to1$ and $d_n(1)=1/n\to0$: every fixed-level [mixing time](../../../markov-process.md#mixing-time-of-a-markov-chain) is eventually one. This is a bounded-time jump satisfying the [ratio definition of cutoff](../../../markov-process.md#ratio-definition-of-cutoff). The ordinary [spectral gap](../../../linear-operator-theory.md#spectral-gap) is $n/(n-1)$ and the absolute one is $(n-2)/(n-1)$, so both products with $T_n=1$ tend to one, not infinity. The divergence assumption on $T_n$ is therefore essential under this convention.

## 3

↑ **Parent:** [Paper 215](paper-215.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

On a finite state space with at least two states, as in the surrounding questions, for a real function write $\pi(f)=\sum_x\pi(x)f(x)$ and $\operatorname{Var}_\pi(f)=\sum_x\pi(x)(f(x)-\pi(f))^2$. The [Poincare inequality for a reversible Markov chain](../../../markov-process.md#poincare-inequality-for-a-reversible-markov-chain) with constant $C$ is

$$
\boxed{\operatorname{Var}_\pi(f)\leq C\mathcal E(f,f)\quad\text{for every }f,}
$$

where the [Dirichlet form of a Markov chain](../../../markov-process.md#dirichlet-form-of-a-markov-chain) is

$$
\mathcal E(f,f)=\frac12\sum_{x,y}\pi(x)P(x,y)(f(x)-f(y))^2=\langle f,(I-P)f\rangle_\pi.
$$

The associated [spectral gap](../../../linear-operator-theory.md#spectral-gap) is the ordinary gap $\gamma=1-\lambda_2$, with variational formula

$$
\boxed{\gamma=\inf_{\operatorname{Var}_\pi(f)>0}\frac{\mathcal E(f,f)}{\operatorname{Var}_\pi(f)}.}
$$

Equivalently minimize $\mathcal E(f,f)$ subject to $\pi(f)=0$ and $\langle f,f\rangle_\pi=1$. Thus the [Poincare inequality for a reversible Markov chain](../../../markov-process.md#poincare-inequality-for-a-reversible-markov-chain) holds precisely for $C\geq1/\gamma$, and the optimal constant is $1/\gamma$. It controls the ordinary rather than absolute [spectral gap](../../../linear-operator-theory.md#spectral-gap), so negative [eigenvalues](../../../linear-operator-theory.md#eigenvalue) do not invalidate it. If the unspecified state space in this part is infinite, the [Poincare inequality for a reversible Markov chain](../../../markov-process.md#poincare-inequality-for-a-reversible-markov-chain) and the variational infimum still make sense on nonconstant functions in $L^2(\pi)$, using the [self-adjoint operator](../../../linear-operator-theory.md#self-adjoint-operator) on that [Hilbert space](../../../hilbert-space.md); the resulting [spectral gap](../../../linear-operator-theory.md#spectral-gap) need not be represented by an actual second [eigenvalue](../../../linear-operator-theory.md#eigenvalue). The finite-state formula above is the intended specialization.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For a finite [irreducible Markov chain](../../../markov-process.md#irreducible-markov-chain) satisfying [detailed balance](../../../markov-process.md#detailed-balance), define the directed-edge capacity $Q(u,v)=\pi(u)P(u,v)$. For every ordered pair $(x,y)$ choose a [path](../../../geometry-and-topology.md#continuous-path) $\eta_{xy}$ from $x$ to $y$ using only positive-capacity [edges](../../../graph-theory.md#edge-of-a-graph); take the empty [path](../../../geometry-and-topology.md#continuous-path) for $x=y$. Let $N_e(\eta)$ count occurrences of the directed [edge](../../../graph-theory.md#edge-of-a-graph) $e$. The [canonical paths Poincare bound](../../../markov-process.md#canonical-paths-poincare-bound) says that

$$
\rho=\max_{e:Q(e)>0}\frac{1}{Q(e)}\sum_{x,y}\pi(x)\pi(y)|\eta_{xy}|N_e(\eta_{xy})
$$

is a valid [Poincare inequality for a reversible Markov chain](../../../markov-process.md#poincare-inequality-for-a-reversible-markov-chain) constant. Simple [paths](../../../geometry-and-topology.md#continuous-path) give $N_e\in\{0,1\}$; allowing repetitions requires the multiplicities shown.

To prove the theorem, expand the [variance](../../../variance.md) using two independent samples from $\pi$:

$$
\operatorname{Var}_\pi(f)=\frac12\sum_{x,y}\pi(x)\pi(y)(f(x)-f(y))^2.
$$

Telescoping along $\eta_{xy}$ and applying the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
(f(x)-f(y))^2\leq|\eta_{xy}|\sum_eN_e(\eta_{xy})(f(e^-)-f(e^+))^2.
$$

Interchange the finite sums, then use the definition of $\rho$:

$$
\begin{aligned}
\operatorname{Var}_\pi(f)&\leq\frac12\sum_e(f(e^-)-f(e^+))^2\sum_{x,y}\pi(x)\pi(y)|\eta_{xy}|N_e(\eta_{xy})\\
&\leq\frac\rho2\sum_eQ(e)(f(e^-)-f(e^+))^2=\rho\mathcal E(f,f).
\end{aligned}
$$

Consequently $\boxed{\operatorname{Var}_\pi(f)\leq\rho\mathcal E(f,f),\quad\gamma\geq1/\rho}$. All [edges](../../../graph-theory.md#edge-of-a-graph) here are directed, so the $1/2$ in the [Dirichlet form of a Markov chain](../../../markov-process.md#dirichlet-form-of-a-markov-chain) is retained consistently.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [lazy Markov chain](../../../markov-process.md#lazy-markov-chain) has holding probability $1/2$ and [transition probability](../../../markov-process.md#transition-probability) $1/(2n)$ to each neighbour in the [hypercube graph](../../../graph.md#hypercube-graph). Its [stationary distribution](../../../markov-process.md#stationary-distribution) is $\pi(x)=2^{-n}$ by symmetry.

For $(x,y)$ choose the [path](../../../geometry-and-topology.md#continuous-path) changing the differing coordinates in increasing order. Its length is at most $n$. Fix a directed [edge](../../../graph-theory.md#edge-of-a-graph) $(u,u^{(k)})$ that flips coordinate $k$. A [path](../../../geometry-and-topology.md#continuous-path) uses this [edge](../../../graph-theory.md#edge-of-a-graph) exactly when $x_k=u_k$, $y_k=-u_k$, $y_j=u_j$ for $j<k$, and $x_j=u_j$ for $j>k$. The coordinates $x_j$ for $j<k$ and $y_j$ for $j>k$ are free. Thus exactly $2^{n-1}$ ordered pairs use it, while

$$
Q(u,u^{(k)})=\frac{2^{-n}}{2n},\qquad
\sum_{(x,y):e\in\eta_{xy}}\pi(x)\pi(y)=2^{n-1}2^{-2n}=2^{-n-1}.
$$

The unweighted load divided by capacity equals $n$; multiplying by the maximum length yields $\rho\leq n^2$. The [canonical paths Poincare bound](../../../markov-process.md#canonical-paths-poincare-bound) therefore proves the slightly stronger $\operatorname{Var}_\pi(f)\leq n^2\mathcal E(f,f)$, and in particular the requested

$$
\boxed{\operatorname{Var}_\pi(f)\leq2n^2\mathcal E(f,f),\qquad\gamma\geq\frac1{2n^2}.}
$$

One can keep the actual lengths: among these $2^{n-1}$ pairs, coordinate $k$ always differs, and each of the other $n-1$ coordinates differs for half the pairs. Their mean [path](../../../geometry-and-topology.md#continuous-path) length is $(n+1)/2$, giving exact congestion $\rho=n(n+1)/2$. This refinement still has order $n^2$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For each [subset](../../../set.md#subset) $J\subseteq\{1,\ldots,n\}$, take the [Walsh character](../../../combinatorics.md#walsh-character) $f_J(x)=\prod_{j\in J}x_j$, including $f_\varnothing\equiv1$. Under the [uniform distribution on a finite set](../../../discrete-probability-distribution.md#discrete-uniform-distribution) these functions are an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis): $f_Jf_K=f_{J\triangle K}$ has mean zero unless $J=K$, since the coordinates are independent fair signs. There are $2^n$ such functions, the full dimension of the function space.

Flipping a coordinate in $J$ changes the sign, while flipping one outside $J$ leaves the value unchanged. The total probability of a sign change is $|J|/(2n)$, so

$$
Pf_J=\left(1-\frac{|J|}{n}\right)f_J.
$$

The [spectrum of lazy random walk on the hypercube](../../../markov-process.md#spectrum-of-lazy-random-walk-on-the-hypercube) is therefore

$$
\boxed{\lambda_k=1-\frac{k}{n}\quad\text{with multiplicity }\binom nk,\quad0\leq k\leq n.}
$$

All [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are nonnegative and the second largest is $1-1/n$. Hence both the ordinary [spectral gap](../../../linear-operator-theory.md#spectral-gap) and the absolute [spectral gap](../../../linear-operator-theory.md#spectral-gap) equal $\boxed{\gamma=1/n}$. The requested bound in part (c) is smaller than the exact gap by a factor $2n$; even the refined increasing-coordinate [canonical paths Poincare bound](../../../markov-process.md#canonical-paths-poincare-bound) loses a factor $(n+1)/2$. The true optimal [Poincare inequality for a reversible Markov chain](../../../markov-process.md#poincare-inequality-for-a-reversible-markov-chain) constant is $n$.

## 4

↑ **Parent:** [Paper 215](paper-215.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Use $\langle f,g\rangle_\pi=\sum_x\pi(x)f(x)g(x)$. The [Dirichlet form of a Markov chain](../../../markov-process.md#dirichlet-form-of-a-markov-chain) is

$$
\boxed{\mathcal E(f,f)=\langle f,(I-P)f\rangle_\pi=\frac12\sum_{x,y}\pi(x)P(x,y)(f(x)-f(y))^2.}
$$

The equality follows by expanding the square and using row sums one and the [stationary distribution](../../../markov-process.md#stationary-distribution) identity. For the [reversible Markov chain](../../../markov-process.md#reversible-markov-chain), [detailed balance](../../../markov-process.md#detailed-balance) makes $P$ a [self-adjoint operator](../../../linear-operator-theory.md#self-adjoint-operator), with real [orthonormal eigenbasis](../../../linear-operator-theory.md#orthonormal-eigenbasis) $f_1\equiv1,f_2,\ldots,f_m$ and ordered [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $1=\lambda_1>\lambda_2\geq\cdots\geq\lambda_m$.

Adding a constant changes neither the [variance](../../../variance.md) nor the [Dirichlet form of a Markov chain](../../../markov-process.md#dirichlet-form-of-a-markov-chain). Expand the centered function as $f-\pi(f)=\sum_{j\geq2}a_jf_j$. Then

$$
\operatorname{Var}_\pi(f)=\sum_{j\geq2}a_j^2,\qquad
\mathcal E(f,f)=\sum_{j\geq2}(1-\lambda_j)a_j^2.
$$

For every nonconstant $f$ the quotient is at least $1-\lambda_2$, and equality is attained at $f=f_2$. This proves

$$
\boxed{\gamma=1-\lambda_2=\min_{\operatorname{Var}_\pi(f)>0}\frac{\mathcal E(f,f)}{\operatorname{Var}_\pi(f)}.}
$$

Equivalently minimize the [Dirichlet form of a Markov chain](../../../markov-process.md#dirichlet-form-of-a-markov-chain) over centered unit-norm functions. This is the variational characterization underlying the [Poincare inequality for a reversible Markov chain](../../../markov-process.md#poincare-inequality-for-a-reversible-markov-chain), and does not require the [transition matrix](../../../markov-process.md#stochastic-matrix) to have nonnegative [eigenvalues](../../../linear-operator-theory.md#eigenvalue). For a one-state chain there is no nonconstant test function; the displayed minimization concerns $m\geq2$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The [symmetric group](../../../finite-group-theory.md#symmetric-group) has $n!$ elements, not the printed order $n$. For $n\geq2$ the identity and the $n-1$ adjacent [transpositions](../../../combinatorics.md#transposition-permutation) have probabilities $1/n$, so the specified [transition matrix](../../../markov-process.md#stochastic-matrix) is normalized. Its [stationary distribution](../../../markov-process.md#stationary-distribution) is uniform and it satisfies [detailed balance](../../../markov-process.md#detailed-balance), since each [transposition](../../../combinatorics.md#transposition-permutation) is its own inverse. Adjacent [transpositions](../../../combinatorics.md#transposition-permutation) generate the [symmetric group](../../../finite-group-theory.md#symmetric-group), making this an [irreducible Markov chain](../../../markov-process.md#irreducible-markov-chain); the positive holding probability makes it an [aperiodic Markov chain](../../../markov-process.md#aperiodic-markov-chain).

For a fixed label $i$, right multiplication swaps positions, so $f(\sigma)=\sigma^{-1}(i)$ is the label's position. Under the [uniform distribution on a finite set](../../../discrete-probability-distribution.md#discrete-uniform-distribution) it is uniform on $\{1,\ldots,n\}$. Therefore

$$
\pi(f)=\frac{n+1}{2},\qquad\operatorname{Var}_\pi(f)=\frac{n^2-1}{12}.
$$

For each generator $s_j=(j,j+1)$, the squared change $[f(\sigma s_j)-f(\sigma)]^2$ is one if the label occupies either of the two positions, and zero otherwise. Its stationary [expected value](../../../probability-theory.md#expected-value) is $2/n$, giving

$$
\mathcal E(f,f)=\frac12\sum_{j=1}^{n-1}\frac1n\frac2n=\frac{n-1}{n^2}.
$$

Thus the [tagged-label Rayleigh quotient for adjacent transpositions](../../../markov-process.md#tagged-label-rayleigh-quotient-for-adjacent-transpositions) gives the corrected bound

$$
\boxed{\gamma\leq\frac{12}{n^2(n+1)}=\frac{12}{n^3}(1+o(1)).}
$$

The printed factor six cannot be obtained: the hint's [variance of a uniform distribution](../../../probability-theory.md#variance-of-a-uniform-distribution) is wrong. Directly, $\operatorname{Var}(U)=\int_0^1u^2\,du-(\int_0^1u\,du)^2=1/12$. Bounded [convergence in distribution](../../../convergence-of-random-variables.md#convergence-in-distribution) of $U_n$ does imply convergence of its first two moments, hence convergence of its [variance](../../../variance.md), but the limit is $1/12$.

More strongly, the claimed asymptotic bound itself is false for this kernel. The [Aldous spectral gap theorem](../../../markov-process.md#aldous-spectral-gap-theorem) states that the [interchange process](../../../markov-process.md#interchange-process) on a finite connected weighted [graph](../../../graph.md) has the same [spectral gap](../../../linear-operator-theory.md#spectral-gap) as the single-label [random walk](../../../markov-process.md#random-walk) with identical edge rates; see [Theorem 1.1 and its proof](https://arxiv.org/abs/0906.1238). Here $P-I$ is that [interchange process](../../../markov-process.md#interchange-process) generator on a [path graph](../../../graph-theory.md#path-graph) with edge rates $1/n$. For the tagged-label generator, direct substitution of $g_\ell(k)=\cos(\ell\pi(k-1/2)/n)$ gives [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $-2(1-\cos(\ell\pi/n))/n$, $0\leq\ell<n$, including the reflecting endpoint equations. These $n$ distinct [eigenvalues](../../../linear-operator-theory.md#eigenvalue) exhaust the tagged-label function space. Consequently the theorem yields

$$
\boxed{\gamma=\frac2n\left(1-\cos\frac\pi n\right)\sim\frac{\pi^2}{n^3},}
$$

which exceeds $6/n^3$ asymptotically. This use of a substantial external theorem is only to certify the printed claim's failure; the corrected factor-twelve upper bound above follows directly from the requested test function and the variational formula.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The reference kernel printed in the hint has total mass $1/n+\binom n2/\binom n2=1+1/n$, so it is not a [Markov kernel](../../../markov-process.md#markov-kernel). We explicitly replace it by the normalized [random transposition shuffle](../../../markov-process.md#random-transposition-shuffle): choose two positions independently and uniformly and swap them. Its probabilities are

$$
\widetilde p(\mathrm{id})=1/n,\qquad\widetilde p((i,j))=2/n^2\quad(i<j).
$$

These sum to one, and its ordinary [spectral gap](../../../linear-operator-theory.md#spectral-gap) is $\widetilde\gamma=2/n$, the value intended in the hint. This value can also be certified by the [Aldous spectral gap theorem](../../../markov-process.md#aldous-spectral-gap-theorem): the single-label generator has rate $2/n^2$ between distinct positions, so on centered functions it acts as multiplication by $-2/n$. Both shuffles have the same [uniform distribution on a finite set](../../../discrete-probability-distribution.md#discrete-uniform-distribution) as [stationary distribution](../../../markov-process.md#stationary-distribution).

We use the [Canonical paths comparison theorem](../../../markov-process.md#canonical-paths-comparison-theorem) in the following precise form. For two finite [reversible Markov chains](../../../markov-process.md#reversible-markov-chain) with the same positive [stationary distribution](../../../markov-process.md#stationary-distribution) $\pi$, route each directed transition $(x,y)$ of $\widetilde P$ along a positive-capacity [path](../../../geometry-and-topology.md#continuous-path) $\eta_{xy}$ of $P$. If

$$
A=\max_{e:Q(e)>0}\frac1{Q(e)}\sum_{x,y}\pi(x)\widetilde P(x,y)|\eta_{xy}|N_e(\eta_{xy}),\qquad Q(u,v)=\pi(u)P(u,v),
$$

then $\widetilde{\mathcal E}(f,f)\leq A\mathcal E(f,f)$ and $\gamma\geq\widetilde\gamma/A$. Indeed, telescope each difference along its [path](../../../geometry-and-topology.md#continuous-path), apply the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality), and sum with weights $\pi(x)\widetilde P(x,y)/2$. The load definition gives the [Dirichlet form of a Markov chain](../../../markov-process.md#dirichlet-form-of-a-markov-chain) inequality; the common [variance](../../../variance.md) denominator then gives the [spectral gap](../../../linear-operator-theory.md#spectral-gap) inequality. Identity transitions use empty [paths](../../../geometry-and-topology.md#continuous-path).

Put $s_k=(k,k+1)$. A [transposition](../../../combinatorics.md#transposition-permutation) $(i,j)$ is routed using the word

$$
s_i s_{i+1}\cdots s_{j-1}s_{j-2}\cdots s_i,
$$

of length $L_{ij}=2(j-i)-1\leq2n$. Each generator occurs at most twice; write its occurrence count as $N_k(i,j)\leq2$. For a fixed directed adjacent edge $(\sigma,\sigma s_k)$ and each occurrence of $s_k$ in a word, there is exactly one starting permutation whose translated word crosses this edge at that occurrence. This follows because right multiplication by the prefix is a [bijection](../../../function.md#bijection) of the [symmetric group](../../../finite-group-theory.md#symmetric-group). Hence the uniform stationary factors cancel in the comparison load, leaving

$$
A=\max_k\frac2n\sum_{i<j}L_{ij}N_k(i,j).
$$

The crude bounds $L_{ij}\leq2n$, $N_k(i,j)\leq2$, and $\binom n2\leq n^2/2$ imply $A\leq4n^2$. Therefore

$$
\boxed{\gamma\geq\frac{2/n}{4n^2}=\frac1{2n^3}.}
$$

Only pairs with $i\leq k<j$ contribute, and there are $k(n-k)\leq n^2/4$ of these. Keeping this restriction gives the stronger $A\leq2n^2$ and $\gamma\geq1/n^3$. Neither comparison bound needs the exact adjacent-shuffle [spectral gap](../../../linear-operator-theory.md#spectral-gap); the normalization repair of the reference kernel is essential.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
