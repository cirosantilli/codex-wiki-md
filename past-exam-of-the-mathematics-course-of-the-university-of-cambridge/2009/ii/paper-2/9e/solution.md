<h1 id="9e/solution">Solution</h1>

↑ **Parent:** [9E](../9e.md)

For $q=(x_1,\eta_1,\eta_2)^T$, the [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) give

$$
m\ddot q+\mu Kq=0,\qquad K=\begin{pmatrix}19/3&-1&0\\-1&2&-1\\0&-1&1\end{pmatrix}.
$$

In components these are $m\ddot x_1=-\mu(19x_1/3-\eta_1)$, $m\ddot\eta_1=-\mu(2\eta_1-x_1-\eta_2)$ and $m\ddot\eta_2=-\mu(\eta_2-\eta_1)$. A [normal mode](../../../../../normal-mode.md) has $q=v\cos(\omega t+\delta)$ and satisfies $Kv=(m\omega^2/\mu)v$. For [eigenvalue](../../../../../eigenvalue.md) $1/3$, the first and third rows give $\eta_1=6x_1$ and $\eta_2=3\eta_1/2$, and the second row then agrees. Hence

$$
\boxed{q=C(1,6,9)^T\cos\left(\sqrt{\frac\mu{3m}}t+\delta\right),\qquad P=2\pi\sqrt{\frac{3m}{\mu}}.}
$$

The particle positions are recovered by adding the equilibrium offsets to the last two entries. Their displacements are in phase with amplitude ratio $1:6:9$.

## ↑ Ancestors (10)

1. [9E](../9e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
