<h1 id="isserlis-s-theorem">Isserlis's theorem</h1>

↑ **Parent:** [Multivariate Gaussian distribution](multivariate-gaussian-distribution.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Isserlis's_theorem)

For centered jointly [Gaussian random variables](gaussian-random-variable.md), an [odd](odd-function.md) product has zero expectation, and an [even](even-function.md) product's expectation is the sum over all pairings of the products of the pair covariances. In particular,

$$
\mathbb E[X_1X_2X_3X_4]
=\mathbb E[X_1X_2]\mathbb E[X_3X_4]
+\mathbb E[X_1X_3]\mathbb E[X_2X_4]
+\mathbb E[X_1X_4]\mathbb E[X_2X_3].
$$

For a proof, the [moment-generating function](moment-generating-function.md) is $\exp(t^T\Sigma t/2)$. Differentiating once in each variable at zero leaves precisely products of covariance entries indexed by complete pairings. No [independence](independent-random-variables.md) assumption between the coordinates is needed.

**Table of contents**

- [Gaussian even-moment pairing count](gaussian-even-moment-pairing-count.md)

## ↑ Ancestors (8)

1. [Multivariate Gaussian distribution](multivariate-gaussian-distribution.md)
2. [Normal distribution](normal-distribution.md)
3. [Probability distribution](probability-distribution.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
