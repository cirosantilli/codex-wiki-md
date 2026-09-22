<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The empirical [kernel covariance operator](../../../../../../kernel-covariance-operator.md) $\Sigma$ is self-adjoint and positive semidefinite. Maximize $\langle u,\Sigma u\rangle$ subject to $\langle u,u\rangle=1$. The first variation of the [Lagrange multiplier](../../../../../../lagrange-multiplier.md) functional gives

$$
2\Sigma v-2\lambda v=0,
$$

so $\Sigma v=\lambda v$. Taking the inner product with $v$ gives

$$
\boxed{\lambda=\langle v,\Sigma v\rangle
=\frac1n\sum_{i=1}^n|\langle v,\phi(x_i)\rangle|^2\geq0.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
