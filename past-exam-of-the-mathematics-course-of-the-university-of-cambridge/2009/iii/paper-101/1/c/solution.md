<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [exponential distribution](../../../../../../exponential-distribution.md) has no atoms, so all sample values are distinct [almost surely](../../../../../../almost-sure-convergence.md), and $M_i$ is the $i$th [order statistic](../../../../../../order-statistic.md). Set $M_0=0$ and $D_i=M_i-M_{i-1}$. Part (b) gives $D_1\sim\operatorname{Exp}(n\lambda)$.

To justify induction and the required [independence](../../../../../../independent-random-variables.md), let $J$ be the label attaining the minimum. Conditional on its time and label, the remaining clocks are fresh [independent](../../../../../../independent-random-variables.md) rate-$\lambda$ [exponential random variables](../../../../../../exponential-distribution.md), by the [memoryless property](../../../../../../memorylessness-of-the-exponential-distribution.md). This conditional claim can be checked directly: for a specified label $j$, first ringing time $u$, and residual lifetimes $y_k>0$ for $k\ne j$, the [joint probability density](../../../../../../joint-probability-density.md) is

$$
\lambda^n e^{-\lambda(nu+\sum_{k\ne j}y_k)}
=\frac1n\left(n\lambda e^{-n\lambda u}\right)
\prod_{k\ne j}\left(\lambda e^{-\lambda y_k}\right).
$$

Thus the first minimum, its uniform winning label and the surviving residual clocks are [independent](../../../../../../independent-random-variables.md). Repeat this argument after each minimum. At the $i$th step there are $n-i+1$ clocks, so the [independent exponential order-statistic spacings](../../../../../../independent-exponential-order-statistic-spacings.md) satisfy

$$
D_i\sim\operatorname{Exp}((n-i+1)\lambda),\qquad D_1,\ldots,D_n\text{ independent}.
$$

Since $Y_k/k$ has rate $k\lambda$ whenever $Y_k\sim\operatorname{Exp}(\lambda)$, summing the gaps proves

$$
\boxed{M_i\overset d=\sum_{k=n-i+1}^n\frac{Y_k}{k}.}
$$

In particular the maximum is $M^*=M_n$. By [variance additivity for independent random variables](../../../../../../variance-additivity-for-independent-random-variables.md) and the [Laplace transform of an exponential distribution](../../../../../../laplace-transform-of-an-exponential-distribution.md), its requested quantities are

$$
\boxed{\mathbb EM^*=\frac1\lambda\sum_{k=1}^n\frac1k,\qquad
\operatorname{Var}(M^*)=\frac1{\lambda^2}\sum_{k=1}^n\frac1{k^2},\qquad
\mathbb E e^{-sM^*}=\prod_{k=1}^n\frac{k\lambda}{k\lambda+s}\quad(s\geq0).}
$$

The product follows from [independence](../../../../../../independent-random-variables.md) of the gaps, not merely from their marginal [probability distributions](../../../../../../probability-distribution.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
