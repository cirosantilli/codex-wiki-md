<h1 id="13c/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Comparison with the [multivariate normal density](../../../../../../multivariate-normal-density.md) shows that $D$ is its [precision matrix](../../../../../../precision-matrix.md). Since the mean is zero,

$$
\boxed{C_{ij}=\langle x_ix_j\rangle=(D^{-1})_{ij}.}
$$

Multiplying $a+\frac12bD=0$ on the right by $C=D^{-1}$ gives $aC=-b/2$. Taking the transpose and using the symmetry of $b$ and $C$ gives $Ca^T=-b/2$. Hence the stationary covariance obeys the [Continuous Lyapunov equation](../../../../../../continuous-lyapunov-equation.md)

$$
\boxed{aC+Ca^T+b=0.}
$$

The same equation follows directly by setting the time derivative of the second-moment equation from part (c) to zero.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [13C](../../13c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
