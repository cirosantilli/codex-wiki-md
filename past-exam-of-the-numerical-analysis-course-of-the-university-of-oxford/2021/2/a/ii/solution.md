<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $m=n$, $U$ and $V$ are square [orthogonal matrices](../../../../../orthogonal-matrix.md). Multiply the [linear system](../../../../../system-of-linear-equations.md) successively by $U^T$, $\Sigma^{-1}$ and $V$ to obtain

$$
\boxed{x=V\Sigma^{-1}U^Tb
=\sum_{j=1}^n\frac{u_j^Tb}{\sigma_j}v_j.}
$$

With the [singular value decomposition](../../../../../singular-value-decomposition.md) already supplied, compute $c=U^Tb$, divide $c_j$ by $\sigma_j$, then form $x=Vc$. The two dense [matrix-vector products](../../../../../matrix-vector-product.md) each cost $O(n^2)$ [arithmetic operations](../../../../../arithmetic-operation.md) in [Big O notation](../../../../../big-o-notation.md), and the diagonal scaling costs $O(n)$. Thus

$$
\boxed{\text{Cost per right-hand side with supplied factors: }O(n^2).}
$$

If the [singular value decomposition](../../../../../singular-value-decomposition.md) first has to be computed, its usual dense cost is $O(n^3)$; that is a separate setup cost and can be reused for further right-hand sides.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
