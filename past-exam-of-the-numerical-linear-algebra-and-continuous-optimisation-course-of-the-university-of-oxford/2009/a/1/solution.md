<h1 id="a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A real square [orthogonal matrix](../../../../orthogonal-matrix.md) satisfies $Q^TQ=QQ^T=I$, so it preserves the [Euclidean norm](../../../../euclidean-norm.md). The columns of $Z_h$ are orthonormal, hence $\|Z_hv\|_2=\|v\|_2$. The [induced matrix norm](../../../../induced-matrix-norm.md) therefore gives

$$
\|AZ_h\|_2=\sup_{\|v\|_2=1}\|AZ_hv\|_2\leq\boxed{\|A\|_2}.
$$

For the left truncation, $\|Q_\ell^TA\|_2\leq\|A\|_2$, and equality is guaranteed for arbitrary $A$ only when $\boxed{\ell=m}$. Indeed, if $\ell<m$, take $A=q_{\ell+1}e_1^T$, where $q_{\ell+1}$ is an omitted column of $Q$. Then $\|A\|_2=1$ but $Q_\ell^TA=0$. Merely taking $\ell\geq n$ does not guarantee preservation for an arbitrary $A$.

A full [QR decomposition](../../../../qr-decomposition.md) of a real $m\times n$ matrix is $A=QR$, with $Q$ orthogonal and $R$ upper trapezoidal; for a square matrix, $R$ is upper triangular. Fix the following sign convention for a [Givens rotation](../../../../givens-rotation.md): it is the identity except for its $(i,k)$ block

$$
\begin{pmatrix}c&s\\-s&c\end{pmatrix},\qquad c=\cos\theta,\ s=\sin\theta.
$$

The block transpose times the block is $I_2$ because $c^2+s^2=1$, proving orthogonality. Writing $r=\sqrt{x_i^2+x_k^2}$, the choice $\boxed{c=x_i/r,\ s=x_k/r}$ gives $(Jx)_k=0$ and $(Jx)_i=r$. To zero the other coordinate take $\boxed{c=x_k/r,\ s=-x_i/r}$, giving $(Jx)_i=0$. If $r=0$, both entries are already zero and the identity suffices.

For a [tridiagonal matrix](../../../../tridiagonal-matrix.md), successively rotate adjacent row pairs $(1,2),(2,3),\ldots,(n-1,n)$, each time zeroing the current entry $(k+1,k)$. Earlier columns remain triangular because both affected rows are already zero there. The result $R=J_{n-1}\cdots J_1A$ is upper triangular, so $Q=J_1^T\cdots J_{n-1}^T$ gives its [QR decomposition](../../../../qr-decomposition.md). Only $n-1$ rotations are required; the resulting $R$ has at most two superdiagonals.

For a full square matrix, process columns $j=1,\ldots,n-1$. Within column $j$, for $i=n,n-1,\ldots,j+1$, rotate rows $(i-1,i)$ to eliminate the current $(i,j)$ entry. Previously cleared columns stay clear. With $J_1,\ldots,J_s$ in application order, $s=n(n-1)/2$, one has $\boxed{R=J_s\cdots J_1A,\quad Q=J_1^T\cdots J_s^T}$. This is [QR decomposition by Givens rotations](../../../../qr-decomposition-by-givens-rotations.md).

## ↑ Ancestors (12)

1. [1](../1.md)
2. [A](../../a.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
