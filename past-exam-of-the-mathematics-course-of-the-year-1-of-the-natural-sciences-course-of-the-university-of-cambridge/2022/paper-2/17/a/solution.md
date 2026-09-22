<h1 id="17/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The displayed [matrix](../../../../../matrix.md) is **not orthogonal**: its first column has squared [Euclidean norm](../../../../../euclidean-norm.md) three, whereas every column of an [orthogonal matrix](../../../../../orthogonal-matrix.md) must have squared length one.

For the general assertion, put $C=AB$. In the [Einstein summation convention](../../../../../einstein-notation.md), orthogonality gives $A_{ki}A_{kj}=\delta_{ij}$ and $B_{ki}B_{kj}=\delta_{ij}$. The entries of $C$ satisfy

$$
C_{ki}C_{kj}
=A_{k\ell}B_{\ell i}A_{km}B_{mj}
=(A_{k\ell}A_{km})B_{\ell i}B_{mj}
=\delta_{\ell m}B_{\ell i}B_{mj}
=B_{\ell i}B_{\ell j}=\delta_{ij}.
$$

This is exactly $C^TC=I$, proving that the [matrix product](../../../../../matrix-product.md) $AB$ is orthogonal. The [Kronecker delta](../../../../../kronecker-delta.md) contracts the two middle indices without changing the multiplication order of the [matrices](../../../../../matrix.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [17](../../17.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
