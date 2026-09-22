<h1 id="4j/solution">Solution</h1>

↑ **Parent:** [4J](../4j.md)

The standard normal [distribution function](../../../../../cumulative-distribution-function.md) $\Phi$ gives

$$
P(Z_i=1\mid x_i)=P(\epsilon_i>\log c-\mu-x_i^T\beta)
=\Phi\!\left(\frac{\mu-\log c}{\sigma}+x_i^T\frac\beta\sigma\right).
$$

The observations are independent [Bernoulli random variables](../../../../../bernoulli-distribution.md), because the original errors are independent. Thus the [probit regression](../../../../../probit-model.md) has intercept $\alpha=(\mu-\log c)/\sigma$ and coefficient vector $\gamma=\beta/\sigma$. With the specified known $\sigma$ and $c$, recovery is

$$
\boxed{\mu=\log c+\sigma\alpha,\qquad\beta=\sigma\gamma}.
$$

The scale would not be recoverable from threshold data alone if $\sigma$ were unknown.

## ↑ Ancestors (10)

1. [4J](../4j.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
