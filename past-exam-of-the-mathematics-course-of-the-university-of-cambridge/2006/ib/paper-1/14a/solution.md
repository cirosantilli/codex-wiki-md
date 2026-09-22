<h1 id="14a/solution">Solution</h1>

↑ **Parent:** [14A](../14a.md)

In orthonormal Cartesian coordinates, a second-rank [tensor](../../../../../tensor.md) has components transforming under a change of axes $Q$ as $M'_{ij}=Q_{ik}Q_{j\ell}M_{k\ell}$, where $QQ^T=I$. Its contraction is invariant:

$$
M'_{ii}=Q_{ik}Q_{i\ell}M_{k\ell}=\delta_{k\ell}M_{k\ell}=M_{kk}.
$$

Thus **$M_{ii}$ is a scalar**. This is [tensor contraction](../../../../../tensor-contraction.md) with the [Euclidean metric](../../../../../euclidean-metric.md). In general nonorthonormal coordinates the invariant expression is $g^{ij}M_{ij}$, not an unweighted sum of diagonal covariant components.

For the planar plate, every mass element has $z=0$. The [inertia tensor](../../../../../inertia-tensor.md) is consequently

$$
M=\begin{pmatrix}
\int_Dy^2\rho\,dS&-\int_Dxy\rho\,dS&0\\
-\int_Dxy\rho\,dS&\int_Dx^2\rho\,dS&0\\
0&0&\int_D(x^2+y^2)\rho\,dS
\end{pmatrix}.
$$

It follows directly that $\mathbf e_z$ is an [eigenvector](../../../../../eigenvector.md) and

$$
\boxed{M_\perp=\int_D(x^2+y^2)\rho\,dS.}
$$

The real [symmetric matrix](../../../../../symmetric-matrix.md) has three real [eigenvalues](../../../../../eigenvalue.md). Its [trace](../../../../../matrix-trace.md) is $2\int_D(x^2+y^2)\rho\,dS=2M_\perp$, so $M_1+M_2+M_\perp=2M_\perp$. Hence the [perpendicular axis theorem](../../../../../perpendicular-axis-theorem.md) gives **$M_\perp=M_1+M_2$**.

For a disc of constant areal [density](../../../../../density.md) $\rho_0$, symmetry gives $\int_Dxy\,dS=0$, and polar integration gives $\int_Dx^2\,dS=\int_Dy^2\,dS=\pi a^4/4$. Therefore

$$
\boxed{M=\frac{\pi\rho_0a^4}{4}\operatorname{diag}(1,1,2)
=\frac{Ma^2}{4}\operatorname{diag}(1,1,2),\qquad M=\pi\rho_0a^2,}
$$

where the scalar $M$ in the last expression denotes the total mass rather than the [tensor](../../../../../tensor.md).

## ↑ Ancestors (10)

1. [14A](../14a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
