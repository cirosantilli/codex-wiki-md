<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [proper gamma approximation to a Poisson Jeffreys prior](../../../../../../proper-gamma-approximation-to-a-poisson-jeffreys-prior.md) uses shape $1/2$ and a small positive rate $\varepsilon$:

$$
\boxed{\lambda_i\sim\operatorname{Gamma}(1/2,\varepsilon),\qquad\varepsilon>0\ \text{small}.}
$$

Its density is proportional to $\lambda_i^{-1/2}e^{-\varepsilon\lambda_i}$, so where $\varepsilon\lambda_i$ is small its kernel approximates the [Jeffreys prior](../../../../../../jeffreys-prior.md). After observing the data, [Poisson-gamma conjugacy](../../../../../../poisson-gamma-conjugacy.md) gives $\operatorname{Gamma}(y_i+1/2,E_i+\varepsilon)$, which converges to the preceding [posterior distribution](../../../../../../bayesian-posterior.md) as $\varepsilon\downarrow0$. This is an approximation of an improper kernel on the relevant parameter range, not a weak limit to a normalized Jeffreys probability distribution. The shape must be $1/2$; a small-shape gamma prior would approximate a different power of $\lambda_i$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
