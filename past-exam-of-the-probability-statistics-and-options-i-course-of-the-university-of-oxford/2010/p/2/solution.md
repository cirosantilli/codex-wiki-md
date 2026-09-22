<h1 id="p/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [QR decomposition](../../../../qr-decomposition.md) is $A=QR$, with $Q$ orthogonal and $R$ upper triangular. Orthogonality gives $Q^{\mathsf T}Q=I$, and therefore $\|Qx\|^2=x^{\mathsf T}Q^{\mathsf T}Qx=x^{\mathsf T}x=\|x\|^2$, proving invariance of the [Euclidean norm](../../../../euclidean-norm.md).

The unshifted [QR algorithm](../../../../qr-algorithm.md) starts with $A_0=A$. At step $k$, factor $A_k=Q_kR_k$ and set $A_{k+1}=R_kQ_k$. Then

$$
\boxed{A_{k+1}=Q_k^{\mathsf T}A_kQ_k.}
$$

Thus consecutive matrices are related by [orthogonal similarity](../../../../orthogonal-similarity.md), so they have the same [characteristic polynomial](../../../../characteristic-polynomial.md) and [eigenvalues](../../../../eigenvalue.md). Induction proves every iterate has the original [eigenvalues](../../../../eigenvalue.md). Symmetry is also preserved. When the iteration converges to diagonal form, its diagonal entries are the [eigenvalues](../../../../eigenvalue.md); practical implementations use shifts and deflation to improve convergence.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [P](../../p.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
