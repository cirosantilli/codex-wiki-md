<h1 id="9a/solution">Solution</h1>

↑ **Parent:** [9A](../9a.md)

Varying the [Lagrangian](../../../../../lagrangian.md) gives, with the cyclic angle conventions,

$$
\boxed{m_i a^2\ddot\theta_i=k(\theta_{i+1}-2\theta_i+\theta_{i-1}).}
$$

All successive angular gaps are $2\pi/N$ in equilibrium, so their two contributions cancel. Because the potential depends only on gaps, a uniform change of all angles costs no energy. Its Hessian therefore annihilates $(1,\ldots,1)$, giving a zero-frequency [normal mode](../../../../../normal-mode.md). The corresponding motion is rigid rotation, $\theta_i(t)=\theta_i^{(0)}+A+Bt$, including a constant common angular shift.

For two particles write $\theta_2-\theta_1=\pi+\delta_2-\delta_1$. Both cyclic gaps contribute, so the quadratic potential is $k(\delta_2-\delta_1)^2$. With the specified masses, the mass matrix is $km\operatorname{diag}(1,2)$ and the stiffness matrix is $2k\left(\begin{smallmatrix}1&-1\\-1&1\end{smallmatrix}\right)$. The [generalized eigenvalue problem](../../../../../generalized-eigenvalue-problem.md) gives

$$
\boxed{\omega_0=0,\quad(\delta_1,\delta_2)\propto(1,1);\qquad \omega_1=\sqrt{3/m},\quad(\delta_1,\delta_2)\propto(2,-1).}
$$

The finite-frequency [normal mode](../../../../../normal-mode.md) keeps the mass-weighted mean angle fixed and changes the angular separation sinusoidally. Together with the two rigid-rotation constants, it spans all small motions about equilibrium.

## ↑ Ancestors (10)

1. [9A](../9a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
