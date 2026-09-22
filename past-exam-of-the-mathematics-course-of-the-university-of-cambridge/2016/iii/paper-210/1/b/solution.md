<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Hoeffding lemma](../../../../../../hoeffding-lemma.md) for a [Bernoulli distribution](../../../../../../bernoulli-distribution.md) variable gives $\mathbb E e^{s(B-p)}\leq e^{s^2/8}$. Multiplication of the [moment-generating functions](../../../../../../moment-generating-function.md) of the [independent random variables](../../../../../../independent-random-variables.md) gives $\mathbb E e^{s(X-np)}\leq e^{ns^2/8}$. Thus the centered count is a [sub-Gaussian random variable](../../../../../../sub-gaussian-distribution.md) with variance proxy $n/4$. The [Chernoff bound](../../../../../../chernoff-bound.md), optimized at $s=4t/n$, gives

$$
\boxed{\mathbb P(X-np>t)\leq e^{-2t^2/n},\qquad t>0.}
$$

The same estimate holds for the lower tail by applying the [Chernoff bound](../../../../../../chernoff-bound.md) to $-(X-np)$. No [independence](../../../../../../independent-random-variables.md) between different bin counts is needed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 210](../../../paper-210-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
