<h1 id="7d/solution">Solution</h1>

↑ **Parent:** [7D](../7d.md)

Let $Az=\lambda z$ with $z\ne0$, allowing complex [eigenvectors](../../../../../eigenvector.md). A real [symmetric matrix](../../../../../symmetric-matrix.md) is [Hermitian](../../../../../hermitian-operator.md), so $z^*Az$ is real and $\lambda=z^*Az/(z^*z)$ is real. For eigenvectors $u,v$ of distinct real [eigenvalues](../../../../../eigenvalue.md) $\lambda,\mu$, self-adjointness gives $\lambda u^*v=u^*Av=\mu u^*v$, hence $u^*v=0$. Thus the distinct eigenspaces are [orthogonal](../../../../../orthogonal-vectors.md).

Here $A=3I-J$, where $J$ is the all-ones matrix. Since $J(1,1,1)^T=3(1,1,1)^T$ and $J$ vanishes on the plane of coordinate sum zero,

$$
\boxed{\lambda=0:\ E_0=\operatorname{span}\{(1,1,1)^T\};\qquad\lambda=3:\ E_3=\operatorname{span}\{(1,-1,0)^T,(1,1,-2)^T\}.}
$$

Every nonzero vector in the indicated eigenspace is an eigenvector. The repeated eigenvalue three has a two-dimensional eigenspace.

A [complex symmetric nilpotent matrix](../../../../../complex-symmetric-nilpotent-matrix.md) provides the requested counterexample:

$$
\boxed{N=\begin{pmatrix}1&i\\i&-1\end{pmatrix},\qquad N\ne0,\quad N^T=N,\quad N^2=0.}
$$

Its characteristic polynomial is $\lambda^2$, so its only eigenvalue is zero. **It is not diagonalizable**: a diagonalizable matrix with only zero eigenvalues would itself be zero. Complex symmetry $N^T=N$ is weaker than the Hermitian condition $N^*=N$.

## ↑ Ancestors (10)

1. [7D](../7d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
