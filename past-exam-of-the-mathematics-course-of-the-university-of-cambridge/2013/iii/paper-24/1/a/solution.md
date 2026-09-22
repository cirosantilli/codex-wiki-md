<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [martingale convergence theorem](../../../../../../martingale-convergence-theorem.md) says that a discrete-time [martingale](../../../../../../martingale-split.md) $(M_n,\mathcal F_n)$ satisfying

$$
\sup_n\mathbb E|M_n|<\infty
$$

has an [almost sure convergence](../../../../../../almost-sure-convergence.md) limit $M_\infty$, finite [almost surely](../../../../../../almost-sure-convergence.md) and in $L^1$. The theorem asserts that the limit is integrable; it does not assert [convergence in L1](../../../../../../convergence-in-l1.md). More generally, the [almost sure submartingale convergence theorem](../../../../../../almost-sure-submartingale-convergence-theorem.md) applies to a [submartingale](../../../../../../submartingale.md) with $\sup_n\mathbb E M_n^+<\infty$. [Uniform integrability](../../../../../../uniform-integrability.md) is the additional condition that upgrades a [martingale](../../../../../../martingale-split.md)'s convergence to [convergence in L1](../../../../../../convergence-in-l1.md).

For the requested distinction, let $(\xi_k)$ be independent fair Bernoulli variables and use their [natural filtration](../../../../../../natural-filtration.md). The [coin-doubling martingale](../../../../../../coin-doubling-martingale.md)

$$
M_0=1,\qquad M_n=2^n\mathbf1_{\{\xi_1=\cdots=\xi_n=1\}}
$$

is a [nonnegative martingale](../../../../../../nonnegative-martingale.md): conditionally on $\mathcal F_n$, the next factor is $2\xi_{n+1}$ with mean one, so $\mathbb E(M_{n+1}\mid\mathcal F_n)=M_n$. Also $\mathbb E|M_n|=\mathbb E M_n=1$ for every $n$, giving the required uniform $L^1$ bound. The probability that all the Bernoulli variables equal one is $\lim_n2^{-n}=0$. Therefore a zero is eventually encountered [almost surely](../../../../../../almost-sure-convergence.md), after which $M_n$ stays zero. Thus

$$
\boxed{M_n\longrightarrow0\text{ almost surely},\qquad
\mathbb E|M_n-0|=1\text{ for every }n.}
$$

There can be no other $L^1$ limit, since [convergence in L1](../../../../../../convergence-in-l1.md) implies [convergence in probability](../../../../../../convergence-in-probability.md), whose limit must agree with the almost sure limit. **This [martingale](../../../../../../martingale-split.md) satisfies the almost sure theorem but does not converge in $L^1$.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
