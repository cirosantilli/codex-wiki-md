<h1 id="27k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The part of the [log-likelihood](../../../../../../log-likelihood.md) depending on $\theta$ is

$$
\ell(\theta)=-\frac12\sum_{i=1}^n(X_i-\theta)^T\Sigma^{-1}(X_i-\theta)+\text{constant}.
$$

[Completing the square](../../../../../../completing-the-square.md) separates the sum into a term independent of $\theta$ and $n(\overline X-\theta)^T\Sigma^{-1}(\overline X-\theta)$. Positive definiteness makes its unique minimum occur at $\overline X$. Since linear combinations of independent [multivariate normal](../../../../../../multivariate-normal-distribution.md) vectors are normal,

$$
\boxed{\widehat\theta_n=\overline X,\qquad\widehat\theta_n\sim\mathcal N_d(\theta,\Sigma/n).}
$$

The [Hessian matrix](../../../../../../hessian-matrix.md) $-n\Sigma^{-1}$ is negative definite, confirming the global likelihood maximum.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [27K](../../27k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
