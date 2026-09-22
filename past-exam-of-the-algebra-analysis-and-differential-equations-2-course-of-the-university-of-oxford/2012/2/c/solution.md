<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a nonzero [eigenvector](../../../../eigenvector.md) $u$ of $S^*S$,

$$
\|Su\|^2=\langle Su,Su\rangle
=\langle u,S^*Su\rangle
=\langle u,\lambda u\rangle
=\overline\lambda\|u\|^2.
$$

Therefore $\overline\lambda=\|Su\|^2/\|u\|^2$ is real and nonnegative, and so **every [eigenvalue](../../../../eigenvalue.md) $\lambda$ is real and nonnegative**.

The preceding adjoint identities give $(S^*S)^*=S^*S$, so this [linear operator](../../../../linear-operator.md) is [self-adjoint](../../../../self-adjoint-operator.md). The stated finite-dimensional [spectral theorem](../../../../spectral-theorem.md) supplies an [orthonormal basis](../../../../orthonormal-basis.md) $e_j$ with $S^*Se_j=\lambda_j e_j$. If $v=\sum_jc_je_j$, then

$$
\|v\|^2=\sum_j|c_j|^2,\qquad
\|Sv\|^2=\langle v,S^*Sv\rangle=\sum_j\lambda_j|c_j|^2.
$$

Since $\lambda_-\leq\lambda_j\leq\lambda_+$,

$$
\lambda_-\|v\|^2\leq\|Sv\|^2\leq\lambda_+\|v\|^2.
$$

Taking nonnegative [square roots](../../../../square-root.md) proves

$$
\boxed{\sqrt{\lambda_-}\|v\|\leq\|Sv\|\leq\sqrt{\lambda_+}\|v\|.}
$$

The square roots of these extreme [eigenvalues](../../../../eigenvalue.md) are the smallest and largest [singular values](../../../../singular-value.md) of $S$; the lower bound can be zero if $S$ has a nontrivial [kernel of a linear map](../../../../kernel-of-a-linear-map-split.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
