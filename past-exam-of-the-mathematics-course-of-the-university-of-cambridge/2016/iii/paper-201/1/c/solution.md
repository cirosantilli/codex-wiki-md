<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take [independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md) $\xi_k$ with the [Bernoulli distribution](../../../../../../bernoulli-distribution.md) of parameter $1/2$, and their [natural filtration](../../../../../../natural-filtration.md). Set

$$
\boxed{M_n=2^n\mathbf1_{\{\xi_1=\cdots=\xi_n=1\}},\qquad M_0=1.}
$$

The event at $n=0$ is the whole sample space. [Independence](../../../../../../independent-random-variables.md) gives

$$
\mathbb E[M_{n+1}\mid\mathcal F_n]
=2^{n+1}\mathbf1_{\{\xi_1=\cdots=\xi_n=1\}}\,\frac12=M_n,
$$

so this is a nonnegative [martingale](../../../../../../martingale-split.md); it is integrable with $\mathbb E M_n=1$. The first zero among the $\xi_k$ is almost surely finite, since the probability of having only ones through time $n$ is $2^{-n}\to0$. After that first zero, every $M_n$ is zero. Hence **the almost sure limit is zero**:

$$
\boxed{M_n\longrightarrow0\quad\text{almost surely},\qquad\mathbb E M_n=1.}
$$

This [fair-coin doubling martingale](../../../../../../fair-coin-doubling-martingale.md) also exhibits failure of [uniform integrability](../../../../../../uniform-integrability.md): [convergence in L1](../../../../../../convergence-in-l1.md) would force the [expectations](../../../../../../expected-value.md) to converge to zero.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
