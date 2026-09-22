<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Unbiasedness requires $\sum_i\alpha_i=1$. Let $S=\sum_i\sigma_i^{-2}$ and minimize $V(\alpha)=\sum_i\sigma_i^2\alpha_i^2$. The [Lagrange multiplier](../../../../../../lagrange-multiplier.md) equations for $V-\lambda(\sum_i\alpha_i-1)$ are $2\sigma_i^2\alpha_i=\lambda$, so normalization gives $\lambda=2/S$. Hence

$$
\boxed{\widehat\mu=\frac{\sum_i\sigma_i^{-2}\widehat\mu_i}{\sum_i\sigma_i^{-2}},\qquad\alpha_i=\frac{\sigma_i^{-2}}S,\qquad\operatorname{Var}(\widehat\mu)=S^{-1}}.
$$

The gradient at this point is $(2/S)\mathbf1$, whose inner product with every feasible displacement $h$ satisfying $\mathbf1^Th=0$ is zero. The [Hessian matrix](../../../../../../hessian-matrix.md) is $2\operatorname{diag}(\sigma_1^2,\ldots,\sigma_N^2)$, and $h^T\nabla^2Vh=2\sum_i\sigma_i^2h_i^2>0$ for every nonzero feasible $h$. These are the first- and second-order constrained minimum conditions. Strict convexity also proves global uniqueness of this [inverse-variance weighted mean](../../../../../../inverse-variance-weighted-mean.md); normal errors are not needed.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
