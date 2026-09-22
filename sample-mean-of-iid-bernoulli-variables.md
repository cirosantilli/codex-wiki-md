# Sample mean of iid Bernoulli variables

↑ **Parent:** [Independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md)

For $n\geq1$ [independent and identically distributed](independent-and-identically-distributed-random-variables.md) [Bernoulli random variables](bernoulli-distribution.md) with success probability $p$, the [sum](sum.md) $K=\sum_iX_i$ has a [binomial distribution](binomial-distribution.md). Every length-$n$ pattern with $k$ successes has [probability](probability.md) $p^k(1-p)^{n-k}$, and the [binomial coefficient](binomial-coefficient-split.md) counts its $\binom nk$ possible success positions. Therefore

$$
\mathbb P(\overline X=k/n)=\binom nk p^k(1-p)^{n-k},\qquad
\mathbb E[\overline X]=p,\qquad
\operatorname{Var}(\overline X)=\frac{p(1-p)}n.
$$

The usual endpoint convention includes $p=0$ and $p=1$ as deterministic cases. For $p=1/2$ and $n=4$, the five [probability masses](probability-mass.md) are $1,4,6,4,1$ divided by $16$. The [sample mean](sample-mean.md) takes values $0,1/4,1/2,3/4,1$, with [variance](variance-split.md) $1/16$ and [standard deviation](standard-deviation.md) $1/4$. At $n=64$, its variance is $1/256$ and its standard deviation is $1/16$.

<a id="image-exact-sample-mean-distributions-distinguish-fresh-iid-draws-from-a-copied-common-coin"></a>
![](iid-versus-common-coin-sample-means.png)

**[Figure 7](#image-exact-sample-mean-distributions-distinguish-fresh-iid-draws-from-a-copied-common-coin). Exact sample-mean distributions distinguish fresh IID draws from a copied common coin**. Original exact [binomial distribution](binomial-distribution.md) probabilities for sample sizes $1,4,16,64$. Blue marks give the mass at each possible mean under independent fair draws. Orange marks give the masses for the same fair draw copied $n$ times: $1/2$ at zero and $1/2$ at one for every $n$. These are discrete [probability masses](probability-mass.md), not density values or measured histograms.

## ↑ Ancestors (8)

1. [Independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md)
2. [Independent random variables](independent-random-variables.md)
3. [Random variable](random-variable-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
