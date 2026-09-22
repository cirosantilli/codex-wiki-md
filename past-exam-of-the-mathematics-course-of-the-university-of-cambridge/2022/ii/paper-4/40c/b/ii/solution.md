<h1 id="40c/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $L_h$ be the spatial matrix, so the [Forward Euler method](../../../../../../../euler-method.md) is

$$
U^{n+1}=(I+kL_h)U^n.
$$

The conservative use of shared edge coefficients makes $L_h$ a real symmetric matrix. In an interior row, put $s=\alpha+\beta+\gamma+\delta<4a_{\max}$. Its diagonal entry is $-s/h^2$, and the sum of the absolute off-diagonal entries is $s/h^2$. Boundary rows have no larger disk because homogeneous [Dirichlet data](../../../../../../../dirichlet-boundary-condition.md) remove some unknown neighbors.

The [Gershgorin circle theorem](../../../../../../../gershgorin-circle-theorem.md) and symmetry therefore place every eigenvalue of $L_h$ in

$$
\left[-\frac{2s}{h^2},0\right]
\subseteq
\left[-\frac{8a_{\max}}{h^2},0\right].
$$

If $\mu=k/h^2$, each amplification eigenvalue is $1+k\lambda$. It lies in $[-1,1]$ whenever

$$
1-8\mu a_{\max}\geq-1,
$$

or

$$
\boxed{0<\mu\leq\frac1{4a_{\max}}}.
$$

Since the amplification matrix is symmetric, bounding all its eigenvalues in modulus by one bounds its discrete Euclidean operator norm by one. This proves the stated stability condition and is the [Gershgorin stability bound for a variable-coefficient diffusion stencil](../../../../../../../gershgorin-stability-bound-for-a-variable-coefficient-diffusion-stencil.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [40C](../../../40c.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
