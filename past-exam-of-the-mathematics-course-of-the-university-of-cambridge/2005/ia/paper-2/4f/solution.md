<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

A [Poisson distribution](../../../../../poisson-distribution.md) with parameter $\lambda>0$ assigns [probability mass function](../../../../../probability-mass-function.md)

$$
P(Z=k)=e^{-\lambda}\frac{\lambda^k}{k!},\qquad k=0,1,2,\ldots.
$$

The [exponential series](../../../../../exponential-series.md) makes these probabilities sum to one. Shifting the indices in the absolutely convergent sums gives

$$
E Z=e^{-\lambda}\sum_{k\geq1}\frac{k\lambda^k}{k!}=\lambda,
\qquad E[Z(Z-1)]=\lambda^2.
$$

Hence $E Z^2=\lambda^2+\lambda$ and

$$
\boxed{E Z=\operatorname{Var}Z=\lambda.}
$$

For [independent random variables](../../../../../independent-random-variables.md) $Z_1,\ldots,Z_n$ of parameter one, let $S_n=\sum_jZ_j$. Summing their product [probability mass function](../../../../../probability-mass-function.md) over all nonnegative $k_1+\cdots+k_n=k$ gives

$$
P(S_n=k)=e^{-n}\sum_{k_1+\cdots+k_n=k}\frac1{k_1!\cdots k_n!}
=e^{-n}\frac{n^k}{k!}.
$$

The final equality follows from the [multinomial theorem](../../../../../multinomial-theorem.md) applied to $(1+\cdots+1)^k$. Thus **$S_n$ has the Poisson distribution of parameter $n$**.

Each $Z_j$ has [expectation](../../../../../expected-value.md) and [variance](../../../../../variance-split.md) one, so the [central limit theorem](../../../../../central-limit-theorem.md) gives [convergence in distribution](../../../../../convergence-in-distribution.md)

$$
\frac{S_n-n}{\sqrt n}\ \Longrightarrow\ N(0,1).
$$

Zero is a continuity point of the [standard normal cumulative distribution function](../../../../../standard-normal-distribution-function.md). Therefore

$$
\boxed{e^{-n}\sum_{k=0}^n\frac{n^k}{k!}=P(S_n\leq n)
=P\left(\frac{S_n-n}{\sqrt n}\leq0\right)\longrightarrow\frac12.}
$$

The discrete atom at $S_n=n$ causes no difficulty: the [central limit theorem](../../../../../central-limit-theorem.md) applies to the entire event with threshold zero.

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
