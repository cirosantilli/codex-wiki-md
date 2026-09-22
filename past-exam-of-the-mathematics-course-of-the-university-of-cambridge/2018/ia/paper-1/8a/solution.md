<h1 id="8a/solution">Solution</h1>

↑ **Parent:** [8A](../8a.md)

A real square matrix $M$ is an [orthogonal matrix](../../../../../orthogonal-matrix.md) when $M^TM=I$. The planar rotation

$$
R=\begin{pmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{pmatrix}
$$

obeys $R^TR=I$ by the [Pythagorean trigonometric identity](../../../../../pythagorean-trigonometric-identity.md).

For $A=\begin{pmatrix}a&b\\b&c\end{pmatrix}$, the off-diagonal entry of $RAR^T$ is $\frac12(a-c)\sin2\theta+b\cos2\theta$. Thus

$$
\boxed{(a-c)\sin2\theta+2b\cos2\theta=0.}
$$

If $(a-c,b)\ne(0,0)$, equivalently $\theta=\frac12\operatorname{atan2}(-2b,a-c)+k\pi/2$; if $A$ is scalar, every angle works.

Because $RAR^T$ is an [orthogonal similarity](../../../../../orthogonal-similarity.md), its diagonal entries are the eigenvalues

$$
\lambda_\pm=\frac{\operatorname{tr}A\pm\sqrt{(\operatorname{tr}A)^2-4\det A}}2.
$$

The matrix $C=\begin{pmatrix}1&2\\2&1\end{pmatrix}$ has eigenvalues $3,-1$ along $(1,1)^T,(1,-1)^T$. Raising its orthogonal diagonalization to the even power gives

$$
\boxed{C^{2N}=\frac12\begin{pmatrix}3^{2N}+1&3^{2N}-1\\3^{2N}-1&3^{2N}+1\end{pmatrix}.}
$$

## ↑ Ancestors (10)

1. [8A](../8a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
