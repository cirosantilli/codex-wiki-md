<h1 id="19c/solution">Solution</h1>

↑ **Parent:** [19C](../19c.md)

The [linear least-squares problem](../../../../../linear-least-squares-problem.md) is to minimize $\|Ax-b\|_2^2$ over $x\in\mathbb R^n$, allowing an overdetermined system to have a nonzero residual. For a full [QR decomposition](../../../../../qr-decomposition.md), $Q$ is $m\times m$ orthogonal and $R$ is $m\times n$ with an upper-triangular top block. [Orthogonal transformations](../../../../../orthogonal-transformation.md) preserve the [Euclidean norm](../../../../../euclidean-norm.md), so

$$
\|Ax-b\|_2=\|Q^T(Ax-b)\|_2=\|Rx-Q^Tb\|_2.
$$

If $A$ has full column rank, the top triangular block is nonsingular; setting its residual to zero gives the unique minimizer, while the remaining residual is independent of $x$. Without full column rank, minimizers still exist but need not be unique.

For the specified matrix, one [Householder reflection](../../../../../householder-transformation.md) already produces an upper-triangular matrix. Take $v=(-1,1,1,1)^T$, the difference between the first column and $2e_1$, and set

$$
H=I-\frac{2vv^T}{v^Tv}
=\frac12\begin{pmatrix}1&1&1&1\\1&1&-1&-1\\1&-1&1&-1\\1&-1&-1&1\end{pmatrix}.
$$

The formula gives $H^T=H$, $H^2=I$. Direct multiplication yields the [Householder QR decomposition](../../../../../householder-qr-decomposition.md)

$$
\boxed{Q=H,\qquad R=HA=\begin{pmatrix}2&4&2\\0&2&2\\0&0&2\\0&0&0\end{pmatrix},\qquad A=QR.}
$$

All subdiagonal entries in the remaining columns are already zero, so no further reflection is needed. For the supplied right-hand side, $Q^Tb=(2,0,2,-2)^T$. Back substitution gives $x_3=1$, $x_2=-1$, $x_1=2$, hence

$$
\boxed{x^*=(2,-1,1)^T,\qquad\min\|Ax-b\|_2^2=4.}
$$

The residual $Ax^*-b=(1,-1,-1,1)^T$ is orthogonal to every column of $A$, independently confirming the [normal equations](../../../../../normal-equation.md) $A^T(Ax^*-b)=0$.

## ↑ Ancestors (10)

1. [19C](../19c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
