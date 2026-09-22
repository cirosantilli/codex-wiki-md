<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [control variate](../../../../../../control-variates.md) is a random variable $C$ correlated with the estimator and with known mean $c_0$. For a fixed real coefficient $a$, define $Y_a=Y-a(C-c_0)$. Then $\mathbb EY_a=\theta$, while

$$
\operatorname{Var}(Y_a)=\operatorname{Var}(Y)-2a\operatorname{Cov}(Y,C)+a^2\operatorname{Var}(C).
$$

Assuming finite second moments and positive control [variance](../../../../../../variance-split.md), complete the square to find

$$
\boxed{a_* =\frac{\operatorname{Cov}(Y,C)}{\operatorname{Var}(C)},\qquad
\min_a\operatorname{Var}(Y_a)=\operatorname{Var}(Y)-\frac{\operatorname{Cov}(Y,C)^2}{\operatorname{Var}(C)}.}
$$

When $\operatorname{Var}(Y)>0$, the minimum is $\operatorname{Var}(Y)(1-\rho_{Y,C}^2)$. A constant control cannot reduce [variance](../../../../../../variance-split.md). A strongly correlated control, including a negatively correlated one with a negative coefficient, can substantially reduce it.

For [multivariate control variates](../../../../../../multivariate-control-variates.md), write $Y_\beta=Y-\beta^T(C-\mathbb EC)$, $\Sigma=\operatorname{Cov}(C)$ and $c=\operatorname{Cov}(C,Y)$. Completing the multivariate square gives

$$
\boxed{\beta_* =\Sigma^{-1}c,\qquad
\min_\beta\operatorname{Var}(Y_\beta)=\operatorname{Var}(Y)-c^T\Sigma^{-1}c.}
$$

If $\Sigma$ is singular, use its [Moore-Penrose inverse](../../../../../../moore-penrose-inverse.md). Indeed any null direction has a constant centered control combination and therefore zero [covariance](../../../../../../covariance.md) with $Y$, so $c$ lies in the range of $\Sigma$. The elementary unbiasedness statement assumes a deterministic coefficient; estimating it from the same simulation may introduce finite-sample bias, whereas an independently trained coefficient keeps the conditional unbiasedness argument valid.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
