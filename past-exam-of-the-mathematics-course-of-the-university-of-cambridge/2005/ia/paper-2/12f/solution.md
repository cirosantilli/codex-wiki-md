<h1 id="12f/solution">Solution</h1>

↑ **Parent:** [12F](../12f.md)

For each $i$, let $R_i$ be the relative rank of $a_i$ among $a_1,\ldots,a_i$, with the smallest value assigned rank one. Then $Y_i=\mathbf1_{\{R_i=1\}}$. The [independent relative ranks of a uniform random permutation](../../../../../independent-relative-ranks-of-a-uniform-random-permutation.md) can be proved directly: for any choices $r_i\in\{1,\ldots,i\}$, insert the index $i$ at position $r_i$ in the list of previous indices ordered by their values. After all insertions, assign the values $1,\ldots,n$ along that list. This is a unique [permutation](../../../../../permutation.md) with those relative ranks, and conversely every permutation yields one such insertion sequence.

There are $\prod_{i=1}^ni=n!$ possible insertion sequences, all equally likely because the [uniform random permutation](../../../../../uniform-random-permutation.md) is uniform. Thus

$$
P(R_1=r_1,\ldots,R_n=r_n)=\frac1{n!}=\prod_{i=1}^n\frac1i.
$$

The ranks are [independent](../../../../../independent-random-variables.md) and each is uniform on its $i$ possible values. It follows that the [independent record indicators](../../../../../independent-record-indicators.md) have

$$
\boxed{P(Y_i=1)=\frac1i,\quad P(Y_i=0)=1-\frac1i,\qquad Y_i\sim\operatorname{Bernoulli}(1/i).}
$$

The first indicator is the constant one, which is also independent of the others. For $K_n=\sum_{i=1}^nY_i$, additivity of [expectation](../../../../../expected-value.md) and [variance additivity for independent random variables](../../../../../variance-additivity-for-independent-random-variables.md) give

$$
\boxed{E K_n=H_n=\sum_{i=1}^n\frac1i,\qquad
\operatorname{Var}K_n=H_n-\sum_{i=1}^n\frac1{i^2}.}
$$

Here $H_n$ is the [harmonic number](../../../../../harmonic-number.md).

Let $T$ be the year index of the second record. For $2\leq i\leq n$, independence gives

$$
\boxed{P(T=i)=\left[\prod_{j=2}^{i-1}\left(1-\frac1j\right)\right]\frac1i
=\frac1{i(i-1)}.}
$$

The empty product for $i=2$ is one. There is no second record in the first $n$ years with [probability](../../../../../probability.md)

$$
P(T>n)=\prod_{j=2}^n\frac{j-1}{j}=\frac1n.
$$

This exposes a finite-horizon qualification in the final request: a permutation of length $n$ alone does not specify when a record outside those years will occur. Under the usual continuation by an infinite sequence of independent, identically distributed observations with a continuous distribution, the same relative-rank argument holds for every finite prefix. Then $P(T=i)=1/[i(i-1)]$ for every $i\geq2$, and $P(T>m)=1/m$. These probabilities sum to one, so the second record occurs almost surely, but

$$
\boxed{E T=\sum_{i=2}^\infty\frac1{i-1}=\infty.}
$$

The expected number of additional years after year one, $E(T-1)$, is also infinite. This is the first-sample case of the [waiting time for a new record after a fixed sample](../../../../../waiting-time-for-a-new-record-after-a-fixed-sample.md).

If instead one asks for the mean year conditional on the second record occurring within the stated $n$ years, then, for $n\geq2$,

$$
\boxed{E[T\mid T\leq n]=\frac{\sum_{i=2}^n1/(i-1)}{1-1/n}
=\frac{n}{n-1}H_{n-1}.}
$$

The mean additional wait under that conditioning is this value minus one. These are distinct questions: assigning $T=\infty$ whenever no second record occurs in the finite horizon also gives an infinite unconditional mean, whereas a censored observation $\min(T,n)$ has finite [expectation](../../../../../expected-value.md) $1+H_{n-1}$ by the [tail-sum formula for expectation](../../../../../tail-sum-formula-for-expectation.md).

## ↑ Ancestors (10)

1. [12F](../12f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
