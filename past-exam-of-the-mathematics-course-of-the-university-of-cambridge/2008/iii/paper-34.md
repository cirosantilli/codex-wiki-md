# Paper 34

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper34.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper34.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
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
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A [sigma-algebra](../../../measure-theory.md#sigma-algebra) on $\Omega$ is a collection $\mathcal G\subseteq\mathcal P(\Omega)$ containing $\Omega$, closed under [complements](../../../set.md#complement-of-a-set) relative to $\Omega$, and closed under [countable unions](../../../set.md#countable-union). These properties also give closure under [countable intersections](../../../set.md#countable-intersection) by [De Morgan laws](../../../computer-science.md#de-morgan-s-laws).

Let $\mathcal G=\bigcap_{r\in R}\mathcal F_r$. Every constituent [sigma-algebra](../../../measure-theory.md#sigma-algebra) contains $\Omega$, so $\Omega\in\mathcal G$. If $A\in\mathcal G$, its [complement](../../../set.md#complement-of-a-set) belongs to every $\mathcal F_r$, hence to $\mathcal G$. Likewise, if $A_j\in\mathcal G$ for all $j$, then $\bigcup_j A_j$ belongs to every $\mathcal F_r$. Thus $\mathcal G$ is a [sigma-algebra](../../../measure-theory.md#sigma-algebra). For an empty indexing set, the usual [intersection](../../../set.md#set-intersection) convention gives $\mathcal G=\mathcal P(\Omega)$, which is also a [sigma-algebra](../../../measure-theory.md#sigma-algebra).

A [union](../../../set.md#set-union) need not work. On $\Omega=\{1,2,3\}$ take

$$
\mathcal F_1=\{\varnothing,\Omega,\{1\},\{2,3\}\},\qquad
\mathcal F_2=\{\varnothing,\Omega,\{2\},\{1,3\}\}.
$$

Their [union](../../../set.md#set-union) contains $\{1\}$ and $\{2\}$ but not $\{1,2\}$, so it is not a [sigma-algebra](../../../measure-theory.md#sigma-algebra). Put $\mathcal A=\bigcup_r\mathcal F_r$ and let $\mathfrak C$ be the collection of all [sigma-algebras](../../../measure-theory.md#sigma-algebra) on $\Omega$ containing $\mathcal A$. This collection is nonempty because it contains the [power set](../../../set.md#power-set) $\mathcal P(\Omega)$. By the preceding [intersection](../../../set.md#set-intersection) argument,

$$
\boxed{\sigma(\mathcal A)=\bigcap_{\mathcal H\in\mathfrak C}\mathcal H}
$$

is a [sigma-algebra](../../../measure-theory.md#sigma-algebra) containing every $\mathcal F_r$, and it is contained in every other such [sigma-algebra](../../../measure-theory.md#sigma-algebra). This proves existence and minimality.

For the [independent random variables](../../../random-variable.md#independent-random-variables), define the [tail sigma-algebra](../../../probability-theory.md#tail-sigma-algebra) by

$$
\mathcal T=\bigcap_{m\geq1}\sigma(X_m,X_{m+1},\ldots).
$$

Fix a [tail event](../../../probability-theory.md#tail-event) $A\in\mathcal T$. For each $m$, it belongs to $\sigma(X_{m+1},X_{m+2},\ldots)$, which is [independent](../../../random-variable.md#independent-random-variables) of $\mathcal H_m=\sigma(X_1,\ldots,X_m)$. To justify independence of the generated [sigma-algebras](../../../measure-theory.md#sigma-algebra), first use independence of finite collections on cylinder [events](../../../probability-theory.md#event), then extend twice by the [pi-lambda theorem](../../../probability-theory.md#pi-lambda-theorem). In particular, $\mathbb P(A\cap C)=\mathbb P(A)\mathbb P(C)$ for every $C\in\mathcal H_m$ and every $m$.

The increasing [union](../../../set.md#set-union) $\bigcup_m\mathcal H_m$ is an [algebra of sets](../../../measure-theory.md#algebra-of-sets) generating $\mathcal H=\sigma(X_1,X_2,\ldots)$. The collection of $C\in\mathcal H$ satisfying this factorization is a [Dynkin system](../../../measure-theory.md#dynkin-system): it contains $\Omega$, is closed under [complements](../../../set.md#complement-of-a-set), and under countable disjoint [unions](../../../set.md#set-union). The [pi-lambda theorem](../../../probability-theory.md#pi-lambda-theorem) therefore extends the factorization to all $C\in\mathcal H$. Since $A\in\mathcal H$, taking $C=A$ gives $\mathbb P(A)=\mathbb P(A)^2$. Consequently,

$$
\boxed{\mathbb P(A)\in\{0,1\}\qquad(A\in\mathcal T).}
$$

This is the [Kolmogorov zero-one law](../../../probability-theory.md#kolmogorov-s-zero-one-law), proved here directly.

For each fixed $m$, write $S_n=S_{m-1}+\sum_{j=m}^nX_j$ for $n\geq m$, with $S_0=0$. The [random variable](../../../random-variable.md) $S_{m-1}$ is finite, so $S_{m-1}/\sqrt n\to0$. Adding a real sequence tending to zero changes neither the extended-real [limit inferior](../../../real-analysis.md#limit-inferior) nor the extended-real [limit superior](../../../real-analysis.md#limit-superior). Hence

$$
\liminf_n\frac{S_n}{\sqrt n}=\liminf_n\frac{\sum_{j=m}^nX_j}{\sqrt n},\qquad
\limsup_n\frac{S_n}{\sqrt n}=\limsup_n\frac{\sum_{j=m}^nX_j}{\sqrt n}.
$$

The quantities on the right are measurable with respect to $\sigma(X_m,X_{m+1},\ldots)$: write the [limit inferior](../../../real-analysis.md#limit-inferior) as $\sup_N\inf_{n\geq N}$ and the [limit superior](../../../real-analysis.md#limit-superior) as $\inf_N\sup_{n\geq N}$, using countable operations on [measurable functions](../../../measure-theory.md#measurable-function). Therefore both threshold [events](../../../probability-theory.md#event) belong to every such [sigma-algebra](../../../measure-theory.md#sigma-algebra), and hence are [tail events](../../../probability-theory.md#tail-event), for every real threshold, including when either limit is infinite.

**The final recurrence claim is false under the printed hypotheses.** For $c>0$, let $\varepsilon_j$ be independent signs with equal probabilities for $+1$ and $-1$, and set $X_j=c4^{-(j-1)}\varepsilon_j$. These [random variables](../../../random-variable.md) are independent, have [symmetric distributions](../../../probability-theory.md#symmetric-distribution), and obey $|X_j|\leq c$. Nevertheless, the [geometric series](../../../real-analysis.md#geometric-series) gives, on every sample path,

$$
|S_n|\geq c-\sum_{j=2}^n c4^{-(j-1)}\geq c-\frac c3=\frac{2c}{3}>\frac c2.
$$

Thus the proposed repeated-return [event](../../../probability-theory.md#event) has [probability](../../../probability-theory.md#probability) zero, even though none of the increments is degenerate. The [Kolmogorov zero-one law](../../../probability-theory.md#kolmogorov-s-zero-one-law) does not determine which of zero and one occurs.

An additional identical-distribution hypothesis makes the intended conclusion true. Here is a full proof of that qualified version, using the [oscillation of a bounded centered iid random walk](../../../stochastic-process.md#oscillation-of-a-bounded-centered-iid-random-walk). Symmetry and integrability give $\mathbb E X_j=0$, so $S_n$ is a [martingale](../../../martingale.md) for its [natural filtration](../../../stochastic-process.md#natural-filtration). If the common [probability distribution](../../../probability-theory.md#probability-distribution) is concentrated at zero, every $S_n$ is zero and the conclusion is immediate. Otherwise choose $\delta>0$ with $\mathbb P(|X_1|>\delta)>0$. The [Borel-Cantelli lemmas](../../../probability-theory.md#borel-cantelli-lemmas) then give $|X_n|>\delta$ infinitely often [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence); thus $S_n$ cannot converge to a finite limit.

For $a>0$, let $T_a=\inf\{n:S_n\geq a\}$. Before $T_a$ the sum is below $a$, and at $T_a$ it is at most $a+c$. The [stopped martingale](../../../martingale.md#stopped-martingale) $a+c-S_{n\wedge T_a}$ is therefore nonnegative. A stopped integrable [martingale](../../../martingale.md) remains a [martingale](../../../martingale.md) at these bounded times, and a nonnegative [martingale](../../../martingale.md) converges finitely [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) by the [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem). On $\{T_a=\infty\}$ this would force $S_n$ to converge finitely, which has just been ruled out. Hence $T_a<\infty$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Apply the same argument to $-S_n$ and take a countable intersection over positive integer $a$. It follows that

$$
\limsup_n S_n=+\infty,\qquad \liminf_n S_n=-\infty\quad\text{almost surely}.
$$

There are therefore arbitrarily late passages from above $c/2$ to below $-c/2$. A path with [bounded increments](../../../stochastic-process.md#bounded-increments) of magnitude at most $c$ cannot make such a passage without visiting $[-c/2,c/2]$: jumping directly between its two open complementary half-lines would require an increment larger than $c$. There are infinitely many such visits. Thus **with the added identical-distribution hypothesis**, the intended answer is

$$
\boxed{\mathbb P\bigl(|S_n|\leq c/2\text{ infinitely often}\bigr)=1.}
$$

## 2

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For [events](../../../probability-theory.md#event) $A_n$, define their [limit superior](../../../real-analysis.md#limit-superior) by

$$
A_\infty=\limsup_n A_n=\bigcap_{N\geq1}\bigcup_{n\geq N}A_n.
$$

It is the [event](../../../probability-theory.md#event) that infinitely many $A_n$ occur. The two [Borel-Cantelli lemmas](../../../probability-theory.md#borel-cantelli-lemmas) are as follows: if $\sum_n\mathbb P(A_n)<\infty$, then $\mathbb P(A_\infty)=0$, without any independence assumption; if the $A_n$ are independent and $\sum_n\mathbb P(A_n)=\infty$, then $\mathbb P(A_\infty)=1$.

For the first assertion, the [union bound](../../../probability-inequality.md#boole-s-inequality) gives, for every $N$,

$$
\mathbb P(A_\infty)\leq\mathbb P\!\left(\bigcup_{n\geq N}A_n\right)
\leq\sum_{n\geq N}\mathbb P(A_n).
$$

The tail of a convergent nonnegative [series](../../../real-analysis.md#series-mathematics) tends to zero, proving the first [Borel-Cantelli lemma](../../../probability-theory.md#borel-cantelli-lemmas).

For the second assertion, independence and $1-u\leq e^{-u}$ for $0\leq u\leq1$ give

$$
\mathbb P\!\left(\bigcap_{n=N}^K A_n^c\right)
=\prod_{n=N}^K(1-\mathbb P(A_n))
\leq\exp\!\left(-\sum_{n=N}^K\mathbb P(A_n)\right)\longrightarrow0.
$$

By [continuity of probability](../../../probability-theory.md#continuity-of-probability), $\mathbb P(\bigcap_{n\geq N}A_n^c)=0$. The [event](../../../probability-theory.md#event) that only finitely many $A_n$ occur is the countable [union](../../../set.md#set-union) of these zero-probability [events](../../../probability-theory.md#event) over $N$. Its [probability](../../../probability-theory.md#probability) is zero. This proves the second [Borel-Cantelli lemma](../../../probability-theory.md#borel-cantelli-lemmas), and hence both requested assertions:

$$
\boxed{\sum_n\mathbb P(A_n)<\infty\Rightarrow\mathbb P(A_\infty)=0,\qquad
\text{independence and }\sum_n\mathbb P(A_n)=\infty\Rightarrow\mathbb P(A_\infty)=1.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Write $Q(x)=1-\Phi(x)=\int_x^\infty\phi(t)\,dt$, where $\phi(t)=(2\pi)^{-1/2}e^{-t^2/2}$ is the [standard normal density](../../../probability-theory.md#standard-normal-density). For $x>0$, $\phi'(t)=-t\phi(t)$ and [integration by parts](../../../calculus.md#integration-by-parts) yield

$$
Q(x)=\int_x^\infty\frac{-\phi'(t)}t\,dt
=\frac{\phi(x)}x-\int_x^\infty\frac{\phi(t)}{t^2}\,dt.
$$

The boundary term at infinity vanishes. The remainder is nonnegative and is at most $Q(x)/x^2$, so

$$
\frac{x\phi(x)}{x^2+1}\leq Q(x)\leq\frac{\phi(x)}x.
$$

Dividing by the positive quantity $\phi(x)/x$ gives lower and upper bounds $x^2/(x^2+1)$ and $1$. The [squeeze theorem](../../../calculus.md#squeeze-theorem) proves the [Mills ratio](../../../probability-theory.md#mills-ratio) asymptotic

$$
\boxed{1-\Phi(x)\sim\frac{\phi(x)}x\qquad(x\to\infty).}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For $a>0$ and $n\geq2$, let $A_n(a)=\{X_n^2>a\log n\}$. Symmetry of the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution) and the [Mills ratio](../../../probability-theory.md#mills-ratio) asymptotic just proved give

$$
\mathbb P(A_n(a))=2\bigl[1-\Phi(\sqrt{a\log n})\bigr]
\sim\sqrt{\frac{2}{\pi a}}\frac{n^{-a/2}}{\sqrt{\log n}}.
$$

For $a>2$ the [series](../../../real-analysis.md#series-mathematics) of these [probabilities](../../../probability-theory.md#probability) converges, since its terms are eventually bounded by a constant times the convergent [p-series](../../../real-analysis.md#p-series) $n^{-a/2}$. For $0<a<2$ it diverges: choose $r$ strictly between $a/2$ and one, and use $(\log n)^{-1/2}\geq n^{-(r-a/2)}$ for sufficiently large $n$, reducing to the divergent [p-series](../../../real-analysis.md#p-series) $n^{-r}$. At $a=2$ it still diverges, as the [integral test](../../../real-analysis.md#integral-test-for-convergence) gives

$$
\int_2^R\frac{dt}{t\sqrt{\log t}}
=2\bigl(\sqrt{\log R}-\sqrt{\log2}\bigr)\longrightarrow\infty.
$$

For $a>2$, the first [Borel-Cantelli lemma](../../../probability-theory.md#borel-cantelli-lemmas) makes $A_n(a)$ occur only finitely often. For $0<a\leq2$, independence of the [random variables](../../../random-variable.md) makes the [events](../../../probability-theory.md#event) $A_n(a)$ independent, so the second [Borel-Cantelli lemma](../../../probability-theory.md#borel-cantelli-lemmas) makes them occur infinitely often [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Apply these conclusions simultaneously at $a=2+1/k$ for positive integers $k$, and at $a=2$. On the resulting [probability](../../../probability-theory.md#probability)-one [event](../../../probability-theory.md#event), the [limit superior](../../../real-analysis.md#limit-superior) is at most every $2+1/k$ and at least two. Therefore the [Gaussian sample limsup at logarithmic scale](../../../probability-theory.md#gaussian-sample-limsup-at-logarithmic-scale) is

$$
\boxed{\limsup_{n\to\infty}\frac{X_n^2}{\log n}=2\quad\text{almost surely}.}
$$

## 3

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The real [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space) on a [probability space](../../../probability-theory.md#probability-space) consists of equivalence classes of [measurable functions](../../../measure-theory.md#measurable-function) $X:\Omega\to\mathbb R$ satisfying $\mathbb E[X^2]<\infty$, where two [random variables](../../../random-variable.md) represent the same element if they are equal [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Its [norm](../../../functional-analysis.md#norm) is

$$
\|X\|_2=(\mathbb E[X^2])^{1/2}.
$$

Passing to equivalence classes makes this a genuine [norm](../../../functional-analysis.md#norm): $\|X\|_2=0$ exactly when $X=0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). The [Minkowski inequality](../../../real-analysis.md#minkowski-inequality) gives the [triangle inequality](../../../topological-analysis.md#triangle-inequality).

Let $(X_n)$ be a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) in this [norm](../../../functional-analysis.md#norm). Choose an increasing sequence of indices $n_k$ such that

$$
\|X_{n_{k+1}}-X_{n_k}\|_2\leq2^{-k}\qquad(k\geq1).
$$

This is possible by choosing $n_k$ beyond a Cauchy threshold for tolerance $2^{-k}$. Set $D_k=X_{n_{k+1}}-X_{n_k}$. The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) on a [probability space](../../../probability-theory.md#probability-space) gives $\mathbb E|D_k|\leq\|D_k\|_2$. By [Tonelli theorem](../../../measure-theory.md#tonelli-theorem),

$$
\mathbb E\!\left[\sum_{k\geq1}|D_k|\right]
=\sum_{k\geq1}\mathbb E|D_k|\leq\sum_{k\geq1}2^{-k}<\infty.
$$

Thus the [series](../../../real-analysis.md#series-mathematics) of absolute differences is finite [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Define $X=X_{n_1}+\sum_{k\geq1}D_k$ on this [probability](../../../probability-theory.md#probability)-one [event](../../../probability-theory.md#event), and give it the value zero on its complement. It is a [measurable function](../../../measure-theory.md#measurable-function), and $X_{n_k}\to X$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence).

For $l>k$, the [Minkowski inequality](../../../real-analysis.md#minkowski-inequality) gives

$$
\|X_{n_l}-X_{n_k}\|_2\leq\sum_{j=k}^{l-1}2^{-j}.
$$

Apply the [Fatou lemma](../../../measure-theory.md#fatou-s-lemma) to the squared difference as $l\to\infty$. It follows that

$$
\|X-X_{n_k}\|_2\leq\sum_{j=k}^\infty2^{-j}=2^{1-k}.
$$

In particular $X-X_{n_1}\in L^2$, and therefore $X\in L^2$ by the [Minkowski inequality](../../../real-analysis.md#minkowski-inequality). This proves [convergence in L2](../../../convergence-of-random-variables.md#convergence-in-l2) of the subsequence. To recover the entire sequence, for a prescribed $\varepsilon>0$ choose a Cauchy threshold $N$ for $\varepsilon/2$, then choose $k$ with $n_k\geq N$ and $\|X-X_{n_k}\|_2<\varepsilon/2$. For every $n\geq N$,

$$
\|X_n-X\|_2\leq\|X_n-X_{n_k}\|_2+\|X_{n_k}-X\|_2<\varepsilon.
$$

Hence $\boxed{X_n\to X\text{ in }L^2}$, proving [completeness of Lp spaces](../../../measure-theory.md#completeness-of-lp-spaces) for $p=2$ without assuming the desired completeness in the argument.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

A [filtration](../../../stochastic-process.md#filtration-probability-theory) $(\mathcal F_n)_{n\geq0}$ on a [probability space](../../../probability-theory.md#probability-space) is an increasing sequence of [sigma-algebras](../../../measure-theory.md#sigma-algebra) contained in $\mathcal F$: $\mathcal F_n\subseteq\mathcal F_{n+1}$. A real [stochastic process](../../../stochastic-process.md) $(X_n)$ is a [martingale](../../../martingale.md) for this [filtration](../../../stochastic-process.md#filtration-probability-theory) if $X_n$ is $\mathcal F_n$-measurable, $\mathbb E|X_n|<\infty$, and

$$
\boxed{\mathbb E[X_{n+1}\mid\mathcal F_n]=X_n\quad\text{almost surely for every }n.}
$$

The first condition is [adaptedness](../../../stochastic-process.md#adapted-process); the [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation) then gives $\mathbb E[X_n\mid\mathcal F_m]=X_m$ whenever $m\leq n$.

The almost-sure [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem) states that if a real [martingale](../../../martingale.md) satisfies $\sup_n\mathbb E|X_n|<\infty$, then some integrable [random variable](../../../random-variable.md) $X_\infty$ satisfies $X_n\to X_\infty$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). The more general [almost sure submartingale convergence theorem](../../../martingale.md#almost-sure-submartingale-convergence-theorem) needs only $\sup_n\mathbb E[X_n^+]<\infty$ for a [submartingale](../../../martingale.md#submartingale). In particular, a nonnegative [martingale](../../../martingale.md) converges to a finite integrable limit [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), because its [expected value](../../../probability-theory.md#expected-value) is constant. Mere boundedness in the [L1 norm](../../../functional-analysis.md#l1-norm) does not imply [convergence in L1](../../../convergence-of-random-variables.md#convergence-in-l1). The stronger [uniformly integrable martingale convergence theorem](../../../martingale.md#uniformly-integrable-martingale-convergence-theorem) gives both almost-sure convergence and [convergence in L1](../../../convergence-of-random-variables.md#convergence-in-l1) when the [martingale](../../../martingale.md) is [uniformly integrable](../../../convergence-of-random-variables.md#uniform-integrability).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [martingale](../../../martingale.md) property gives $\mathbb E[X_n\mid\mathcal F_m]=X_m$. Both $X_m$ and $X_n$ are [square-integrable](../../../measure-theory.md#square-integrable-function), so their product is integrable by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). Using the $\mathcal F_m$-measurability of $X_m$ in [conditional expectation](../../../measure-theory.md#conditional-expectation) gives

$$
\mathbb E[X_nX_m]=\mathbb E\!\left[X_m\mathbb E[X_n\mid\mathcal F_m]\right]=\mathbb E[X_m^2].
$$

The pull-out step for the possibly unbounded $X_m$ can be justified by first truncating it, then passing to the limit in the [L2 norm](../../../real-analysis.md#l2-norm) and using the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). Expanding the square now yields

$$
\boxed{\mathbb E[(X_n-X_m)^2]=\mathbb E[X_n^2]-\mathbb E[X_m^2]\qquad(m\leq n).}
$$

The left side is nonnegative. Thus $a_n=\mathbb E[X_n^2]$ is nondecreasing and bounded above by $M$, and so $a_n\to a\leq M$. For $m\leq n$,

$$
\|X_n-X_m\|_2^2=a_n-a_m\leq a-a_m\longrightarrow0.
$$

By symmetry of the [norm](../../../functional-analysis.md#norm) difference this proves that $(X_n)$ is a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) in the [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space). The completeness established in part (a) gives an $X_\infty\in L^2$ with

$$
\boxed{X_n\longrightarrow X_\infty\text{ in }L^2.}
$$

This is the [L2-bounded martingale convergence theorem](../../../martingale.md#l2-bounded-martingale-convergence-theorem), derived from [martingale-difference orthogonality](../../../martingale.md#martingale-difference-orthogonality) and completeness. The same sequence also converges [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) by part (b), since $\mathbb E|X_n|\leq\sqrt M$; uniqueness of a limit in [probability](../../../probability-theory.md#probability) identifies that limit with this $X_\infty$.

## 4

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Put $S_0=0$ and take $\mathcal F_0$ to be the trivial [sigma-algebra](../../../measure-theory.md#sigma-algebra). Each $S_n$ is measurable with respect to the [natural filtration](../../../stochastic-process.md#natural-filtration) $\mathcal F_n=\sigma(X_1,\ldots,X_n)$, and

$$
\mathbb E|S_n|\leq\sum_{i=1}^n\mathbb E|X_i|<\infty.
$$

Independence of $X_{n+1}$ from $\mathcal F_n$ makes its [conditional expectation](../../../measure-theory.md#conditional-expectation) equal to its [expected value](../../../probability-theory.md#expected-value), which is zero. Hence

$$
\mathbb E[S_{n+1}\mid\mathcal F_n]
=S_n+\mathbb E[X_{n+1}\mid\mathcal F_n]
=S_n+\mathbb E X_{n+1}=S_n.
$$

The measurability, integrability and [conditional expectation](../../../measure-theory.md#conditional-expectation) conditions are all verified, so $\boxed{(S_n)\text{ is a martingale for }(\mathcal F_n).}$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Here $X_1\leq1$, so for every $\tau>0$,

$$
0<e^{\tau X_1}\leq e^\tau,\qquad M(\tau)=\mathbb E e^{\tau X_1}\leq e^\tau<\infty.
$$

The [Jensen inequality](../../../real-analysis.md#jensen-s-inequality) for the strictly convex [exponential function](../../../calculus.md#exponential-function) gives

$$
M(\tau)\geq e^{\tau\mathbb E X_1}=1.
$$

In fact the inequality is strict: $\mathbb P(X_1=1)>0$ and $\mathbb E X_1=0$ exclude a constant [random variable](../../../random-variable.md). In particular, $\boxed{1\leq M(\tau)<\infty}$ as required.

For $Z_n=e^{\tau S_n}/M(\tau)^n$, independence and identical distribution give

$$
\mathbb E e^{\tau S_n}=\prod_{i=1}^n\mathbb E e^{\tau X_i}=M(\tau)^n.
$$

Thus $Z_n$ is positive, integrable with mean one, and adapted to the [natural filtration](../../../stochastic-process.md#natural-filtration). Conditioning on the next increment gives

$$
\mathbb E[Z_{n+1}\mid\mathcal F_n]
=\frac{e^{\tau S_n}}{M(\tau)^{n+1}}\mathbb E[e^{\tau X_{n+1}}\mid\mathcal F_n]
=\frac{e^{\tau S_n}}{M(\tau)^n}=Z_n.
$$

Consequently $\boxed{(Z_n)\text{ is a martingale}.}$ This is the [exponential martingale of a random walk](../../../markov-process.md#exponential-martingale-of-a-random-walk).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The [hitting time](../../../markov-process.md#first-passage-time) $T$ is a [stopping time](../../../martingale.md#stopping-time) for the [natural filtration](../../../stochastic-process.md#natural-filtration), because $\{T\leq n\}=\bigcup_{k\leq n}\{S_k=b\}$. The integer-valued increments are at most one. A path started at zero therefore cannot reach or exceed $b$ without first visiting $b$, so

$$
S_{n\wedge T}\leq b\quad\text{for every }n.
$$

Define $Y_n=b-S_{n\wedge T}$. It is nonnegative and integrable: $|S_{n\wedge T}|\leq\sum_{j\leq n}|X_j|$. Moreover,

$$
S_{(n+1)\wedge T}-S_{n\wedge T}=\mathbf1_{\{T>n\}}X_{n+1}.
$$

The [indicator function](../../../measure-theory.md#indicator-function) is $\mathcal F_n$-measurable, and $X_{n+1}$ is independent of $\mathcal F_n$ with zero [expected value](../../../probability-theory.md#expected-value). Taking [conditional expectation](../../../measure-theory.md#conditional-expectation) therefore proves directly that $(Y_n)$ is a nonnegative [martingale](../../../martingale.md).

The general result used here is that a nonnegative discrete-time [martingale](../../../martingale.md) has a finite almost-sure limit; this is the [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem), since $\mathbb E Y_n=\mathbb E Y_0=b$ bounds its [L1 norm](../../../functional-analysis.md#l1-norm). On $\{T=\infty\}$ it follows that $S_n=b-Y_n$ converges finitely. A convergent sequence of integers is eventually constant, so $X_n=S_n-S_{n-1}$ would eventually be zero on this [event](../../../probability-theory.md#event).

However, the independent [events](../../../probability-theory.md#event) $\{X_n=1\}$ all have the same strictly positive [probability](../../../probability-theory.md#probability). The second [Borel-Cantelli lemma](../../../probability-theory.md#borel-cantelli-lemmas) says that they occur infinitely often [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). This contradicts eventual constancy on any positive-probability subset of $\{T=\infty\}$. Thus

$$
\boxed{\mathbb P(T<\infty)=1.}
$$

Notice that no lower bound on the negative increments was needed.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The [stopped martingale](../../../martingale.md#stopped-martingale) $Z_{n\wedge T}$ is a [martingale](../../../martingale.md). For completeness, the bounded-time stopping rule follows directly from

$$
Z_{(n+1)\wedge T}-Z_{n\wedge T}
=\mathbf1_{\{T>n\}}(Z_{n+1}-Z_n),
$$

whose [conditional expectation](../../../measure-theory.md#conditional-expectation) given $\mathcal F_n$ is zero. Integrability at each fixed $n$ follows by expressing the stopped value as a finite sum of the integrable $Z_j$ restricted to disjoint [events](../../../probability-theory.md#event). Therefore $\mathbb E Z_{n\wedge T}=\mathbb E Z_0=1$.

The crucial bound is deterministic. Since $S_{n\wedge T}\leq b$ and $M(\tau)\geq1$,

$$
0<Z_{n\wedge T}=\frac{e^{\tau S_{n\wedge T}}}{M(\tau)^{n\wedge T}}\leq e^{\tau b}.
$$

A bounded family is [uniformly integrable](../../../convergence-of-random-variables.md#uniform-integrability): for $K>e^{\tau b}$ all its quantities $\mathbb E[|Z_{n\wedge T}|\mathbf1_{\{|Z_{n\wedge T}|>K\}}]$ vanish. Part (c) gives $T<\infty$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), and then $S_T=b$. Hence

$$
Z_{n\wedge T}\longrightarrow e^{\tau b}M(\tau)^{-T}\quad\text{almost surely}.
$$

The general result for passing to expectations is the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem): almost-sure convergence under one integrable bound implies [convergence in L1](../../../convergence-of-random-variables.md#convergence-in-l1) and convergence of expectations. Applying it with the bound $e^{\tau b}$ gives

$$
1=\lim_n\mathbb E Z_{n\wedge T}=e^{\tau b}\mathbb E[M(\tau)^{-T}],
\qquad
\boxed{\mathbb E[M(\tau)^{-T}]=e^{-\tau b}.}
$$

This is the [exponential first-passage transform for an upward skip-free random walk](../../../markov-process.md#exponential-first-passage-transform-for-an-upward-skip-free-random-walk); it avoids an unjustified use of [optional stopping](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) at an unbounded [stopping time](../../../martingale.md#stopping-time).

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

For the [simple symmetric random walk](../../../probability-theory.md#simple-symmetric-random-walk), the [moment-generating function](../../../probability-theory.md#moment-generating-function) is

$$
M(\tau)=\frac{e^\tau+e^{-\tau}}2=\cosh\tau.
$$

For a given $\alpha>0$, choose the unique $\tau>0$ satisfying $\cosh\tau=e^\alpha$. The transform in part (d) becomes $\mathbb E e^{-\alpha T}=e^{-b\tau}$. To express this in terms of $\alpha$, put $r=e^{-\tau}\in(0,1)$. The equation $(r+r^{-1})/2=e^\alpha$ gives $r^2-2e^\alpha r+1=0$. Its smaller root is the one in $(0,1)$, so

$$
\boxed{\mathbb E[e^{-\alpha T}]
=\left(e^\alpha-\sqrt{e^{2\alpha}-1}\right)^b
=\left(\frac{e^{-\alpha}}{1+\sqrt{1-e^{-2\alpha}}}\right)^b.}
$$

The second expression follows by rationalizing the first root. As $\alpha\downarrow0$ the transform tends to one, consistent with the almost-sure finiteness proved in part (c).

## 5

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

A family $(Y_i)_{i\in I}$ of integrable [random variables](../../../random-variable.md) is [uniformly integrable](../../../convergence-of-random-variables.md#uniform-integrability) if

$$
\boxed{\lim_{K\to\infty}\sup_{i\in I}\mathbb E\bigl[|Y_i|\mathbf1_{\{|Y_i|>K\}}\bigr]=0.}
$$

This controls the contributions of large values uniformly over the family, rather than merely bounding its [L1 norms](../../../functional-analysis.md#l1-norm).

Put $X_n=\mathbb E[Z\mid\mathcal F_n]$ and $A_n(K)=\{|X_n|>K\}\in\mathcal F_n$. The [conditional Jensen inequality](../../../measure-theory.md#conditional-jensen-inequality) gives $|X_n|\leq\mathbb E[|Z|\mid\mathcal F_n]$, hence $\mathbb E|X_n|\leq\mathbb E|Z|$. The [Markov inequality](../../../probability-inequality.md#markov-inequality) therefore gives

$$
\mathbb P(A_n(K))\leq\frac{\mathbb E|Z|}{K}.
$$

Using the measurability of $A_n(K)$ in the defining integral identity for [conditional expectation](../../../measure-theory.md#conditional-expectation), for every $R>0$ we get

$$
\begin{aligned}
\mathbb E[|X_n|\mathbf1_{A_n(K)}]
&\leq\mathbb E[|Z|\mathbf1_{A_n(K)}]\\
&\leq\mathbb E[|Z|\mathbf1_{\{|Z|>R\}}]+R\mathbb P(A_n(K))\\
&\leq\mathbb E[|Z|\mathbf1_{\{|Z|>R\}}]+\frac{R\mathbb E|Z|}{K}.
\end{aligned}
$$

The first term tends to zero as $R\to\infty$ because $Z$ is integrable, by the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem). Given $\varepsilon>0$, first choose $R$ to make it less than $\varepsilon/2$, then choose $K$ to make the second term less than $\varepsilon/2$. These choices work for every $n$. This proves [uniform integrability of conditional expectations](../../../convergence-of-random-variables.md#uniform-integrability-of-conditional-expectations):

$$
\boxed{\{\mathbb E[Z\mid\mathcal F_n]:n\geq1\}\text{ is uniformly integrable}.}
$$

In fact the argument works for an arbitrary family of [sigma-algebras](../../../measure-theory.md#sigma-algebra); nesting is not needed for this conclusion.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Values at the endpoint one do not affect any of the conclusions, since $\mathbb P(U=1)=0$. Set $b_n(1)=1$ to define each [random variable](../../../random-variable.md) everywhere, and choose a [Borel measurable function](../../../measure-theory.md#borel-measurable-function) agreeing with $f$ [almost everywhere](../../../measure-theory.md#almost-everywhere) if necessary. These choices leave all integrals and almost-sure assertions unchanged.

Every [dyadic interval](../../../real-analysis.md#dyadic-interval) at level $n+1$ lies in a [dyadic interval](../../../real-analysis.md#dyadic-interval) at level $n$. Equivalently, $b_n(U)$ is a measurable function of $b_{n+1}(U)$, so $\mathcal F_n\subseteq\mathcal F_{n+1}$: these [sigma-algebras](../../../measure-theory.md#sigma-algebra) form a [filtration](../../../stochastic-process.md#filtration-probability-theory). Since the [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) of $U$ gives $\mathbb E|f(U)|=\int_0^1|f(u)|\,du<\infty$, the [conditional expectations](../../../measure-theory.md#conditional-expectation) $X_n=\mathbb E[f(U)\mid\mathcal F_n]$ are integrable and adapted. The [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation) gives

$$
\mathbb E[X_{n+1}\mid\mathcal F_n]
=\mathbb E[\mathbb E[f(U)\mid\mathcal F_{n+1}]\mid\mathcal F_n]
=\mathbb E[f(U)\mid\mathcal F_n]=X_n.
$$

Thus $(X_n)$ is a [martingale](../../../martingale.md), and part (a) proves that it is [uniformly integrable](../../../convergence-of-random-variables.md#uniform-integrability).

For $I_{n,k}=[k2^{-n},(k+1)2^{-n})$, the [event](../../../probability-theory.md#event) $\{U\in I_{n,k}\}$ is an [atom of a sigma-algebra](../../../measure-theory.md#atom-of-a-sigma-algebra) $\mathcal F_n$, with [probability](../../../probability-theory.md#probability) $2^{-n}$. The value of the [conditional expectation](../../../measure-theory.md#conditional-expectation) there is therefore

$$
\frac{\mathbb E[f(U)\mathbf1_{\{U\in I_{n,k}\}}]}{\mathbb P(U\in I_{n,k})}
=2^n\int_{I_{n,k}}f(u)\,du.
$$

Consequently $\boxed{X_n=f_n(U)\text{ almost surely}.}$ This also shows directly that $\int_0^1|f_n|\leq\int_0^1|f|$.

By the [uniformly integrable martingale convergence theorem](../../../martingale.md#uniformly-integrable-martingale-convergence-theorem), there is an integrable $Y$ such that $X_n\to Y$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) and in the [L1 norm](../../../functional-analysis.md#l1-norm). To identify this limit, put $\mathcal F_\infty=\sigma(\bigcup_n\mathcal F_n)$. Since $0\leq U-b_n(U)<2^{-n}$ away from the harmless endpoint, $U=\lim_n b_n(U)$, and $U$ is $\mathcal F_\infty$-measurable. Conversely every $b_n(U)$ is a measurable function of $U$. Thus $\mathcal F_\infty=\sigma(U)$, and both $Y$ and $f(U)$ have $\mathcal F_\infty$-measurable versions.

For $A\in\mathcal F_m$, the defining property of [conditional expectation](../../../measure-theory.md#conditional-expectation) gives $\mathbb E[X_n\mathbf1_A]=\mathbb E[f(U)\mathbf1_A]$ whenever $n\geq m$. Passing to the limit in the [L1 norm](../../../functional-analysis.md#l1-norm) yields

$$
\mathbb E[Y\mathbf1_A]=\mathbb E[f(U)\mathbf1_A].
$$

The increasing [union](../../../set.md#set-union) $\bigcup_m\mathcal F_m$ is an [algebra of sets](../../../measure-theory.md#algebra-of-sets) generating $\mathcal F_\infty$. The class of [events](../../../probability-theory.md#event) for which this integral identity holds is a [Dynkin system](../../../measure-theory.md#dynkin-system), so the [pi-lambda theorem](../../../probability-theory.md#pi-lambda-theorem) extends the identity to every $A\in\mathcal F_\infty$. Since both [random variables](../../../random-variable.md) are measurable there, uniqueness of [conditional expectation](../../../measure-theory.md#conditional-expectation) gives $Y=f(U)$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). We have proved that the [dyadic conditional averages recover integrable functions](../../../measure-theory.md#dyadic-conditional-averages-recover-integrable-functions):

$$
\boxed{f_n(x)\longrightarrow f(x)\quad\text{for Lebesgue-almost every }x\in[0,1],}
$$

because a [probability](../../../probability-theory.md#probability)-one assertion for $U$ is a full-[Lebesgue measure](../../../measure-theory.md#lebesgue-measure) assertion for $x$. Likewise, the [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) of $U$ turns [convergence in L1](../../../convergence-of-random-variables.md#convergence-in-l1) into

$$
\boxed{\int_0^1|f_n(u)-f(u)|\,du
=\mathbb E|X_n-f(U)|\longrightarrow0.}
$$

No pointwise continuity of $f$ is required.

## 6

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

A standard [Brownian motion](../../../brownian-motion.md) is a real [stochastic process](../../../stochastic-process.md) $(B_t)_{t\geq0}$ with $B_0=0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), continuous [sample paths](../../../stochastic-process.md#sample-path) [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), and independent increments such that $B_t-B_s$ has [normal distribution](../../../probability-theory.md#normal-distribution) $N(0,t-s)$ whenever $0\leq s<t$. With its completed, right-continuous [natural filtration](../../../stochastic-process.md#natural-filtration) $(\mathcal F_t)$, its [Strong Markov property](../../../markov-process.md#strong-markov-property) is the following: for every almost-surely finite [stopping time](../../../martingale.md#stopping-time) $T$, the process

$$
W_s=B_{T+s}-B_T,\qquad s\geq0,
$$

is a standard [Brownian motion](../../../brownian-motion.md) independent of $\mathcal F_T$. Here the [stopping-time sigma-algebra](../../../martingale.md#stopping-time-sigma-algebra) is

$$
\mathcal F_T=\{A\in\mathcal F:A\cap\{T\leq t\}\in\mathcal F_t\text{ for all }t\geq0\}.
$$

In particular, for every bounded $\mathcal F_T$-measurable [random variable](../../../random-variable.md) $H$ and bounded Borel functional $G$ on the continuous path space,

$$
\mathbb E\bigl[H\,G((B_{T+s}-B_T)_{s\geq0})\bigr]
=\mathbb E[H]\,\mathbb E\bigl[G((B_s)_{s\geq0})\bigr].
$$

Thus the independence is from the entire stopped past, not only from $B_T$, and is a statement about the whole future path, not just a single increment.

To prove the [Brownian reflection principle](../../../brownian-motion.md#reflection-principle-wiener-process) without assuming that a level is hit in finite time, fix $t>0$, $m>0$, and set $T_m=\inf\{s\geq0:B_s\geq m\}$ and $R=T_m\wedge t$. Continuity of the [sample paths](../../../stochastic-process.md#sample-path) makes $T_m$ a [stopping time](../../../martingale.md#stopping-time) and gives $B_{T_m}=m$ whenever $T_m<\infty$. The [stopping time](../../../martingale.md#stopping-time) $R$ is bounded. Reflect the path after $R$:

$$
\widehat B_s=
\begin{cases}
B_s,&s\leq R,\\
2B_R-B_s,&s>R.
\end{cases}
$$

By the [Strong Markov property](../../../markov-process.md#strong-markov-property), the future increments after $R$ are an independent [Brownian motion](../../../brownian-motion.md). Negating them preserves their [probability distribution](../../../probability-theory.md#probability-distribution), by symmetry of their joint [normal distributions](../../../probability-theory.md#normal-distribution). Hence the reflected process $\widehat B$ has the same path law as $B$.

If $T_m>t$, reflection changes nothing on $[0,t]$ and $\widehat B_t=B_t<m$. If $T_m\leq t$, both paths first hit $m$ at the same time and $\widehat B_t=2m-B_t$. Therefore, for $x\leq m$, the following [events](../../../probability-theory.md#event) agree path by path:

$$
\{M_t\geq m,\ B_t\leq x\}
=\{\widehat B_t\geq2m-x\}.
$$

Indeed, the right-hand endpoint is at least $m$, so the reflected path must have hit $m$ before or at $t$; this also forces the original path to have done so. The reflection relation then makes the endpoint inequality equivalent to $B_t\leq x$. Equality cases at $T_m=t$ satisfy the same relation. Since $\widehat B_t$ and $B_t$ have the same [probability distribution](../../../probability-theory.md#probability-distribution),

$$
\boxed{\mathbb P(M_t\geq m,\ B_t\leq x)
=\mathbb P(B_t\geq2m-x)\qquad(m>0,\ x\leq m).}
$$

For $t=0$, both sides are zero, because $B_0=M_0=0$ and $2m-x\geq m>0$.

For $t>0$, set $x=m$ in this identity. Continuity implies $\{B_t>m\}\subseteq\{M_t\geq m\}$, and the [normal distribution](../../../probability-theory.md#normal-distribution) of $B_t$ has no atom at $m$. Splitting according to whether $B_t\leq m$ gives

$$
\mathbb P(M_t\geq m)=\mathbb P(B_t\geq m)+\mathbb P(B_t>m)
=2\mathbb P(B_t\geq m)=\mathbb P(|B_t|\geq m).
$$

Both [random variables](../../../random-variable.md) are nonnegative. Their tails agree for all $m>0$, which determines their [probability distributions](../../../probability-theory.md#probability-distribution), including the mass at zero. Thus the [Brownian running maximum](../../../brownian-motion.md#brownian-running-maximum) satisfies

$$
\boxed{M_t\overset d=|B_t|\quad(t\geq0).}
$$

For $x>0$ and $t>0$, continuity again gives $\{T_x\leq t\}=\{M_t\geq x\}$. Since $B_t/\sqrt t$ is a [standard normal random variable](../../../probability-theory.md#standard-normal-random-variable), the [distribution function](../../../probability-theory.md#cumulative-distribution-function) of the [Brownian first-passage time](../../../markov-process.md#brownian-first-passage-time) is

$$
F_{T_x}(t)=2\left[1-\Phi\!\left(\frac{x}{\sqrt t}\right)\right].
$$

It tends to one as $t\to\infty$ and to zero as $t\downarrow0$, proving almost-sure finiteness and absence of an atom at zero. For the [standard normal random variable](../../../probability-theory.md#standard-normal-random-variable) $B_1$,

$$
\mathbb P\!\left(\left(\frac{x}{B_1}\right)^2\leq t\right)
=\mathbb P\!\left(|B_1|\geq\frac{x}{\sqrt t}\right)
=2\left[1-\Phi\!\left(\frac{x}{\sqrt t}\right)\right].
$$

The value of this ratio on the zero-probability [event](../../../probability-theory.md#event) $\{B_1=0\}$ may be defined arbitrarily. Matching the [distribution functions](../../../probability-theory.md#cumulative-distribution-function) proves

$$
\boxed{T_x\overset d=\left(\frac{x}{B_1}\right)^2.}
$$

Finally, differentiate the [distribution function](../../../probability-theory.md#cumulative-distribution-function) on $t>0$, using $\Phi'=\phi$ and $\frac{d}{dt}(x/\sqrt t)=-x/(2t^{3/2})$. The [first-passage-time density](../../../markov-process.md#first-passage-time-density) is

$$
\boxed{f_{T_x}(t)=\frac{x}{\sqrt{2\pi}\,t^{3/2}}\exp\!\left(-\frac{x^2}{2t}\right)\quad(t>0),}
$$

and is zero for $t\leq0$. Its integral is one by the endpoint limits of $F_{T_x}$, so no missing mass at an infinite [hitting time](../../../markov-process.md#first-passage-time) is present.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
