<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the infinite translation-invariant chain first. Set $\rho=e^{-\kappa}$ and Fourier-transform the exchange [matrix](../../../../../../matrix.md):

$$
\mathsf J(q)=J\sum_{n\in\mathbb Z}\rho^{|n|}e^{-iqn}
=J\left(1+\frac{\rho e^{iq}}{1-\rho e^{iq}}+\frac{\rho e^{-iq}}{1-\rho e^{-iq}}\right)
=\frac{J(1-\rho^2)}{1-2\rho\cos q+\rho^2}
=\frac{J\sinh\kappa}{\cosh\kappa-\cos q}.
$$

For positive $J,\kappa$ this is strictly positive. Its reciprocal is a linear polynomial in $\cos q$, proving the nearest-neighbour form of the [exponentially coupled Ising inverse kernel](../../../../../../exponentially-coupled-ising-inverse-kernel.md):

$$
[\mathsf J^{-1}]_{ij}=\frac{\cosh\kappa}{J\sinh\kappa}\delta_{ij}
-\frac{\delta_{i,j+1}+\delta_{i,j-1}}{2J\sinh\kappa}.
$$

Expanding the squared difference gives

$$
m^T\mathsf J^{-1}m
=\sum_j\left[\frac{(m_j-m_{j+1})^2}{2J\sinh\kappa}
+\frac{\cosh\kappa-1}{J\sinh\kappa}m_j^2\right].
$$

Since $(\cosh\kappa-1)/\sinh\kappa=\tanh(\kappa/2)$, substitution into part (a) yields

$$
\boxed{Z=C\int\prod_jdm_j\,
\exp\left[-\sum_j\left\{\frac{(m_j-m_{j+1})^2}{2J\sinh\kappa}+U(m_j)\right\}\right],
\qquad U(m)=\frac{\tanh(\kappa/2)}Jm^2-\log[2\cosh(2m+h)].}
$$

This is the exact bulk identity. A finite periodic version uses the periodized coupling $J_{ij}=J\sum_{\ell\in\mathbb Z}e^{-\kappa|i-j+\ell N|}$; its discrete Fourier symbols are the same and the squared differences wrap around the ring. Simply truncating the exponential at open ends gives a different inverse at those ends.

For an open chain of $N\ge2$ sites with the literal finite matrix $J\rho^{|i-j|}$, the [open-chain endpoint corrections for an exponential Ising kernel](../../../../../../open-chain-endpoint-corrections-for-an-exponential-ising-kernel.md) are explicit:

$$
m^T\mathsf J_N^{-1}m
=\frac1{2J\sinh\kappa}\sum_{j=1}^{N-1}(m_{j+1}-m_j)^2
+\frac{\tanh(\kappa/2)}J\sum_{j=1}^Nm_j^2
+\frac{\rho}{J(1+\rho)}(m_1^2+m_N^2).
$$

The inverse has endpoint diagonal entries $1/[J(1-\rho^2)]$, interior diagonal entries $(1+\rho^2)/[J(1-\rho^2)]$ and adjacent entries $-\rho/[J(1-\rho^2)]$. Multiplication by the original geometric matrix verifies every entry. These boundary terms affect boundary amplitudes, but not the bulk [free-energy density](../../../../../../free-energy-density.md) in the [thermodynamic limit](../../../../../../thermodynamic-limit.md) at fixed $\kappa>0$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
