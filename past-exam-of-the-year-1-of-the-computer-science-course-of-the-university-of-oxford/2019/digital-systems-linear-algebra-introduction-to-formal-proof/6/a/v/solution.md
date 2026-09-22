<h1 id="6/a/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

The [iteration matrix](../../../../../../iteration-matrix.md) has [eigenvalues](../../../../../../eigenvalue.md) **$0,-1/2,1/2$**: expanding its [characteristic polynomial](../../../../../../characteristic-polynomial.md) down the first column leaves the triangular two-by-two block with diagonal entries $-1/2,1/2$. The distinct [eigenvalues](../../../../../../eigenvalue.md) ensure [diagonalizability](../../../../../../diagonalizable-matrix.md). Thus its [spectral radius](../../../../../../spectral-radius.md) is $1/2<1$.

The previous bound gives $\|f_n\|\le2^{-n}\|f_0\|\to0$, so **the [Gauss-Seidel iteration](../../../../../../gauss-seidel-method.md) converges for every initial guess** under the stated [diagonalization](../../../../../../diagonalization-of-a-matrix.md). Its [limit](../../../../../../limit-of-a-function.md) is the exact solution $(1,1,-1)^T$. Since $e_n=Sf_n$, a fixed [matrix](../../../../../../matrix.md) also sends this transformed error to zero; its [operator norm](../../../../../../operator-norm.md) can account for any amplification in the original coordinates.

## ↑ Ancestors (13)

1. [V](../v.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
