<h1 id="2b/solution">Solution</h1>

↑ **Parent:** [2B](../2b.md)

Substituting an exponential particular solution gives $\lambda u-Au=v$, or $(\lambda I-A)u=v$. Since $\lambda$ is not an [eigenvalue](../../../../../eigenvalue.md) of $A$, the matrix is invertible. The [exponential forcing of a constant-coefficient differential system](../../../../../exponential-forcing-of-a-constant-coefficient-differential-system.md) therefore has

$$
\boxed{x_p(t)=e^{\lambda t}(\lambda I-A)^{-1}v.}
$$

For the specified matrix, $I-A=\begin{pmatrix}1&-1\\0&1\end{pmatrix}$. Solving $u_2=1$, $u_1-u_2=1$ gives $u=(2,1)^T$, so

$$
\boxed{x_p(t)=e^t\begin{pmatrix}2\\1\end{pmatrix}.}
$$

Differentiation verifies both component equations directly. If a general solution were desired, the homogeneous term $e^{tA}c$ would be added, with the [matrix exponential](../../../../../matrix-exponential.md) here equal to $I+tA$ because $A^2=0$.

## ↑ Ancestors (10)

1. [2B](../2b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
