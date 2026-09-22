<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

Write the countable supports as $D_i$ and the marginal masses as $p_i(x_i)$. [Independence](../../../../../independent-random-variables.md) gives joint mass $\prod_ip_i(x_i)$. Assuming finite [expected values](../../../../../expected-value.md), absolute integrability is justified by [Tonelli theorem](../../../../../tonelli-theorem.md):

$$
\mathbb E\left[\prod_i|X_i|\right]=\sum_{x_1\in D_1,\ldots,x_n\in D_n}\prod_i|x_i|p_i(x_i)=\prod_i\mathbb E|X_i|<\infty.
$$

Consequently [Fubini's theorem](../../../../../fubini-s-theorem.md) permits factorization of the signed sum, proving the [expectation of a product of independent random variables](../../../../../expectation-of-a-product-of-independent-random-variables.md):

$$
\boxed{\mathbb E\left[\prod_iX_i\right]=\prod_i\mathbb E[X_i].}
$$

The second claim holds as a general assertion with the additional hypothesis that **the positive variables are integer-valued**. For a nonnegative integer-valued $Z$, the pointwise identity $Z=\sum_{m\ge0}\mathbf1_{\{Z>m\}}$ and [Tonelli theorem](../../../../../tonelli-theorem.md) give the [tail-sum formula](../../../../../tail-sum-formula.md)

$$
\mathbb E[Z]=\sum_{m=0}^\infty\mathbb P(Z>m).
$$

If each $X_i$ is integer-valued, their product is too. Apply this identity to each factor and to the product, then use [independence](../../../../../independent-random-variables.md):

$$
\boxed{\prod_i\sum_{m\ge0}\mathbb P(X_i>m)=\prod_i\mathbb E[X_i]=\mathbb E\left[\prod_iX_i\right]=\sum_{m\ge0}\mathbb P\left(\prod_iX_i>m\right).}
$$

Under the literal broader meaning of a [discrete random variable](../../../../../discrete-random-variable.md), the second claim is false. Two independent constants $X_1=X_2=3/2$ are positive and discrete, but the left side is $2\cdot2=4$ and the right side is $3$. More generally the integer-indexed tail sum of a positive real-valued variable is $\mathbb E\lceil Z\rceil$, not $\mathbb E Z$. This is the [integer-valued hypothesis in the tail-sum formula](../../../../../integer-valued-hypothesis-in-the-tail-sum-formula.md).

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
