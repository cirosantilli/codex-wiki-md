<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $T=\prod_{j=1}^nR_j$, and let $\rho_j:T\to R_j$ be the coordinate [ring homomorphism](../../../../../ring-homomorphism.md). Set $I_j=\rho_j(I)$. Each $I_j$ is an [ideal](../../../../../ideal.md): it is an additive subgroup, and multiplying a lift in $I$ on either side by a tuple with prescribed $j$th coordinate proves closure under left and right multiplication by $R_j$.

Certainly $I\subseteq\prod_jI_j$. Conversely, let $a=(a_1,\ldots,a_n)\in\prod_jI_j$. For each $j$, choose $b^{(j)}\in I$ with $j$th coordinate $a_j$, and let $e_j$ have $1_{R_j}$ in coordinate $j$ and zero elsewhere. Since $I$ is an [ideal](../../../../../ideal.md), $e_jb^{(j)}\in I$, and

$$
a=\sum_{j=1}^ne_jb^{(j)}\in I.
$$

Therefore

$$
\boxed{I=I_1\times\cdots\times I_n}.
$$

The finite sum is essential to this proof of [ideals of a finite product of rings](../../../../../ideals-of-a-finite-product-of-rings.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the rings and modules course of the University of Oxford](../../../../split.md)
6. [Rings and modules course of the University of Oxford](../../../../../rings-and-modules-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
