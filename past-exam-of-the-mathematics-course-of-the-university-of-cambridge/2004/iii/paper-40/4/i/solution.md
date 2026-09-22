<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume the draws are [independent](../../../../../../independent-random-variables.md) from $g$, that the target-weighted integrand is covered by its support, and that $\int|\theta(x)|f(x)\,dx<\infty$. Define the [importance weight](../../../../../../importance-weight.md) $w(x)=f(x)/g(x)$. The change-of-density identity is

$$
\mathbb E_g[w(X)\theta(X)]=\int\frac{f(x)}{g(x)}\theta(x)g(x)\,dx
=\int\theta(x)f(x)\,dx=\mu.
$$

Therefore [importance sampling](../../../../../../importance-sampling.md) uses the unbiased estimator

$$
\boxed{\widehat\mu_g=\frac1n\sum_{i=1}^nw(x_i)\theta(x_i).}
$$

The [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) gives consistency. A finite [second moment](../../../../../../second-moment.md) of the weighted integrand additionally gives finite [variance](../../../../../../variance-split.md) and a usual independent-sample [central limit theorem](../../../../../../central-limit-theorem.md). A useful proposal places enough [probability](../../../../../../probability.md) where $f|\theta|$ is large and avoids tiny proposal [probability density function](../../../../../../probability-density-function.md) there; common support alone does not guarantee finite [variance](../../../../../../variance-split.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
