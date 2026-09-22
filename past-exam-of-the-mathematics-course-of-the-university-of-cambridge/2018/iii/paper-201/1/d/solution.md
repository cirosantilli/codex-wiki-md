<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\xi_1,\xi_2,\ldots$ be [independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md) with the fair [Bernoulli distribution](../../../../../../bernoulli-distribution.md), and put

$$
M_0=1,\qquad M_n=2^n\mathbf1_{\{\xi_1=\cdots=\xi_n=1\}}.
$$

Relative to $\mathcal F_n=\sigma(\xi_1,\ldots,\xi_n)$, this [fair-coin doubling martingale](../../../../../../fair-coin-doubling-martingale.md) satisfies $\mathbb E[M_{n+1}\mid\mathcal F_n]=M_n$: while alive it doubles with probability $1/2$ and becomes zero otherwise. Its [expected value](../../../../../../expected-value.md) is $\mathbb E M_n=2^n2^{-n}=1$.

The probability of an infinite run of ones is $\lim_n2^{-n}=0$, so $M_n$ is eventually zero [almost surely](../../../../../../almost-sure-convergence.md). However,

$$
\boxed{M_n\to0\ \text{almost surely},\qquad \mathbb E|M_n-0|=1\ \text{for every }n.}
$$

Thus the [martingale](../../../../../../martingale-split.md) lacks [convergence in L1](../../../../../../convergence-in-l1.md) to its limit from [almost sure convergence](../../../../../../almost-sure-convergence.md). Nor can it have [convergence in L1](../../../../../../convergence-in-l1.md) to any other limit: [convergence in L1](../../../../../../convergence-in-l1.md) implies [convergence in probability](../../../../../../convergence-in-probability.md), whose limit is unique up to [almost sure equality](../../../../../../almost-sure-equality.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
