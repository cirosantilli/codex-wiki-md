<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the first [matrix](../../../../../matrix.md), the [characteristic polynomial](../../../../../characteristic-polynomial.md) is

$$
\det(tI-A)=(t-3)\big((t-2)(t-1)-6\big)=(t-3)(t-4)(t+1).
$$

Thus the real [eigenvalues](../../../../../eigenvalue.md) are $4,-1,3$. Corresponding [eigenvectors](../../../../../eigenvector.md) are $(3,1,0)^\mathsf T$, $(-2,1,0)^\mathsf T$ and $(0,0,1)^\mathsf T$. They are [linearly independent](../../../../../linear-independence.md); the [determinant](../../../../../determinant.md) of the [matrix](../../../../../matrix.md) with these columns is $5$. Therefore

$$
\boxed{X=\begin{pmatrix}3&-2&0\\1&1&0\\0&0&1\end{pmatrix},\qquad X^{-1}AX=\operatorname{diag}(4,-1,3).}
$$

For example, multiplying the first column by $A$ gives $(12,4,0)^\mathsf T$, four times that column; multiplying the second gives $(2,-1,0)^\mathsf T$, its negative. These also check the chosen [eigenvectors](../../../../../eigenvector.md) directly.

For the second [matrix](../../../../../matrix.md),

$$
\det(tI-A)=t^3-1=(t-1)(t^2+t+1).
$$

The quadratic factor has negative [discriminant](../../../../../discriminant.md) $-3$, so $1$ is the only real [eigenvalue](../../../../../eigenvalue.md). Solving $Av=v$ gives $v=(a,a,a)^\mathsf T$, a one-dimensional [eigenspace](../../../../../eigenspace.md). It cannot provide a [basis](../../../../../basis.md) of $\mathbb R^3$, so

$$
\boxed{\text{the only real eigenvalue is }1;\quad A\text{ is not diagonalizable over }\mathbb R.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Calculus, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../calculus-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
