<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a [submartingale](../../../../../submartingale.md) $(Z_n)$ and $a<b$, let $U_N(a,b)$ count the completed [upcrossings](../../../../../upcrossing.md) of $[a,b]$ by time $N$. The [Doob upcrossing inequality](../../../../../doob-upcrossing-inequality.md) gives

$$
(b-a)\mathbb E U_N(a,b)\leq\mathbb E(Z_N-a)^+.
$$

For a [martingale](../../../../../martingale-split.md) $(X_n)$, a useful sharper form is

$$
\boxed{(b-a)\mathbb E U_N(a,b)\leq\mathbb E(X_N-a)^-.}
$$

Here $x^+=\max(x,0)$ and $x^-=\max(-x,0)$. To see the martingale form, use a bounded [predictable process](../../../../../predictable-process.md) $H_k\in\{0,1\}$ that holds one unit after an observation at or below $a$ and releases it on the next observation at or above $b$. Its gain $G_N=\sum_{k=1}^NH_k(X_k-X_{k-1})$ is at least $(b-a)U_N-(X_N-a)^-$: completed trades earn at least $b-a$, and any unfinished trade loses at most $(X_N-a)^-$. Since $\mathbb E G_N=0$, the bound follows. For the submartingale version, apply the same strategy to $(Z_n-a)^+$, itself a [submartingale](../../../../../submartingale.md). Each purchase occurs at value zero, so its gain is at least $(b-a)U_N$. The complementary predictable strategy has nonnegative expected gain, bounding this strategy's expected gain by $\mathbb E(Z_N-a)^+-\mathbb E(Z_0-a)^+$, and in particular by the stated right side.

The almost-sure [martingale convergence theorem](../../../../../martingale-convergence-theorem.md) says that if $C=\sup_n\mathbb E|X_n|<\infty$, then $X_n$ converges almost surely to a finite, integrable [random variable](../../../../../random-variable-split.md) $Y$, with $\mathbb E|Y|\leq C$. Indeed, the [Doob upcrossing inequality](../../../../../doob-upcrossing-inequality.md) bounds the expected total number of [upcrossings](../../../../../upcrossing.md) of every rational interval by $(C+|a|)/(b-a)$. By [monotone convergence](../../../../../monotone-convergence-theorem.md), each such total count is finite almost surely; intersect these probability-one events over all rational $a<b$. If the lower and upper limits of a [sample path](../../../../../sample-path.md) differed, some rational interval strictly between them would be crossed infinitely often. Thus each remaining path has a limit in the extended real line. The [Fatou lemma](../../../../../fatou-s-lemma.md) gives

$$
\mathbb E\bigl[\liminf_n|X_n|\bigr]\leq C,
$$

so the limit is finite almost surely and integrable. Almost-sure convergence by itself neither preserves [expectations](../../../../../expected-value.md) nor supplies this uniform first-moment bound.

For the loss of [expectation](../../../../../expected-value.md), let $(\eta_k)$ be independent variables with the fair [Bernoulli distribution](../../../../../bernoulli-distribution.md) and set

$$
X_0=1,\qquad X_n=2^n\mathbf1_{\{\eta_1=\cdots=\eta_n=1\}}.
$$

Conditional on the past, survival doubles the value with [probability](../../../../../probability.md) $1/2$ and otherwise sets it to zero, so this is a [nonnegative martingale](../../../../../nonnegative-martingale.md). An infinite string of successes has [probability](../../../../../probability.md) zero. The process therefore eventually vanishes almost surely, giving **yes: $X_0=1$ and $Y=0$ almost surely are possible**. Its [expectations](../../../../../expected-value.md) remain one at every finite time; the process is not [uniformly integrable](../../../../../uniform-integrability.md).

A nonintegrable limit is also possible for a signed [martingale](../../../../../martingale-split.md). Take independent $\xi_k$ with

$$
\mathbb P(\xi_k=4^k)=\mathbb P(\xi_k=-4^k)=2^{-k-1},\qquad
\mathbb P(\xi_k=0)=1-2^{-k},\qquad k\geq1,
$$

and let $M_0=1$, $M_n=1+\sum_{k=1}^n\xi_k$. Every increment has mean zero and a finite absolute [expectation](../../../../../expected-value.md), so each $M_n$ is integrable and $(M_n)$ is a [martingale](../../../../../martingale-split.md). Since $\sum_k\mathbb P(\xi_k\ne0)<\infty$, the [Borel-Cantelli lemma](../../../../../borel-cantelli-lemmas.md) makes only finitely many increments nonzero almost surely; hence the finite limit $Y=1+\sum_k\xi_k$ exists almost surely. To compute its absolute [expectation](../../../../../expected-value.md), let $A_k$ be the event that only the $k$th increment is nonzero. [Independence](../../../../../independent-random-variables.md) gives

$$
\mathbb P(A_k)=2^{-k}\prod_{j\ne k}(1-2^{-j})\geq c2^{-k},\qquad
c=\prod_{j\geq1}(1-2^{-j})>0.
$$

The [infinite product](../../../../../infinite-product.md) is positive because its tail logarithms are bounded in absolute value by a constant times the summable series $\sum_j2^{-j}$. The events $A_k$ are disjoint, and on $A_k$, $|Y|\geq4^k-1$. Therefore

$$
\mathbb E|Y|\geq c\sum_{k\geq1}2^{-k}(4^k-1)=\infty.
$$

Thus **yes: a finite almost-sure martingale limit can have infinite absolute [expectation](../../../../../expected-value.md)**, even with deterministic $M_0=1$. This is [almost-sure martingale convergence to a nonintegrable limit](../../../../../almost-sure-martingale-convergence-to-a-nonintegrable-limit.md); the missing hypothesis is the uniform first-moment bound. For a [nonnegative martingale](../../../../../nonnegative-martingale.md), in contrast, the [Fatou lemma](../../../../../fatou-s-lemma.md) would force the limit to be integrable.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
