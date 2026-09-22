<h1 id="10f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [Poisson distribution](../../../../../../poisson-distribution.md) with parameter $\mu$ has [probability generating function](../../../../../../probability-generating-function.md) $G_N(s)=e^{\mu(s-1)}$. The preceding part gives $G_F(s)=e^{\mu p(s-1)}$, the [probability generating function](../../../../../../probability-generating-function.md) of a [Poisson distribution](../../../../../../poisson-distribution.md) with parameter $\mu p$. To prove [independence](../../../../../../independent-random-variables.md), retain both counts:

$$
\mathbb E[s^Ft^S\mid N]=(ps+(1-p)t)^N.
$$

Consequently the joint [probability generating function](../../../../../../probability-generating-function.md) factors as

$$
\mathbb E[s^Ft^S]=e^{\mu(ps+(1-p)t-1)}=e^{\mu p(s-1)}e^{\mu(1-p)(t-1)}.
$$

Comparing the coefficients of $s^ft^k$ proves that the joint [probabilities](../../../../../../probability.md) are the products of the marginal [probabilities](../../../../../../probability.md). Hence **$F$ and $S$ are independent, with distributions $\operatorname{Poisson}(\mu p)$ and $\operatorname{Poisson}(\mu(1-p))$**. This is [Poisson thinning](../../../../../../poisson-thinning.md), including the degenerate counts when $p=0$ or $p=1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
