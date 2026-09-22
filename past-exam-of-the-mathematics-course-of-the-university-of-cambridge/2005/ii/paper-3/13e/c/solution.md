<h1 id="13e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At the deterministic feedback equilibrium use $\lambda_2m_1f(m_2)=\beta_2m_2$. The indicated elasticity is

$$
H_{22}=1-\frac{\partial\log f}{\partial\log x_2}=1+h=:H.
$$

The normalized drift becomes $A=\begin{pmatrix}-\beta_1&0\\\beta_2&-\beta_2H\end{pmatrix}$; equal mean birth and death rates still give $D=\operatorname{diag}(2\beta_1/m_1,2\beta_2/m_2)$. Solving the same [covariance](../../../../../../covariance.md) equation yields the [feedback attenuation of gene-expression noise](../../../../../../feedback-attenuation-of-gene-expression-noise.md):

$$
\boxed{\eta_{22}\simeq\frac1{Hm_2}+\frac{\beta_2}{H(\beta_1+\beta_2H)m_1}.}
$$

For $f(x_2)=k/x_2$, $h=1,H=2$, so

$$
\boxed{m_2\simeq\sqrt{\lambda_2km_1/\beta_2},\qquad \eta_{22}\simeq\frac1{2m_2}+\frac{\beta_2}{2(\beta_1+2\beta_2)m_1}.}
$$

The inverse-feedback expression is interpreted near a positive equilibrium; a microscopic birth rate singular at zero needs a separate regularization there.

## ↑ Ancestors (11)

1. [C](../c.md)
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
