<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Condition on $N$. Since the amounts are [independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md) and are independent of $N$, their [moment-generating functions](../../../../../../moment-generating-function.md) multiply:

$$
\mathbb E[e^{tS}\mid N=n]=M_X(t)^n.
$$

Summing against the positive-support [geometric distribution](../../../../../../geometric-distribution.md) gives the [geometric-sum moment-generating function](../../../../../../geometric-sum-moment-generating-function.md)

$$
\boxed{M_S(t)=\sum_{n\geq1}p(1-p)^{n-1}M_X(t)^n
=\frac{pM_X(t)}{1-(1-p)M_X(t)}.}
$$

The finite-transform domain is $M_X(t)<\infty$ and $(1-p)M_X(t)<1$. The terms are nonnegative for real $t$, so if the latter condition fails the sum diverges. For $t\leq0$ both conditions always hold, since the claims are positive; thus the same calculation always provides the [Laplace transform of a nonnegative random variable](../../../../../../laplace-transform-of-a-nonnegative-random-variable.md). Positivity alone does not guarantee a finite [moment-generating function](../../../../../../moment-generating-function.md) on a positive neighbourhood of zero.

There is at least one strictly positive amount in the portfolio. Hence **$\mathbb P(S=0)=0$**; zero carries no [atom of a measure](../../../../../../atom-measure-theory.md) to add to the continuous laws in the next two parts.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
