<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An **[orthonormal basis](../../../../orthonormal-basis.md)** $(q_1,\ldots,q_n)$ is a [basis](../../../../basis.md) with $\langle q_i,q_j\rangle=\delta_{ij}$, where $\delta_{ij}$ is the [Kronecker delta](../../../../kronecker-delta.md). Each [vector](../../../../vector.md) has [norm](../../../../norm.md) one and distinct [vectors](../../../../vector.md) are [orthogonal](../../../../orthogonal-vectors.md).

The [Gram-Schmidt process](../../../../gram-schmidt-process.md) starts from a [basis](../../../../basis.md) $(e_1,\ldots,e_n)$ and defines

$$
u_1=e_1,\qquad q_1=\frac{u_1}{\|u_1\|},\qquad
u_k=e_k-\sum_{j=1}^{k-1}\langle e_k,q_j\rangle q_j,\qquad
q_k=\frac{u_k}{\|u_k\|}.
$$

The [coefficients](../../../../coefficient.md) are in this order because the [inner product](../../../../inner-product-split.md) is linear in its first argument. For $i<k$, taking the [inner product](../../../../inner-product-split.md) with $q_i$ gives $\langle u_k,q_i\rangle=0$. The residual $u_k$ cannot be zero: otherwise $e_k$ would belong to the [linear span](../../../../linear-span.md) of $e_1,\ldots,e_{k-1}$, contradicting the initial [basis](../../../../basis.md). Normalization makes $\|q_k\|=1$, while induction preserves

$$
\operatorname{span}(q_1,\ldots,q_k)=\operatorname{span}(e_1,\ldots,e_k).
$$

Thus the process produces an [orthonormal basis](../../../../orthonormal-basis.md) of all of $V$.

## ↑ Ancestors (12)

1. [A](../a.md)
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
