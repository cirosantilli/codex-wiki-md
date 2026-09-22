<h1 id="17h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Ignoring terms independent of $\theta$, the [log-likelihood](../../../../../../log-likelihood.md) is

$$
\ell(\theta)
=\sum_i\bigl(Y_i\log\theta-\theta x_i\bigr)+\text{constant}.
$$

Its [score function](../../../../../../informant-function.md) is

$$
\ell'(\theta)=\frac{\sum_iY_i}{\theta}-\sum_i x_i.
$$

Since $\ell''(\theta)=-(\sum_iY_i)/\theta^2\leq0$, the interior critical point is the maximum, giving

$$
\boxed{\widehat\theta_{MLE}
=\frac{\sum_iY_i}{\sum_i x_i}}.
$$

The sum of independent [Poisson distributions](../../../../../../poisson-distribution.md) is Poisson with mean $\theta\sum_i x_i$, so

$$
\mathbb E\widehat\theta_{MLE}=\theta.
$$

**Thus the [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) is also unbiased.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17H](../../17h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
