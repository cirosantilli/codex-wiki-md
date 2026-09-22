<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Define $N_i=\sum_{k=1}^N\mathbf1_{\{X_k=a_i\}}$. Grouping equal [claim sizes](../../../../../../claim-size.md) gives the pathwise identity

$$
\boxed{\widetilde T=\sum_{i=1}^m a_iN_i.}
$$

Conditional on $N=n$, the $n$ [independent](../../../../../../independent-random-variables.md) claims receive category labels with [probabilities](../../../../../../probability.md) $p_i$. There are $n!/(n_1!\cdots n_m!)$ assignments producing prescribed category counts, and every assignment has [probability](../../../../../../probability.md) $\prod_i p_i^{n_i}$. Thus the conditional [probability distribution](../../../../../../probability-distribution.md) is a [multinomial distribution](../../../../../../multinomial-distribution.md):

$$
\mathbb P(N_1=n_1,\ldots,N_m=n_m\mid N=n)
=\frac{n!}{\prod_i n_i!}\prod_i p_i^{n_i}
$$

when the nonnegative counts sum to $n$, and is zero otherwise.

For $0\le z_i\le1$, condition first on $N$ and use the [probability generating function](../../../../../../probability-generating-function.md) of a [Poisson distribution](../../../../../../poisson-distribution.md):

$$
\mathbb E\prod_i z_i^{N_i}
=\mathbb E\left(\sum_i p_i z_i\right)^N
=\exp\left\{\lambda\left(\sum_i p_i z_i-1\right)\right\}
=\prod_i\exp\{\lambda p_i(z_i-1)\}.
$$

This factorization is the joint [probability generating function](../../../../../../probability-generating-function.md) of [independent](../../../../../../independent-random-variables.md) [Poisson distribution](../../../../../../poisson-distribution.md) variables. Hence

$$
\boxed{N_i\sim\operatorname{Pois}(\lambda p_i)\quad\text{independently}.}
$$

A category with $p_i=0$ has zero count [almost surely](../../../../../../almost-sure-convergence.md). The [categorical thinning of a Poisson claim count](../../../../../../categorical-thinning-of-a-poisson-claim-count.md) produces [independence](../../../../../../independent-random-variables.md) after averaging over the random total, even though the counts are constrained to sum to $n$ conditional on that total.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
