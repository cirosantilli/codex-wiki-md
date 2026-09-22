<h1 id="7d/solution">Solution</h1>

↑ **Parent:** [7D](../7d.md)

Allow an [eigenvector](../../../../../eigenvector.md) $v\ne0$ to have complex entries, since real matrices can initially have complex [eigenvalues](../../../../../eigenvalue.md). Write $v^*$ for its conjugate transpose. Reality of $A$ gives $A^*=A^T$; symmetry then gives $A^*=A$. Thus $A$ is a [Hermitian matrix](../../../../../hermitian-operator.md). The scalar $v^*Av$ equals its complex conjugate, because $(v^*Av)^*=v^*A^*v=v^*Av$. If $Av=\lambda v$, then

$$
\lambda=\frac{v^*Av}{v^*v}\in\mathbb R,
$$

since $v^*v>0$. This proves that all [eigenvalues](../../../../../eigenvalue.md) are real. The equality $A^*=A^T$ is precisely where reality was used; a complex symmetric matrix need not be Hermitian, as $iI$ illustrates.

If $Au=\lambda u$ and $Av=\mu v$, then $u^*Av=\mu u^*v$, but also $u^*Av=(Au)^*v=\overline\lambda u^*v=\lambda u^*v$. Consequently $(\mu-\lambda)u^*v=0$. Distinct [eigenvalues](../../../../../eigenvalue.md) force $u^*v=0$. For real [eigenvectors](../../../../../eigenvector.md) this is ordinary Euclidean orthogonality. These arguments establish [real symmetric spectral orthogonality](../../../../../real-symmetric-spectral-orthogonality.md) without assuming a diagonalization in advance.

A real [orthogonal matrix](../../../../../orthogonal-matrix.md) satisfies $P^TP=I$, equivalently $P^{-1}=P^T$. If $A$ is symmetric,

$$
(P^{-1}AP)^T=(P^TAP)^T=P^TA^TP=P^TAP=P^{-1}AP,
$$

so orthogonal similarity preserves symmetry. An arbitrary real invertible change of basis need not do so. For example,

$$
A=\begin{pmatrix}1&0\\0&2\end{pmatrix},\qquad P=\begin{pmatrix}1&1\\0&1\end{pmatrix},\qquad P^{-1}AP=\begin{pmatrix}1&-1\\0&2\end{pmatrix}.
$$

The final matrix is not symmetric. **Orthogonal similarity preserves real symmetry; general similarity does not.**

## ↑ Ancestors (10)

1. [7D](../7d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
