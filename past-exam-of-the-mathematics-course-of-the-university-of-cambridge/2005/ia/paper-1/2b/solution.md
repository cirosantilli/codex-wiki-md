<h1 id="2b/solution">Solution</h1>

↑ **Parent:** [2B](../2b.md)

Expanding the [cross product](../../../../../cross-product.md) component by component gives its [cross-product matrix](../../../../../cross-product-matrix.md):

$$
\boxed{A=\begin{pmatrix}0&-n_3&n_2\\n_3&0&-n_1\\-n_2&n_1&0\end{pmatrix}.}
$$

It is a real [skew-symmetric matrix](../../../../../skew-symmetric-matrix.md) and annihilates $\mathbf n$. By the [vector triple product](../../../../../vector-triple-product.md),

$$
A^2\mathbf x=\mathbf n\times(\mathbf n\times\mathbf x)=\mathbf n(\mathbf n\cdot\mathbf x)-\mathbf x,
$$

so $A^2=\mathbf n\mathbf n^T-I$ for a [unit vector](../../../../../unit-vector.md) $\mathbf n$. Choose a [unit vector](../../../../../unit-vector.md) $\mathbf u\perp\mathbf n$ and put $\mathbf v=\mathbf n\times\mathbf u$. Then $(\mathbf u,\mathbf v,\mathbf n)$ is an orthonormal basis and $A\mathbf u=\mathbf v$, $A\mathbf v=-\mathbf u$, $A\mathbf n=0$. Thus the characteristic polynomial is $\lambda(\lambda^2+1)$ and the [cross-product matrix spectrum](../../../../../cross-product-matrix-spectrum.md) is

$$
\boxed{\lambda=0,\ i,\ -i.}
$$

Over the complex numbers, corresponding [eigenvectors](../../../../../eigenvector.md) are $\mathbf n$, $\mathbf u-i\mathbf v$, and $\mathbf u+i\mathbf v$. Only the zero [eigenvalue](../../../../../eigenvalue.md) has real [eigenvectors](../../../../../eigenvector.md).

For the specified third coordinate axis, direct multiplication gives

$$
A=\begin{pmatrix}0&-1&0\\1&0&0\\0&0&0\end{pmatrix},\qquad \boxed{A^2=\operatorname{diag}(-1,-1,0).}
$$

Its zero [eigenspace](../../../../../eigenspace.md) is $\operatorname{span}\{(0,0,1)\}$, and its $-1$ [eigenspace](../../../../../eigenspace.md) is the whole plane $\operatorname{span}\{(1,0,0),(0,1,0)\}$. Hence the [eigenvalues](../../../../../eigenvalue.md) of $A^2$ are $-1,-1,0$, with every nonzero [vector](../../../../../vector.md) in the appropriate [eigenspace](../../../../../eigenspace.md) an [eigenvector](../../../../../eigenvector.md).

## ↑ Ancestors (10)

1. [2B](../2b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
