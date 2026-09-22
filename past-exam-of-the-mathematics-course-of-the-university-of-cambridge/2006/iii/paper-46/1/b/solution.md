<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take the coordinate-selection matrix

$$
A=\begin{pmatrix}I_q\\0_{(p-q)\times q}\end{pmatrix}.
$$

Then $A^TX=X_1$, $A^T\mu=\mu_1$ and $A^T\Sigma A=\Sigma_{11}$. The permitted result on a [linear image of a multivariate normal vector](../../../../../../linear-image-of-a-multivariate-normal-vector.md) therefore gives

$$
\boxed{X_1\sim N_q(\mu_1,\Sigma_{11}).}
$$

This is the [marginal distribution](../../../../../../marginal-distribution.md) obtained by discarding the other coordinates. The conclusion holds also for a positive-semidefinite marginal covariance: in that case the Gaussian law may be degenerate and need not have a full-dimensional density. If the original covariance is positive definite, its principal block $\Sigma_{11}$ is positive definite as well.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
