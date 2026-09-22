<h1 id="7a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [characteristic polynomials](../../../../../../characteristic-polynomial.md), in the convention $\det(\lambda I-T)$, are

$$
\chi_A(\lambda)=(\lambda-1)(\lambda-2)^2,\qquad\chi_B(\lambda)=(\lambda-2)(\lambda-4)(\lambda-6).
$$

Solving the [eigenvalue equations](../../../../../../eigenvalue-equation.md) gives the complete [eigenspaces](../../../../../../eigenspace.md)

$$
\begin{aligned}
E_1(A)&=\operatorname{span}\{(1,1,1)^T\},\\
E_2(A)&=\{(x,y,z)^T:y=x+z\}=\operatorname{span}\{(1,0,-1)^T,(1,2,1)^T\},\\
E_2(B)&=\operatorname{span}\{(1,1,1)^T\},\\
E_4(B)&=\operatorname{span}\{(1,0,-1)^T\},\\
E_6(B)&=\operatorname{span}\{(1,2,1)^T\}.
\end{aligned}
$$

Every nonzero vector in a listed [eigenspace](../../../../../../eigenspace.md) is an [eigenvector](../../../../../../eigenvector.md), and these are all the [eigenvectors](../../../../../../eigenvector.md). For $A$, the repeated [eigenvalue](../../../../../../eigenvalue.md) $2$ has a two-dimensional [eigenspace](../../../../../../eigenspace.md); for $B$, all three [eigenvalues](../../../../../../eigenvalue.md) are simple. The three displayed generating vectors form a [basis](../../../../../../basis.md) because their column matrix

$$
S=\begin{pmatrix}1&1&1\\1&0&2\\1&-1&1\end{pmatrix}
$$

has [determinant](../../../../../../determinant.md) $2$. Thus **both matrices are diagonalizable**, with diagonal entries $(1,2,2)$ for $A$ and $(2,4,6)$ for $B$ in this [basis](../../../../../../basis.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [7A](../../7a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
