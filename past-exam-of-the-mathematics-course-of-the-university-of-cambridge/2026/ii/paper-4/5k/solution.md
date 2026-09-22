<h1 id="5k/solution">Solution</h1>

↑ **Parent:** [5K](../5k.md)

Write $f(y;\theta)=\exp\{y\theta-b(\theta)+c(y)\}$ and use canonical parameter $\theta_i=X_i^T\beta$. Then

$$
\ell(\beta)=\sum_i[Y_iX_i^T\beta-b(X_i^T\beta)+c(Y_i)],\quad X^T(Y-\mu)=0,
$$

where $\mu_i=b'(X_i^T\beta)$. Geometrically the residual [vector](../../../../../vector.md) is orthogonal to every design column. For $H_0:\beta_1=0$, use a two-sided Wald statistic $\hat\beta_1/\operatorname{se}(\hat\beta_1)$ (or likelihood-ratio statistic), rejecting at the corresponding normal or chi-square critical value.

## ↑ Ancestors (10)

1. [5K](../5k.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
