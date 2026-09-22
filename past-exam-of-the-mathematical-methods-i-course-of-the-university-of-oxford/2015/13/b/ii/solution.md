<h1 id="13/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The second [gradient](../../../../../gradient.md) is $\nabla_v b=[A+B-(\alpha+\beta)I]v$. Combining its vanishing with $(A-\alpha I)v=0$ gives

$$
\boxed{v\in\ker(A-\alpha I)\cap\ker(B-\beta I).}
$$

The zero vector always works. A nonzero common stationary vector exists exactly when $A,B$ have a common [eigenvector](../../../../../eigenvector.md) with respective [eigenvalues](../../../../../eigenvalue.md) $\alpha,\beta$; both stationary values are then zero. [Commuting symmetric matrices have a common orthonormal eigenbasis](../../../../../commuting-symmetric-matrices-have-a-common-orthonormal-eigenbasis.md), so commutation is sufficient to find such vectors for the paired [eigenvalues](../../../../../eigenvalue.md) in that basis. It does not guarantee an arbitrary prescribed pair.

Commutation is also not necessary for one common [eigenvector](../../../../../eigenvector.md). For example,

$$
A=\operatorname{diag}(1,2,3),\qquad B=\begin{pmatrix}\beta&0&0\\0&0&1\\0&1&0\end{pmatrix}
$$

are real [symmetric matrices](../../../../../symmetric-matrix.md) sharing $e_1$ with [eigenvalues](../../../../../eigenvalue.md) $1,\beta$, but $AB\ne BA$. This separates the question's common-vector condition from the stronger [simultaneous diagonalization](../../../../../simultaneous-diagonalization.md) of the entire space.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [13](../../../13.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the mathematical methods I course of the University of Oxford](../../../../split.md)
6. [Mathematical methods I course of the University of Oxford](../../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
