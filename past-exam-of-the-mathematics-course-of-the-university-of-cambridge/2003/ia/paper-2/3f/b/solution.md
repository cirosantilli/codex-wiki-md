<h1 id="3f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For [independent random variables](../../../../../../independent-random-variables.md), their sum has the product of their [probability generating functions](../../../../../../probability-generating-function.md):

$$
G_{X+Y}(z)=\mathbb E[z^Xz^Y]=G_X(z)G_Y(z)=(1-p+pz)^{n+m}.
$$

Comparing polynomial coefficients identifies a [binomial distribution](../../../../../../binomial-distribution.md) with parameters $n+m,p$:

$$
\boxed{\mathbb P(X+Y=k)=\binom{n+m}{k}p^k(1-p)^{n+m-k},\qquad k=0,\ldots,n+m,}
$$

and the [probability](../../../../../../probability.md) is zero at all other values. The common success [probability](../../../../../../probability.md) is essential to this binomial form; independent binomial counts with different [probabilities](../../../../../../probability.md) do not in general add to a binomial count.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3F](../../3f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
