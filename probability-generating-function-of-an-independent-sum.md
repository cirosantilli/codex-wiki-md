# Probability generating function of an independent sum

↑ **Parent:** [Probability generating function](probability-generating-function.md)

For nonnegative integer-valued [independent random variables](independent-random-variables.md) $X,Y$, factor the [expected value](expected-value-split.md) of a product:

$$
G_{X+Y}(s)=\mathbb E[s^Xs^Y]=\mathbb E[s^X]\mathbb E[s^Y]=G_X(s)G_Y(s),\qquad |s|\leq1.
$$

The [Cauchy product](cauchy-product.md) explains what this means for individual [probability masses](probability-mass.md):

$$
\mathbb P(X+Y=n)=\sum_{j=0}^n\mathbb P(X=j)\mathbb P(Y=n-j).
$$

Every way of splitting the total contributes once. This is [convolution of independent random variables](convolution-of-independent-random-variables.md); multiplying [probability generating functions](probability-generating-function.md) performs the bookkeeping automatically.

For an original example, take [independent](independent-random-variables.md) $X\sim\operatorname{Bernoulli}(0.3)$ and $Y\sim\operatorname{Binomial}(2,0.5)$, using the [Bernoulli distribution](bernoulli-distribution.md) and [binomial distribution](binomial-distribution.md). Then

$$
G_X(s)=0.7+0.3s,\qquad G_Y(s)=\frac{(1+s)^2}{4},
$$

so

$$
G_{X+Y}(s)=\frac{(0.7+0.3s)(1+s)^2}{4}=0.175+0.425s+0.325s^2+0.075s^3.
$$

Direct enumeration of the six pairs $(x,y)$ gives the same [probability masses](probability-mass.md). For example, total one collects $(0,1)$ and $(1,0)$, with contributions $0.7\cdot0.5+0.3\cdot0.25=0.425$. The [coefficients](coefficient.md) sum to one. The [expected value](expected-value-split.md) is $G_{X+Y}'(1)=1.3$; since $G_{X+Y}''(1)=1.1$, the [variance](variance-split.md) is $1.1+1.3-1.3^2=0.71$, agreeing with $0.3\cdot0.7+2\cdot0.5\cdot0.5$.

<a id="image-multiplying-probability-generating-functions-accounts-for-every-pair-with-the-same-total"></a>
![](probability-generating-function-coefficient-convolution.png)

**[Figure 8](#image-multiplying-probability-generating-functions-accounts-for-every-pair-with-the-same-total). Multiplying probability generating functions accounts for every pair with the same total**. The six cells give the exact [joint probability mass function](joint-probability-mass-function.md) for the chosen [independent](independent-random-variables.md) [Bernoulli distribution](bernoulli-distribution.md) and [binomial distribution](binomial-distribution.md). Colors group equal totals; the stacked bars collect their contributions to the [coefficients](coefficient.md) of the product [probability generating function](probability-generating-function.md). These are calculated model probabilities.

[Uncorrelated random variables](uncorrelated-random-variables.md) are insufficient for the product identity. For a concrete counterexample, let $U$ be uniform on $\{-1,0,1\}$ and set $A=U+1$, $B=U^2$. Then $\operatorname{Cov}(A,B)=\mathbb E[U^3]=0$, but $\mathbb P(A+B=0)=0$, whereas $G_A(0)G_B(0)=1/9$. Zero [covariance](covariance.md) controls one mixed [moment](moment.md), not the full [joint probability mass function](joint-probability-mass-function.md).

## ↑ Ancestors (7)

1. [Probability generating function](probability-generating-function.md)
2. [Probability distribution](probability-distribution-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Probability generating function of an independent random sum](probability-generating-function-of-an-independent-random-sum.md)
