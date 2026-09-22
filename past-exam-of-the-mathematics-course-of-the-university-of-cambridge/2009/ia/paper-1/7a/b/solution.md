<h1 id="7a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the convention

$$
P_A(t)=\det(tI-A)=\sum_{r=0}^n a_rt^r
$$

for the [characteristic polynomial](../../../../../../characteristic-polynomial.md). Choosing $\det(A-tI)$ instead multiplies it by $(-1)^n$ and leaves the requested zero identity unchanged. For each [eigenvector](../../../../../../eigenvector.md) $v_j$, induction gives $A^rv_j=\lambda_j^rv_j$, including $r=0$. Thus

$$
\left(\sum_{r=0}^n a_rA^r\right)v_j=P_A(\lambda_j)v_j=0,
$$

because $\lambda_jI-A$ has the nonzero [kernel](../../../../../../kernel-of-a-linear-map.md) [vector](../../../../../../vector.md) $v_j$ and therefore has zero [determinant](../../../../../../determinant.md). Part (a) supplies a [basis](../../../../../../basis.md) consisting of these $n$ [eigenvectors](../../../../../../eigenvector.md). A [linear map](../../../../../../linear-map.md) vanishing on every [basis](../../../../../../basis.md) [vector](../../../../../../vector.md) vanishes everywhere. Consequently

$$
\boxed{\sum_{r=0}^n a_rA^r=0.}
$$

This proves the [Cayley-Hamilton theorem](../../../../../../cayley-hamilton-theorem.md) identity directly in the distinct-[eigenvalue](../../../../../../eigenvalue.md) case assumed here.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7A](../../7a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
