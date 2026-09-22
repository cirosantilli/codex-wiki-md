<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

By the [Eckart-Young-Mirsky theorem](../../../../../eckart-young-mirsky-theorem.md), truncate the [singular value decomposition](../../../../../singular-value-decomposition.md):

$$
\boxed{A_r=\sum_{j=1}^r\sigma_j u_jv_j^T},\qquad
\boxed{\|A-A_r\|_2=\sigma_{r+1}},\qquad
\boxed{\|A-A_r\|_F=\left(\sum_{j=r+1}^n\sigma_j^2\right)^{1/2}}.
$$

The same $A_r$ minimizes the [spectral norm](../../../../../matrix-2-norm.md) and [Frobenius norm](../../../../../frobenius-norm.md) errors over [matrices](../../../../../matrix.md) of [matrix rank](../../../../../matrix-rank.md) at most $r$. This conventional meaning of rank-$r$ [low-rank approximation](../../../../../low-rank-approximation.md) includes the case $\operatorname{rank}A<r$, when $A_r=A$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the numerical linear algebra course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra course of the University of Oxford](../../../../../numerical-linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
