<h1 id="8d/solution">Solution</h1>

↑ **Parent:** [8D](../8d.md)

Expanding the [characteristic polynomial](../../../../../characteristic-polynomial.md) along the first column gives

$$
\begin{aligned}
\chi_A(\lambda)&=(\lambda-3)\left[(\lambda-4+s)(\lambda-4s+1)+4(s-1)^2\right]\\
&=\boxed{(\lambda-3)^2(\lambda-3s)}.
\end{aligned}
$$

For $s\ne1$, solving the two nullspace equations gives

$$
\boxed{E_3=\operatorname{span}\{(1,0,0)^T,(0,2,1)^T\},\qquad E_{3s}=\operatorname{span}\{(1,s-1,2s-2)^T\}.}
$$

These are all the [eigenvalues](../../../../../eigenvalue.md) and [eigenvectors](../../../../../eigenvector.md), with nonzero vectors understood. The three displayed spanning vectors form an [eigenbasis](../../../../../eigenbasis.md), so $A$ is [diagonalizable](../../../../../diagonalizable-matrix.md).

At $s=1$, the sole eigenvalue is three, with algebraic multiplicity three but the same two-dimensional $E_3$. Thus **$A$ is diagonalizable exactly when $s\ne1$**. Indeed, at the exceptional parameter, $A=3I+N$ with $N\ne0$ and $N^2=0$, so its [Jordan normal form](../../../../../jordan-normal-form.md) has one block of size two and one of size one. This illustrates how an [eigenvalue collision](../../../../../eigenvalue-collision.md) can destroy diagonalizability without changing the two-dimensional eigenspace.

## ↑ Ancestors (10)

1. [8D](../8d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
