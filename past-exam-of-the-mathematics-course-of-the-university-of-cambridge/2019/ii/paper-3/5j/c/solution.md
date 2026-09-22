<h1 id="5j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [canonical link function](../../../../../../canonical-link-function.md), $\theta_i=\eta_i=x_i^T\beta$. Differentiating the log-likelihood gives the [score function](../../../../../../informant-function.md)

$$
\nabla_\beta\ell(\beta)=\sigma^{-2}X^T(y-\mu).
$$

Since

$$
\frac{d\mu_i}{d\eta_i}=b''(\theta_i)=V(\mu_i),
$$

where $V$ is the [variance function](../../../../../../variance-function.md), a second differentiation gives

$$
\nabla_\beta^2\ell(\beta)
=-\sigma^{-2}X^T
\operatorname{diag}\bigl(V(\mu_1),\ldots,V(\mu_n)\bigr)X.
$$

This Hessian does not depend on the observed $y$, so taking its negative expectation changes nothing. Hence

$$
\boxed{\mathcal I(\beta)=\sigma^{-2}X^TWX,
\qquad W=\operatorname{diag}\bigl(V(\mu_1),\ldots,V(\mu_n)\bigr).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5J](../../5j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
