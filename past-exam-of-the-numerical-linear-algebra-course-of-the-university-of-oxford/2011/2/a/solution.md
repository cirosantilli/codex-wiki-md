<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [spectral theorem for real symmetric matrices](../../../../spectral-theorem-for-real-symmetric-matrices.md) gives $A=Q\Lambda Q^T$ with an [orthogonal matrix](../../../../orthogonal-matrix.md) $Q$. [Positive definiteness](../../../../positive-definiteness.md) makes every [eigenvalue](../../../../eigenvalue.md) $\lambda_i$ positive. Define the [matrix square root](../../../../square-root-of-a-matrix.md)

$$
\boxed{A^{1/2}=Q\operatorname{diag}(\sqrt{\lambda_1},\ldots,\sqrt{\lambda_n})Q^T.}
$$

It is [symmetric](../../../../symmetric-relation.md), its square is $A$, and for any nonzero [vector](../../../../vector.md) $x$,

$$
x^TA^{1/2}x=\sum_i\sqrt{\lambda_i}\,(Q^Tx)_i^2>0.
$$

Thus it is also [positive-definite](../../../../positive-definite-bilinear-form.md), and its [matrix inverse](../../../../matrix-inverse-split.md) is $A^{-1/2}=Q\operatorname{diag}(\lambda_i^{-1/2})Q^T$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the numerical linear algebra course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra course of the University of Oxford](../../../../numerical-linear-algebra-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
