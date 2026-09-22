<h1 id="2c/solution">Solution</h1>

↑ **Parent:** [2C](../2c.md)

Substituting the proposed form $\mathbf v(t)=e^{\lambda t}\mathbf u$ into the [linear system of ordinary differential equations](../../../../../linear-system-of-differential-equations.md) gives

$$
e^{\lambda t}(\lambda I-B)\mathbf u=e^{\lambda t}\mathbf x.
$$

If $\lambda$ is not an [eigenvalue](../../../../../eigenvalue.md) of $B$, the matrix $\lambda I-B$ is [invertible](../../../../../invertible-matrix.md), so

$$
\mathbf u=(\lambda I-B)^{-1}\mathbf x
$$

provides the required particular solution.

In the stated two-dimensional case,

$$
2I-B=\begin{pmatrix}2&-3\\-1&2\end{pmatrix},
\qquad
(2I-B)^{-1}=\begin{pmatrix}2&3\\1&2\end{pmatrix},
$$

and therefore $\mathbf u=(3,2)^T$. The [eigenvalues](../../../../../eigenvalue.md) of $B$ are $\pm\sqrt3$, with corresponding [eigenvectors](../../../../../eigenvector.md) $(\sqrt3,1)^T$ and $(-\sqrt3,1)^T$. Adding the [general solution](../../../../../general-solution.md) of the homogeneous system yields

$$
\boxed{
\mathbf v(t)=e^{2t}\begin{pmatrix}3\\2\end{pmatrix}
+C_+e^{\sqrt3t}\begin{pmatrix}\sqrt3\\1\end{pmatrix}
+C_-e^{-\sqrt3t}\begin{pmatrix}-\sqrt3\\1\end{pmatrix}}.
$$

## ↑ Ancestors (10)

1. [2C](../2c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
