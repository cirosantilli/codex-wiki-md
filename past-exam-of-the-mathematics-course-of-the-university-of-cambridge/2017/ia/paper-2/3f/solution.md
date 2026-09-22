<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

Because $X$ is a nonnegative integer, its [indicator function](../../../../../indicator-function.md) satisfies $\mathbf1_{\{X>0\}}\leq X$. Taking [expected values](../../../../../expected-value.md) proves the upper bound. The finite [second moment](../../../../../second-moment.md) also gives a finite [expected value](../../../../../expected-value.md), by the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md). Applying that inequality to $X$ and $\mathbf1_{\{X>0\}}$ gives

$$
(\mathbb EX)^2
=\bigl(\mathbb E[X\mathbf1_{\{X>0\}}]\bigr)^2
\leq\mathbb E[X^2]\,\mathbb P(X>0).
$$

The assumed positive [second moment](../../../../../second-moment.md) permits division, yielding

$$
\boxed{\frac{(\mathbb EX)^2}{\mathbb E[X^2]}\leq\mathbb P(X>0)\leq\mathbb EX.}
$$

The lower bound is the basic [second moment method](../../../../../second-moment-method.md); the upper bound also follows from [Markov's inequality](../../../../../markov-inequality.md) at threshold one. Integer-valuedness is essential for that upper bound, but not for the lower bound. For example, a constant $X=1/2$ would violate the upper bound.

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
