<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Work first on the infinite chain, or with a periodized exponential kernel. Put $\rho=e^{-\kappa}$ and use lattice Fourier momentum $q\in[-\pi,\pi]$. Summing the geometric series gives the [exponentially coupled Ising inverse kernel](../../../../../../exponentially-coupled-ising-inverse-kernel.md):

$$
J(q)=J\sum_{n\in\mathbb Z}\rho^{|n|}e^{iqn}
=J\frac{1-\rho^2}{1-2\rho\cos q+\rho^2}
=\frac{J\sinh\kappa}{\cosh\kappa-\cos q}>0.
$$

Thus

$$
J^{-1}(q)=\frac{\cosh\kappa-\cos q}{J\sinh\kappa}
=\frac{\tanh(\kappa/2)}J+\frac{1-\cos q}{J\sinh\kappa}.
$$

Although the original kernel is long-ranged, its inverse contains only a constant and a cosine and therefore is nearest-neighbor. Fourier orthogonality gives

$$
\sum_{ij}m_i[\mathsf J^{-1}]_{ij}m_j
=\frac1{2J\sinh\kappa}\sum_j(m_j-m_{j+1})^2
+\frac{\tanh(\kappa/2)}J\sum_jm_j^2.
$$

Substitution into part (a) yields

$$
\boxed{\mathcal Z=C\int\prod_jdm_j\,e^{-\sum_j[(m_j-m_{j+1})^2/(2J\sinh\kappa)+U(m_j)]},\quad
U(m)=\frac{\tanh(\kappa/2)}Jm^2-\log[2\cosh(2m+h)].}
$$

This exact bulk identity does not require replacing $\sinh\kappa$ by $\kappa$; small $\kappa$ is used later to motivate a smooth continuum field.

For a finite open chain the inverse has off-diagonal entries $-\rho/[J(1-\rho^2)]$, interior diagonal entries $(1+\rho^2)/[J(1-\rho^2)]$ and endpoint diagonal entries $1/[J(1-\rho^2)]$. Accordingly the displayed homogeneous potential acquires the endpoint correction $\rho(m_1^2+m_N^2)/[J(1+\rho)]$. These boundary terms do not change the bulk thermodynamic conclusion. Stating infinite-chain or periodized [boundary conditions](../../../../../../boundary-condition.md) is necessary if the translation-invariant expression is asserted exactly.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
