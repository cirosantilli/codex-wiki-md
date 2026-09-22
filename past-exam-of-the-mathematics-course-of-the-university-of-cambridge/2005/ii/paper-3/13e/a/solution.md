<h1 id="13e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $m_i=\langle x_i\rangle$. The mean equations give $m_1=\lambda_1/\beta_1$ and $m_2=\lambda_2m_1/\beta_2$. For relative deviations, the drift Jacobian and normalized reaction-noise [covariance](../../../../../../covariance.md) are

$$
A=\begin{pmatrix}-\beta_1&0\\\beta_2&-\beta_2\end{pmatrix},\qquad D=\operatorname{diag}(2\beta_1/m_1,2\beta_2/m_2).
$$

The [normalized stationary fluctuation-dissipation relation for a reaction network](../../../../../../normalized-stationary-fluctuation-dissipation-relation-for-a-reaction-network.md) is $A\eta+\eta A^T+D=0$ with this negative-drift convention. Its entries successively give

$$
\boxed{\eta_{11}=\frac1{m_1},\qquad \eta_{12}=\frac{\beta_2}{\beta_1+\beta_2}\frac1{m_1},\qquad
\eta_{22}=\frac1{m_2}+\frac{\beta_2}{\beta_1+\beta_2}\frac1{m_1}.}
$$

The birth and death channels act on one species at a time, so the diffusion [matrix](../../../../../../matrix.md) is diagonal even though the stationary [covariance](../../../../../../covariance.md) is not.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [13E](../../13e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
