<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

A loaded gun remains loaded after its visit with [probability](../../../../../probability.md) $1/2$. An unloaded gun is loaded and then not fired with [probability](../../../../../probability.md) $(3/4)(1/2)=3/8$. The visited gun's new loaded [probability](../../../../../probability.md) is therefore

$$
p'=\frac p2+\frac{3(1-p)}8=\frac38+\frac p8.
$$

Preservation requires $p'=p$, giving

$$
\boxed{p=\frac37.}
$$

This is [product stationarity under single-coordinate Markov updates](../../../../../product-stationarity-under-single-coordinate-markov-updates.md): the visited coordinate has the same [Bernoulli distribution](../../../../../bernoulli-distribution.md) afterward, and its [independent](../../../../../independent-random-variables.md) local random decisions do not affect the other coordinates. Thus the originally [independent](../../../../../independent-random-variables.md) [indicator random variables](../../../../../indicator-random-variable.md) remain jointly [independent](../../../../../independent-random-variables.md) after each scheduled visit, not merely equal in their marginal [probabilities](../../../../../probability.md).

Let $X_j$ be the [indicator random variable](../../../../../indicator-random-variable.md) that gun $j$ is loaded. Then $N=\sum_{j=1}^mX_j$ has [binomial distribution](../../../../../binomial-distribution.md) with parameters $m,3/7$. By [linearity of expectation](../../../../../linearity-of-expectation.md) and [independence](../../../../../independent-random-variables.md) of the [indicator random variables](../../../../../indicator-random-variable.md),

$$
\boxed{\mathbb EN=\frac{3m}{7},\qquad
\operatorname{Var}N=\sum_{j=1}^m\operatorname{Var}X_j
=m\frac37\frac47=\frac{12m}{49}.}
$$

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
