<h1 id="7d/solution">Solution</h1>

↑ **Parent:** [7D](../7d.md)

For the [homogeneous solution](../../../../../homogeneous-solution.md), expand in the independent [eigenvectors](../../../../../eigenvector.md) of $A$. Each coefficient obeys $c_j'=\lambda_jc_j$, so the [complementary function](../../../../../homogeneous-solution.md) is

$$
\boxed{\mathbf x_c(t)=\sum_{j=1}^nC_j\mathbf a_j e^{\lambda_jt}.}
$$

If $\mathbf x_p$ is any [particular integral](../../../../../particular-solution.md), subtracting it from any other solution gives a [homogeneous solution](../../../../../homogeneous-solution.md). Hence $\mathbf x=\mathbf x_p+\mathbf x_c$ is the [general solution](../../../../../general-solution.md). Complex-conjugate modes can be combined to produce real solutions when the forcing is real.

For a real two-by-two matrix, the characteristic polynomial is $\lambda^2-(\operatorname{tr}A)\lambda+\det A$. Under the stated distinct-eigenvalue assumption, all nonzero homogeneous modes are purely oscillatory exactly when the [eigenvalues](../../../../../eigenvalue.md) are $\pm i\omega$ with $\omega>0$. Their sum and product imply $\operatorname{tr}A=0$, $\det A=\omega^2>0$. Conversely these [trace](../../../../../matrix-trace.md) and [determinant](../../../../../determinant.md) conditions force those [eigenvalues](../../../../../eigenvalue.md), so there is no exponential growth, decay or Jordan-block secular growth.

For the final specified initial-value problem, direct multiplication gives $A^2=-9I$. The forcing vector $\mathbf b=(2,3i-1)^T$ satisfies $A\mathbf b=3i\mathbf b$, so the forcing is resonant and $t\mathbf b e^{3it}$ is a [particular integral](../../../../../particular-solution.md). The [matrix exponential](../../../../../matrix-exponential.md) is

$$
e^{At}=I\cos3t+\frac A3\sin3t.
$$

Since the resonant [particular integral](../../../../../particular-solution.md) vanishes initially, the initial-value solution is

$$
\boxed{\mathbf x(t)=
\begin{pmatrix}\cos3t+\tfrac13\sin3t\\-\tfrac53\sin3t\end{pmatrix}
+t e^{3it}\begin{pmatrix}2\\3i-1\end{pmatrix}.}
$$

This complex solution is appropriate to the complex forcing as written. Taking real parts gives the corresponding solution for the real part of that forcing.

## ↑ Ancestors (10)

1. [7D](../7d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
