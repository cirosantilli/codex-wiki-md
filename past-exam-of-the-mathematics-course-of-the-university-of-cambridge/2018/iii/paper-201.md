# Paper 201

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_201.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_201.pdf)

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
  - [d](#6/d)
    - [Solution](#6/d/solution)

## 1

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a discrete-time [martingale](../../../martingale.md) $(M_n)$ and real $a<b$, let $U_N[a,b]$ be the [upcrossing count](../../../martingale.md#upcrossing-count): buy on the first observation at or below $a$, sell on the next observation at or above $b$, and repeat up to time $N$, counting only completed pairs. Writing $z^-=max(-z,0)$, the [Doob upcrossing inequality](../../../martingale.md#doob-upcrossing-inequality) is

$$
\boxed{(b-a)\mathbb E U_N[a,b]\leq\mathbb E(M_N-a)^-.}
$$

This convention permits the first purchase at time zero. Equivalently, the right side is $\mathbb E(M_N-a)^+-\mathbb E(M_0-a)$, because the [martingale](../../../martingale.md) has constant [expected value](../../../probability-theory.md#expected-value).

For completeness, let $H_k\in\{0,1\}$ indicate whether the trading rule holds one unit during $(k-1,k]$. This is a [predictable process](../../../martingale.md#predictable-process), so the [martingale transform](../../../martingale.md#martingale-transform) $G_N=\sum_{k=1}^NH_k(M_k-M_{k-1})$ has zero [expected value](../../../probability-theory.md#expected-value). Every completed trade gains at least $b-a$, and an unfinished trade loses at most $(M_N-a)^-$. Thus $G_N\geq(b-a)U_N[a,b]-(M_N-a)^-$, giving the inequality.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem) says that if a discrete-time [martingale](../../../martingale.md) $(M_n)$ satisfies $C=\sup_n\mathbb E|M_n|<\infty$, then there is an [integrable random variable](../../../probability-theory.md#integrable-random-variable) $M_\infty$ such that

$$
\boxed{M_n\longrightarrow M_\infty\quad\text{almost surely},\qquad \mathbb E|M_\infty|\leq C.}
$$

The hypothesis does not by itself ensure [convergence in L1](../../../convergence-of-random-variables.md#convergence-in-l1).

For each pair of [rational numbers](../../../number-theory.md#rational-number) $a<b$, the [Doob upcrossing inequality](../../../martingale.md#doob-upcrossing-inequality) gives $\mathbb E U_N[a,b]\leq(C+|a|)/(b-a)$. The [monotone convergence theorem](../../../measure-theory.md#monotone-convergence-theorem) therefore gives a finite [expected value](../../../probability-theory.md#expected-value) for $U_\infty[a,b]=\lim_NU_N[a,b]$, so this [upcrossing count](../../../martingale.md#upcrossing-count) is finite [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). There are only countably many such pairs, hence all their [upcrossing counts](../../../martingale.md#upcrossing-count) are simultaneously finite outside one event of probability zero.

If $\liminf_nM_n<\limsup_nM_n$, the [density of the rational numbers](../../../number-theory.md#density-of-the-rational-numbers) supplies $a<b$ strictly between them, forcing infinitely many [upcrossings](../../../martingale.md#upcrossing). Consequently $M_n$ has a limit in the [extended real numbers](../../../arithmetic.md#extended-real-number-line) [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). By the [Fatou lemma](../../../measure-theory.md#fatou-s-lemma),

$$
\mathbb E\left[\liminf_n|M_n|\right]\leq\liminf_n\mathbb E|M_n|\leq C.
$$

A limit of either $+\infty$ or $-\infty$ would make this lower limit infinite, so the limit is finite [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), and the same inequality proves its [integrability](../../../probability-theory.md#integrable-random-variable).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Set $M_n=\sum_{j=0}^nX_j$ and $\mathcal F_n=\sigma(X_0,\ldots,X_n)$. The [independence](../../../random-variable.md#independent-random-variables) and zero [expected values](../../../probability-theory.md#expected-value) give $\mathbb E[M_{n+1}\mid\mathcal F_n]=M_n$, so $(M_n)$ is a [martingale](../../../martingale.md). The [variance additivity for independent random variables](../../../variance.md#variance-additivity-for-independent-random-variables) gives

$$
\mathbb E[M_n^2]=\sum_{j=0}^n\mathbb E[X_j^2]\leq V:=\sum_{j=0}^\infty\mathbb E[X_j^2]<\infty.
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) implies $\sup_n\mathbb E|M_n|\leq\sqrt V$. Applying the [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem) from (b),

$$
\boxed{\sum_{j=0}^{\infty}X_j\ \text{converges almost surely}.}
$$

In fact the [L2 martingale convergence theorem](../../../martingale.md#l2-martingale-convergence-theorem) also gives [convergence in L2](../../../convergence-of-random-variables.md#convergence-in-l2). Independently, for $n>m$ the same [variance additivity for independent random variables](../../../variance.md#variance-additivity-for-independent-random-variables) yields $\mathbb E|M_n-M_m|^2=\sum_{j=m+1}^n\mathbb E[X_j^2]\to0$, confirming that the partial sums form a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) in $L^2$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Let $\xi_1,\xi_2,\ldots$ be [independent and identically distributed random variables](../../../random-variable.md#independent-and-identically-distributed-random-variables) with the fair [Bernoulli distribution](../../../discrete-probability-distribution.md#bernoulli-distribution), and put

$$
M_0=1,\qquad M_n=2^n\mathbf1_{\{\xi_1=\cdots=\xi_n=1\}}.
$$

Relative to $\mathcal F_n=\sigma(\xi_1,\ldots,\xi_n)$, this [fair-coin doubling martingale](../../../martingale.md#fair-coin-doubling-martingale) satisfies $\mathbb E[M_{n+1}\mid\mathcal F_n]=M_n$: while alive it doubles with probability $1/2$ and becomes zero otherwise. Its [expected value](../../../probability-theory.md#expected-value) is $\mathbb E M_n=2^n2^{-n}=1$.

The probability of an infinite run of ones is $\lim_n2^{-n}=0$, so $M_n$ is eventually zero [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). However,

$$
\boxed{M_n\to0\ \text{almost surely},\qquad \mathbb E|M_n-0|=1\ \text{for every }n.}
$$

Thus the [martingale](../../../martingale.md) lacks [convergence in L1](../../../convergence-of-random-variables.md#convergence-in-l1) to its limit from [almost sure convergence](../../../convergence-of-random-variables.md#almost-sure-convergence). Nor can it have [convergence in L1](../../../convergence-of-random-variables.md#convergence-in-l1) to any other limit: [convergence in L1](../../../convergence-of-random-variables.md#convergence-in-l1) implies [convergence in probability](../../../convergence-of-random-variables.md#convergence-in-probability), whose limit is unique up to [almost sure equality](../../../convergence-of-random-variables.md#almost-sure-equality).

## 2

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A sequence of [integrable random variables](../../../probability-theory.md#integrable-random-variable) $(X_n)$ has [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability) exactly when

$$
\boxed{\lim_{K\to\infty}\sup_{n\geq0}\mathbb E\left[|X_n|\mathbf1_{\{|X_n|>K\}}\right]=0.}
$$

The [uniformly integrable martingale convergence theorem](../../../martingale.md#uniformly-integrable-martingale-convergence-theorem) states that a [uniformly integrable](../../../convergence-of-random-variables.md#uniform-integrability) discrete-time [martingale](../../../martingale.md) $(M_n)$ has an [integrable random variable](../../../probability-theory.md#integrable-random-variable) $M_\infty$ with

$$
\boxed{M_n\to M_\infty\ \text{almost surely and in }L^1,\qquad M_n=\mathbb E[M_\infty\mid\mathcal F_n].}
$$

Indeed, [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability) implies $\sup_n\mathbb E|M_n|<\infty$, so the [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem) gives [almost sure convergence](../../../convergence-of-random-variables.md#almost-sure-convergence). The combination of [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability) and [almost sure convergence](../../../convergence-of-random-variables.md#almost-sure-convergence) gives [convergence in L1](../../../convergence-of-random-variables.md#convergence-in-l1). For $m\geq n$, the [martingale](../../../martingale.md) identity $\mathbb E[M_m\mid\mathcal F_n]=M_n$ passes to the limit by the [L1 contraction of conditional expectation](../../../measure-theory.md#l1-contraction-of-conditional-expectation).

Conversely, [uniform integrability of conditional expectations](../../../convergence-of-random-variables.md#uniform-integrability-of-conditional-expectations) shows that a [martingale](../../../martingale.md) of the form $M_n=\mathbb E[Y\mid\mathcal F_n]$ for one [integrable random variable](../../../probability-theory.md#integrable-random-variable) $Y$ is [uniformly integrable](../../../convergence-of-random-variables.md#uniform-integrability).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The original PDF has $\mathbb E|X_T|<\infty$ and $\mathbb E[|X_n|\mathbf1_{\{T>n\}}]\to0$. The TeX transcription drops the [expected value](../../../probability-theory.md#expected-value) and absolute value in the first condition, and the absolute value in the second. The proof uses the PDF's conditions.

Because the [stopping time](../../../martingale.md#stopping-time) $T$ is finite [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), $X_{n\wedge T}\to X_T$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). More strongly,

$$
\mathbb E|X_{n\wedge T}-X_T|
=\mathbb E\left[|X_n-X_T|\mathbf1_{\{T>n\}}\right]
\leq\mathbb E\left[|X_n|\mathbf1_{\{T>n\}}\right]
+\mathbb E\left[|X_T|\mathbf1_{\{T>n\}}\right]\longrightarrow0.
$$

The first term tends to zero by hypothesis; the second does so by the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem). Thus there is [convergence in L1](../../../convergence-of-random-variables.md#convergence-in-l1).

Here is the needed [L1 convergence implies uniform integrability](../../../convergence-of-random-variables.md#l1-convergence-implies-uniform-integrability) argument. For any [integrable random variables](../../../probability-theory.md#integrable-random-variable) $Z,Y$ and $K>0$, splitting according to $|Y|>K/2$ gives

$$
\mathbb E\left[|Z|\mathbf1_{\{|Z|>K\}}\right]
\leq2\mathbb E|Z-Y|+\mathbb E\left[|Y|\mathbf1_{\{|Y|>K/2\}}\right].
$$

Take $Z=X_{n\wedge T}$ and $Y=X_T$. For large $n$, the first term is uniformly small by [convergence in L1](../../../convergence-of-random-variables.md#convergence-in-l1), and the second is small for large $K$ by [integrability](../../../probability-theory.md#integrable-random-variable). The finitely many remaining $n$ are handled individually by [integrability](../../../probability-theory.md#integrable-random-variable). Hence **the stopped process is [uniformly integrable](../../../convergence-of-random-variables.md#uniform-integrability)**. This proves the [stopped-martingale uniform integrability criterion](../../../martingale.md#stopped-martingale-uniform-integrability-criterion); the [martingale](../../../martingale.md) assumption is not needed for this particular implication.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Pointwise, an integer-valued nonnegative [random variable](../../../random-variable.md) has the representation

$$
T=\sum_{n=0}^{\infty}\mathbf1_{\{T>n\}}:
$$

when $T=k$, exactly the terms $n=0,\ldots,k-1$ equal one. Applying the [Tonelli theorem](../../../measure-theory.md#tonelli-theorem), or the [monotone convergence theorem](../../../measure-theory.md#monotone-convergence-theorem) to the finite sums of [indicator random variables](../../../probability-theory.md#indicator-random-variable), gives the [tail-sum formula for expectation](../../../probability-theory.md#tail-sum-formula-for-expectation)

$$
\boxed{\mathbb ET=\sum_{n=0}^{\infty}\mathbb P(T>n).}
$$

Both sides may be infinite; no [integrability](../../../probability-theory.md#integrable-random-variable) assumption is necessary.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Write $\Delta X_{n+1}=X_{n+1}-X_n$ and $Y=\sum_{n\geq0}|\Delta X_{n+1}|\mathbf1_{\{T>n\}}$. Since $T$ is a [stopping time](../../../martingale.md#stopping-time), $\{T>n\}\in\mathcal F_n$. The [Tonelli theorem](../../../measure-theory.md#tonelli-theorem), [conditional expectation](../../../measure-theory.md#conditional-expectation), and (c)'s [tail-sum formula for expectation](../../../probability-theory.md#tail-sum-formula-for-expectation) yield

$$
\begin{aligned}
\mathbb EY
&=\sum_{n\geq0}\mathbb E\left[\mathbf1_{\{T>n\}}\mathbb E(|\Delta X_{n+1}|\mid\mathcal F_n)\right]\\
&\leq C\sum_{n\geq0}\mathbb P(T>n)=C\mathbb ET<\infty.
\end{aligned}
$$

Thus $Y$ is an [integrable random variable](../../../probability-theory.md#integrable-random-variable). Since $X_0=0$, telescoping gives $|X_T|\leq Y$ and $|X_n|\mathbf1_{\{T>n\}}\leq Y\mathbf1_{\{T>n\}}$. The [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) gives $\mathbb E[|X_n|\mathbf1_{\{T>n\}}]\to0$, so (b) gives [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability) of the [stopped martingale](../../../martingale.md#stopped-martingale).

The [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) at the bounded [stopping time](../../../martingale.md#stopping-time) $n\wedge T$ gives $\mathbb E X_{n\wedge T}=\mathbb E X_0=0$. Passing to the limit using the [convergence in L1](../../../convergence-of-random-variables.md#convergence-in-l1) proved in (b),

$$
\boxed{\mathbb E X_T=\mathbb E X_0=0.}
$$

One can also pass directly by the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem), since $|X_{n\wedge T}|\leq Y$.

## 3

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [tail sigma-algebra](../../../probability-theory.md#tail-sigma-algebra) is

$$
\boxed{\mathcal T=\bigcap_{N\geq1}\sigma(X_N,X_{N+1},\ldots).}
$$

Its [events](../../../probability-theory.md#event) depend only on arbitrarily late coordinates. The [Kolmogorov zero-one law](../../../probability-theory.md#kolmogorov-s-zero-one-law) states that for a sequence of [independent random variables](../../../random-variable.md#independent-random-variables), every [tail event](../../../probability-theory.md#tail-event) has probability zero or one:

$$
\boxed{A\in\mathcal T\ \Longrightarrow\ \mathbb P(A)\in\{0,1\}.}
$$

Identical [probability distributions](../../../probability-theory.md#probability-distribution) and [integrability](../../../probability-theory.md#integrable-random-variable) are not required for the [Kolmogorov zero-one law](../../../probability-theory.md#kolmogorov-s-zero-one-law).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $\mathcal G_n=\sigma(S_n,S_{n+1},\ldots)$. Since $X_{n+j}=S_{n+j}-S_{n+j-1}$,

$$
\mathcal G_n=\sigma(S_n,X_{n+1},X_{n+2},\ldots).
$$

Permuting $X_1,\ldots,X_n$ preserves their [joint probability distribution](../../../probability-theory.md#joint-probability-distribution) and leaves every generator of $\mathcal G_n$ unchanged. Therefore, for each bounded $\mathcal G_n$-measurable $H$,

$$
\mathbb E[X_1H]=\mathbb E[X_jH]\qquad(1\leq j\leq n).
$$

This is the symmetry of [exchangeable random variables](../../../probability-theory.md#exchangeable-random-variables). By the defining identity of [conditional expectation](../../../measure-theory.md#conditional-expectation), all $\mathbb E[X_j\mid\mathcal G_n]$ are equal [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Summing these [conditional expectations](../../../measure-theory.md#conditional-expectation) and using that $S_n$ is $\mathcal G_n$-measurable gives

$$
n\mathbb E[X_1\mid\mathcal G_n]=\mathbb E[S_n\mid\mathcal G_n]=S_n.
$$

Hence the [conditional expectation of a summand given future partial sums](../../../measure-theory.md#conditional-expectation-of-a-summand-given-future-partial-sums) is

$$
\boxed{\mathbb E[X_1\mid S_n,S_{n+1},\ldots]=\frac{S_n}{n}\quad\text{almost surely}.}
$$

The [integrability](../../../probability-theory.md#integrable-random-variable) of each $X_j$ justifies every [conditional expectation](../../../measure-theory.md#conditional-expectation) above.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [sigma-algebras](../../../measure-theory.md#sigma-algebra) $\mathcal G_n=\sigma(S_n,S_{n+1},\ldots)$ decrease with $n$, and (b) gives $S_n/n=\mathbb E[X_1\mid\mathcal G_n]$. The permitted [reverse martingale convergence theorem](../../../martingale.md#reverse-martingale-convergence-theorem) therefore gives an [integrable random variable](../../../probability-theory.md#integrable-random-variable) $L$ such that $S_n/n\to L$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) and with [convergence in L1](../../../convergence-of-random-variables.md#convergence-in-l1). In particular,

$$
\mathbb EL=\lim_n\mathbb E[S_n/n]=m.
$$

It remains to prove that $L$ is constant. We must not assume that $\bigcap_n\mathcal G_n$ is the [tail sigma-algebra](../../../probability-theory.md#tail-sigma-algebra) of the $X_j$; instead use [tail measurability of limits of sample averages](../../../probability-theory.md#tail-measurability-of-limits-of-sample-averages) directly. Define the [random variable](../../../random-variable.md) valued in the [extended real numbers](../../../arithmetic.md#extended-real-number-line) $L^*=\limsup_n S_n/n$. For every fixed $N$,

$$
L^*=\limsup_{n\to\infty}\frac{X_{N+1}+\cdots+X_n}{n},
$$

because $S_N/n\to0$ pointwise. Thus $L^*$ is measurable with respect to $\sigma(X_{N+1},X_{N+2},\ldots)$ for every $N$, and hence to the [tail sigma-algebra](../../../probability-theory.md#tail-sigma-algebra). Also $L^*=L$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence).

By the [Kolmogorov zero-one law](../../../probability-theory.md#kolmogorov-s-zero-one-law), each [tail event](../../../probability-theory.md#tail-event) $\{L^*\leq q\}$, for a [rational number](../../../number-theory.md#rational-number) $q$, has probability zero or one. Since $L^*$ is finite [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), its [distribution function](../../../probability-theory.md#cumulative-distribution-function) can only be that of a constant $c$: taking $c=\inf\{q\in\mathbb Q:\mathbb P(L^*\leq q)=1\}$ and using the [density of the rational numbers](../../../number-theory.md#density-of-the-rational-numbers) gives $L^*=c$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Its [expected value](../../../probability-theory.md#expected-value) identifies $c=m$. This proves the [strong law of large numbers](../../../convergence-of-random-variables.md#strong-law-of-large-numbers):

$$
\boxed{\frac{S_n}{n}\longrightarrow m\quad\text{almost surely}.}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Split the adjacent products into two subsequences:

$$
Y_j=X_{2j-1}X_{2j},\qquad Z_j=X_{2j}X_{2j+1}\qquad(j\geq1).
$$

Within each subsequence the pairs use disjoint coordinates, so each subsequence consists of [independent and identically distributed random variables](../../../random-variable.md#independent-and-identically-distributed-random-variables). The two subsequences need not be [independent](../../../random-variable.md#independent-random-variables) of each other. By [independence](../../../random-variable.md#independent-random-variables) within a pair,

$$
\mathbb E|Y_j|=\mathbb E|Z_j|=(\mathbb E|X_1|)^2<\infty,\qquad
\mathbb E Y_j=\mathbb E Z_j=m^2.
$$

Apply the [strong law of large numbers](../../../convergence-of-random-variables.md#strong-law-of-large-numbers) from (c) separately to obtain $k^{-1}\sum_{j=1}^kY_j\to m^2$ and $k^{-1}\sum_{j=1}^kZ_j\to m^2$ simultaneously [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Since

$$
\frac{\widetilde S_n}{n}
=\frac{\lceil n/2\rceil}{n}\frac{\sum_{j=1}^{\lceil n/2\rceil}Y_j}{\lceil n/2\rceil}
+\frac{\lfloor n/2\rfloor}{n}\frac{\sum_{j=1}^{\lfloor n/2\rfloor}Z_j}{\lfloor n/2\rfloor},
$$

and both prefactors tend to $1/2$, the [strong law for adjacent products](../../../convergence-of-random-variables.md#strong-law-for-adjacent-products) gives

$$
\boxed{\frac{\widetilde S_n}{n}\longrightarrow m^2\quad\text{almost surely}.}
$$

## 4

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A standard one-dimensional [Brownian motion](../../../brownian-motion.md) is a real-valued [stochastic process](../../../stochastic-process.md) $(B_t)_{t\geq0}$ satisfying $B_0=0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), having [continuous paths](../../../geometry-and-topology.md#continuous-path) [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), and having [independent increments](../../../stochastic-process.md#independent-increments) with

$$
\boxed{B_t-B_s\sim N(0,t-s)\qquad(0\leq s<t).}
$$

Here $N(0,t-s)$ is the [normal distribution](../../../probability-theory.md#normal-distribution) with zero [expected value](../../../probability-theory.md#expected-value) and [variance](../../../variance.md) $t-s$. Thus the increments are also [stationary increments](../../../stochastic-process.md#stationary-increments).

If [Brownian motion](../../../brownian-motion.md) is defined relative to a specified [filtration](../../../stochastic-process.md#filtration-probability-theory) $(\mathcal F_t)$, additionally require that it is an [adapted process](../../../stochastic-process.md#adapted-process) and that $B_t-B_s$ is [independent](../../../random-variable.md#independent-random-variables) of $\mathcal F_s$. For its [natural filtration](../../../stochastic-process.md#natural-filtration), this follows from [independent increments](../../../stochastic-process.md#independent-increments). **These are the defining properties of standard [Brownian motion](../../../brownian-motion.md).**

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For any finite list $t_1,\ldots,t_k\in[0,1]$, the [random vector](../../../random-variable.md#random-vector) $(U_{t_1},\ldots,U_{t_k},B_1)$ has a [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution), since it is a linear image of a vector of [Brownian motion](../../../brownian-motion.md) coordinates. The [Brownian covariance kernel](../../../random-variable.md#brownian-covariance-kernel) and [linearity of covariance](../../../variance.md#linearity-of-covariance) give

$$
\operatorname{Cov}(U_t,B_1)=\operatorname{Cov}(B_t,B_1)-t\operatorname{Var}(B_1)=t-t=0.
$$

The [independence of uncorrelated jointly normal variables](../../../probability-and-statistics.md#independence-of-uncorrelated-jointly-normal-variables) implies that $(U_{t_1},\ldots,U_{t_k})$ is [independent](../../../random-variable.md#independent-random-variables) of $B_1$. Extending from finite-coordinate cylinder [events](../../../probability-theory.md#event) by [independence extended from generating pi-systems](../../../probability-theory.md#independence-extended-from-generating-pi-systems) proves

$$
\boxed{\sigma(U_t:0\leq t\leq1)\ \text{is independent of}\ \sigma(B_1).}
$$

Thus **the [Brownian bridge](../../../brownian-motion.md#brownian-bridge) is [independent](../../../random-variable.md#independent-random-variables) of its endpoint**. Its [covariance kernel](../../../random-variable.md#covariance-kernel) is $\operatorname{Cov}(U_s,U_t)=\min(s,t)-st$, confirming that $U$ is the standard [Brownian bridge](../../../brownian-motion.md#brownian-bridge). This is the [Brownian bridge independence from its endpoint](../../../brownian-motion.md#brownian-bridge-independence-from-its-endpoint) property.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Put $D_t=B_t-B'_t$. By [independence](../../../random-variable.md#independent-random-variables) of the two [Brownian motions](../../../brownian-motion.md), $D_t/\sqrt2$ is a standard [Brownian motion](../../../brownian-motion.md): its [independent increments](../../../stochastic-process.md#independent-increments) have the [normal distribution](../../../probability-theory.md#normal-distribution) with [variance](../../../variance.md) equal to elapsed time. The [stopping time](../../../martingale.md#stopping-time) $\tau$ is the first time $D$ hits $-1$ or $3$.

To justify finiteness without presupposing the desired [hitting probability](../../../markov-process.md#hitting-probability), each unit-time increment of $D$ has the [normal distribution](../../../probability-theory.md#normal-distribution) $N(0,2)$. An increment of absolute value greater than $4$ forces exit from $[-1,3]$ if the path was inside at its start. These [independent increments](../../../stochastic-process.md#independent-increments) give $\mathbb P(\tau>n)\leq(1-p)^n$, where $p=\mathbb P(|N(0,2)|>4)>0$. Hence $\tau<\infty$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence).

The [stopped martingale](../../../martingale.md#stopped-martingale) $D_{t\wedge\tau}$ lies in $[-1,3]$. The [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) at $t\wedge\tau$ gives $\mathbb ED_{t\wedge\tau}=0$, and the [bounded convergence theorem](../../../measure-theory.md#bounded-convergence-theorem) gives $\mathbb ED_\tau=0$. Writing $q=\mathbb P(D_\tau=-1)$, path [continuity](../../../calculus.md#continuous-function) gives $0=-q+3(1-q)$. Therefore, as in [Brownian exit from an interval](../../../brownian-motion.md#brownian-exit-from-an-interval),

$$
\boxed{\mathbb P(B_\tau=B'_\tau-1)=\frac34.}
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Fix an integer $k\geq1$ and consider the [independent increments](../../../stochastic-process.md#independent-increments)

$$
\Delta_{j,k}=B_{(j+1)/k}-B_{j/k},\qquad j=0,1,2,\ldots.
$$

For fixed $k$ these are [independent and identically distributed random variables](../../../random-variable.md#independent-and-identically-distributed-random-variables) with the [normal distribution](../../../probability-theory.md#normal-distribution) $N(0,1/k)$, so $p_k=\mathbb P(|\Delta_{j,k}|>1)>0$. The second [Borel-Cantelli lemma](../../../probability-theory.md#borel-cantelli-lemmas) gives $|\Delta_{j,k}|>1$ for infinitely many $j$, [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Intersecting these probability-one [events](../../../probability-theory.md#event) over the countably many $k$ preserves probability one.

On any path in this intersection, [uniform continuity](../../../topological-analysis.md#uniform-continuity) on $[0,\infty)$ would give some $\delta>0$ such that $|B_t-B_s|<1$ whenever $|t-s|<\delta$. Choosing $k$ with $1/k<\delta$ contradicts the existence of an increment $|\Delta_{j,k}|>1$. Therefore [Brownian paths are not uniformly continuous on the half-line](../../../brownian-motion.md#brownian-paths-are-not-uniformly-continuous-on-the-half-line):

$$
\boxed{\mathbb P\bigl(B\text{ is uniformly continuous on }[0,\infty)\bigr)=0.}
$$

The event is measurable: for [continuous paths](../../../geometry-and-topology.md#continuous-path), [uniform continuity](../../../topological-analysis.md#uniform-continuity) can be tested by countably many pairs of nonnegative [rational numbers](../../../number-theory.md#rational-number) and tolerances $1/m$. **[Brownian motion](../../../brownian-motion.md) has [uniform continuity](../../../topological-analysis.md#uniform-continuity) on every compact time interval, but [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) fails it on the whole half-line.**

## 5

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

For a [stopping time](../../../martingale.md#stopping-time) $T$ of a [Brownian filtration](../../../brownian-motion.md#brownian-filtration), define the reflected [stochastic process](../../../stochastic-process.md)

$$
\boxed{\widehat B_t=\begin{cases}B_t,&t\leq T,\\2B_T-B_t,&t>T.\end{cases}}
$$

The [Brownian reflection at a stopping time](../../../brownian-motion.md#brownian-reflection-at-a-stopping-time) form of the [Brownian reflection principle](../../../brownian-motion.md#reflection-principle-wiener-process) states that **$\widehat B$ is again standard [Brownian motion](../../../brownian-motion.md)**. If $T=\infty$, leave the path unchanged; the second branch is used only when $T<t$.

For an [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) finite $T$, the [Strong Markov property](../../../markov-process.md#strong-markov-property) says that $(B_{T+s}-B_T)_{s\geq0}$ is a fresh [Brownian motion](../../../brownian-motion.md) [independent](../../../random-variable.md#independent-random-variables) of $\mathcal F_T$. Its negative has the same [probability distribution](../../../probability-theory.md#probability-distribution), so reflecting the future preserves the full path [probability distribution](../../../probability-theory.md#probability-distribution). Allowing $T=\infty$ follows by applying this argument to $T\wedge n$ and restricting to each fixed finite time interval.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

For $a>0$, the [Brownian reflection principle](../../../brownian-motion.md#reflection-principle-wiener-process) at the [first-passage time](../../../markov-process.md#first-passage-time) of $a$ gives the [Brownian running maximum](../../../brownian-motion.md#brownian-running-maximum) identity

$$
\mathbb P(S_t\geq a)=2\mathbb P(B_t\geq a)=2\left(1-\Phi\left(\frac a{\sqrt t}\right)\right),\qquad t>0,
$$

where $\Phi$ is the [distribution function](../../../probability-theory.md#cumulative-distribution-function) of the standard [normal distribution](../../../probability-theory.md#normal-distribution). Indeed, reflection pairs paths that have reached $a$ and end below $a$ with paths ending above $a$; $B_t$ has no atom at $a$.

As $t\to\infty$, this probability tends to one. The [events](../../../probability-theory.md#event) $\{S_n\geq a\}$ increase with integer $n$, so with probability one the path reaches $a$ in finite time. Taking a countable intersection over positive integer $a$ gives

$$
\boxed{\mathbb P(S_\infty=\infty)=1.}
$$

Here $S_\infty=\sup_{s\geq0}B_s$. This also proves that every positive-level [Brownian first-passage time](../../../markov-process.md#brownian-first-passage-time) is finite [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence).

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Let $T_y=\inf\{s\geq0:B_s=y\}$. Reflect at this [stopping time](../../../martingale.md#stopping-time), using the [Brownian reflection principle](../../../brownian-motion.md#reflection-principle-wiener-process) from (a). Path [continuity](../../../calculus.md#continuous-function) gives $\{S_t\geq y\}=\{T_y\leq t\}$, and on this [event](../../../probability-theory.md#event) the reflected endpoint is $\widehat B_t=2y-B_t$. Consequently

$$
\{S_t\geq y,\ B_t\leq x\}
=\{T_y\leq t,\ \widehat B_t\geq2y-x\}.
$$

Since $x\leq y$, an endpoint $\widehat B_t\geq2y-x\geq y$ forces the reflected path to have hit $y$ by time $t$. Reflection preserves the first hit of $y$, so the condition $T_y\leq t$ is redundant on the right. As $\widehat B$ has the same [probability distribution](../../../probability-theory.md#probability-distribution) as $B$, the [joint distribution of Brownian motion and its running maximum](../../../brownian-motion.md#joint-distribution-of-brownian-motion-and-its-running-maximum) satisfies

$$
\boxed{\mathbb P(S_t\geq y,\ B_t\leq x)=\mathbb P(B_t\geq2y-x).}
$$

This argument includes $x=y$; at positive $t$ the boundary endpoint has zero probability under the [normal distribution](../../../probability-theory.md#normal-distribution). At $t=0$ both sides vanish because $y>0$.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

Taking $x=y=a$ in (c) and using that $B_t$ has no atom at $a$ gives

$$
\mathbb P(T_a\leq t)=\mathbb P(S_t\geq a)=2\mathbb P(B_t\geq a)
=2\left(1-\Phi\left(\frac a{\sqrt t}\right)\right),\qquad t>0.
$$

This is the [distribution function](../../../probability-theory.md#cumulative-distribution-function) of the [Brownian first-passage time](../../../markov-process.md#brownian-first-passage-time); (b) ensures that it is a proper [probability distribution](../../../probability-theory.md#probability-distribution). Comparing these [distribution functions](../../../probability-theory.md#cumulative-distribution-function) gives the [Brownian scaling](../../../brownian-motion.md#brownian-scaling) identity $T_{ca}\overset d=c^2T_a$ for $c>0$.

For an integer $n\geq1$, set $T_0=0$ and successively hit the levels $a,2a,\ldots,na$. The [Strong Markov property](../../../markov-process.md#strong-markov-property) at these finite [stopping times](../../../martingale.md#stopping-time) and spatial translation imply that

$$
T_a-T_0,\ T_{2a}-T_a,\ldots,T_{na}-T_{(n-1)a}
$$

are [independent random variables](../../../random-variable.md#independent-random-variables), each with the [probability distribution](../../../probability-theory.md#probability-distribution) of $T_a$. Thus, for [independent](../../../random-variable.md#independent-random-variables) copies $T_a^{(j)}$,

$$
T_a^{(1)}+\cdots+T_a^{(n)}\overset d=T_{na}\overset d=n^2T_a.
$$

Therefore

$$
\boxed{\frac{T_a^{(1)}+\cdots+T_a^{(n)}}{n^2}\overset d=T_a,\qquad \alpha=\frac12.}
$$

The paper's definition is the [strictly stable distribution](../../../probability-theory.md#strictly-stable-distribution) convention, with no centering term, a special case of a [stable distribution](../../../probability-theory.md#stable-distribution).

## 6

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

The [Lévy continuity theorem](../../../probability-theory.md#levy-continuity-theorem) states that if [characteristic functions](../../../probability-theory.md#characteristic-function) $\varphi_n$ of [probability distributions](../../../probability-theory.md#probability-distribution) $\mu_n$ converge pointwise on $\mathbb R$ to $\varphi$, and $\varphi$ is continuous at zero, then $\varphi$ is the [characteristic function](../../../probability-theory.md#characteristic-function) of a unique [probability distribution](../../../probability-theory.md#probability-distribution) $\mu$ and

$$
\boxed{\mu_n\Rightarrow\mu.}
$$

Here the arrow denotes [weak convergence of probability measures](../../../convergence-of-random-variables.md#weak-convergence-of-probability-measures), equivalently [convergence in distribution](../../../convergence-of-random-variables.md#convergence-in-distribution) of associated [random variables](../../../random-variable.md). Conversely, [weak convergence of probability measures](../../../convergence-of-random-variables.md#weak-convergence-of-probability-measures) implies pointwise convergence of their [characteristic functions](../../../probability-theory.md#characteristic-function) to the [characteristic function](../../../probability-theory.md#characteristic-function) of the limit. The continuity-at-zero condition is essential to ensure that the pointwise limit is a [characteristic function](../../../probability-theory.md#characteristic-function).

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Write $A_n=n^{-1}\sum_{j=1}^nX_j$ and $\varphi(t)=\mathbb E e^{itX_1}$. The given two-sided limit $|f(u)|/u\to0$ implies $|f(u)|/|u|\to0$, so $f(u)=o(|u|)$. For each fixed real $t$, [independence](../../../random-variable.md#independent-random-variables) and the [characteristic function of a sum of independent variables](../../../probability-theory.md#characteristic-function-of-a-sum-of-independent-variables) give

$$
\mathbb E e^{itA_n}=\left(1+\frac{iat}{n}+f(t/n)\right)^n.
$$

Set $z_n=iat/n+f(t/n)$. For $t\ne0$, $nz_n\to iat$ and $z_n=O(n^{-1})$. The local [Taylor expansion](../../../calculus.md#taylor-expansion) of the [complex logarithm](../../../analysis.md#complex-logarithm) at $1$ gives

$$
n\log(1+z_n)=nz_n+O(n|z_n|^2)\longrightarrow iat.
$$

Thus $\mathbb E e^{itA_n}\to e^{iat}$; at $t=0$ the identity is immediate. The limit is continuous at zero and is the [characteristic function](../../../probability-theory.md#characteristic-function) of the constant [random variable](../../../random-variable.md) $a$. The [Lévy continuity theorem](../../../probability-theory.md#levy-continuity-theorem) proves the [weak law from a characteristic-function expansion](../../../probability-theory.md#weak-law-from-a-characteristic-function-expansion):

$$
\boxed{\frac{X_1+\cdots+X_n}{n}\xrightarrow{d}a.}
$$

No [integrability](../../../probability-theory.md#integrable-random-variable) hypothesis has been used. The conclusion is also [convergence in probability](../../../convergence-of-random-variables.md#convergence-in-probability) by (d)'s [convergence in distribution to a constant implies convergence in probability](../../../convergence-of-random-variables.md#convergence-in-distribution-to-a-constant-implies-convergence-in-probability). If the word “constant” were to allow complex $a$, the [characteristic function](../../../probability-theory.md#characteristic-function) symmetry $\varphi(-t)=\overline{\varphi(t)}$ forces $a=\overline a$, so it is necessarily real.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Suppose $X_n\to X$ with [convergence in probability](../../../convergence-of-random-variables.md#convergence-in-probability). For real $t$ and $\delta>0$, the elementary inequality $|e^{iu}-e^{iv}|\leq\min(2,|u-v|)$ gives

$$
\left|\mathbb E e^{itX_n}-\mathbb E e^{itX}\right|
\leq |t|\delta+2\mathbb P(|X_n-X|>\delta).
$$

First let $n\to\infty$, then let $\delta\downarrow0$. The [characteristic functions](../../../probability-theory.md#characteristic-function) converge pointwise to that of $X$, which is continuous at zero. The [Lévy continuity theorem](../../../probability-theory.md#levy-continuity-theorem) gives **[convergence in probability](../../../convergence-of-random-variables.md#convergence-in-probability) implies [convergence in distribution](../../../convergence-of-random-variables.md#convergence-in-distribution)**.

For the converse, let $Z$ have the fair [Bernoulli distribution](../../../discrete-probability-distribution.md#bernoulli-distribution), put $X=Z$, and set $X_n=1-Z$ for every $n$. All $X_n$ have the same [probability distribution](../../../probability-theory.md#probability-distribution) as $X$, so $X_n\xrightarrow dX$. But $|X_n-X|=1$ always, hence

$$
\boxed{\mathbb P(|X_n-X|>1/2)=1\quad\text{for every }n.}
$$

There is no [convergence in probability](../../../convergence-of-random-variables.md#convergence-in-probability) to $X$. In this example $X_n$ does have [convergence in probability](../../../convergence-of-random-variables.md#convergence-in-probability) to $1-Z$: the counterexample concerns the converse with the specified limit $X$, as usual. If one interprets the question as denying [convergence in probability](../../../convergence-of-random-variables.md#convergence-in-probability) to any limit, take $X_n=Z$ for even $n$ and $X_n=1-Z$ for odd $n$. Its [probability distribution](../../../probability-theory.md#probability-distribution) is still constant, while the two subsequences have distinct limits from [almost sure convergence](../../../convergence-of-random-variables.md#almost-sure-convergence), ruling out any common limit in probability by [uniqueness of a limit in probability](../../../convergence-of-random-variables.md#uniqueness-of-a-limit-in-probability).

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

Let $F_n$ be the [distribution function](../../../probability-theory.md#cumulative-distribution-function) of $X_n$. The limiting constant zero has [distribution function](../../../probability-theory.md#cumulative-distribution-function) $F(x)=0$ for $x<0$ and $F(x)=1$ for $x\geq0$. For every $\varepsilon>0$, both $-\varepsilon$ and $\varepsilon$ are continuity points of $F$. Thus [convergence in distribution](../../../convergence-of-random-variables.md#convergence-in-distribution) implies $F_n(-\varepsilon)\to0$ and $F_n(\varepsilon)\to1$. Therefore

$$
0\leq\mathbb P(|X_n|>\varepsilon)
\leq F_n(-\varepsilon)+1-F_n(\varepsilon)\longrightarrow0.
$$

This proves

$$
\boxed{X_n\xrightarrow d0\ \Longrightarrow\ X_n\xrightarrow{\mathbb P}0.}
$$

The same proof after subtracting a fixed real $c$ proves [convergence in distribution to a constant implies convergence in probability](../../../convergence-of-random-variables.md#convergence-in-distribution-to-a-constant-implies-convergence-in-probability). A deterministic limit fixes the coupling automatically; the counterexample in (c) exploits a nonconstant limit whose [probability distribution](../../../probability-theory.md#probability-distribution) alone does not fix that coupling.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
