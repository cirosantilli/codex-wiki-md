<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

Write $\ell(\beta)$ for the [log-likelihood](../../../../../log-likelihood.md) and $U=\nabla\ell$ for the [score function](../../../../../informant-function.md). [Newton method](../../../../../newton-s-method-in-optimization.md) uses the [Observed Fisher information](../../../../../observed-fisher-information.md) $M=-\nabla^2\ell$; [Fisher scoring](../../../../../scoring-algorithm.md) uses the [Fisher information](../../../../../fisher-information-matrix.md) $M=\mathbb E_\beta[-\nabla^2\ell]$.

For independent responses in an [exponential family](../../../../../exponential-family-split.md), with fixed [dispersion parameter](../../../../../dispersion-parameter.md) and fixed weights $a_i$, a [canonical link function](../../../../../canonical-link-function.md) gives $\theta_i=x_i^T\beta$ and

$$
 \ell(\beta)=\sum_i\frac{y_i\theta_i-b(\theta_i)}{a_i}+\sum_i c_i(y_i),\qquad
 U=\sum_i\frac{x_i(y_i-b'(\theta_i))}{a_i},\qquad
 -\nabla^2\ell=\sum_i\frac{b''(\theta_i)}{a_i}x_ix_i^T.
$$

The last [matrix](../../../../../matrix.md) depends on $\beta$ but not on the responses, so taking its [expectation](../../../../../expected-value.md) leaves it unchanged. Hence **the two updates are identical**, wherever this [Fisher information matrix](../../../../../fisher-information-matrix.md) is invertible. Equivalently both solve the same [iteratively reweighted least squares](../../../../../iteratively-reweighted-least-squares.md) problem. This statement concerns the regression coefficients at a fixed [dispersion parameter](../../../../../dispersion-parameter.md); a joint update of an unknown [dispersion parameter](../../../../../dispersion-parameter.md) need not have identical observed and expected full [Fisher information matrices](../../../../../fisher-information-matrix.md).

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
