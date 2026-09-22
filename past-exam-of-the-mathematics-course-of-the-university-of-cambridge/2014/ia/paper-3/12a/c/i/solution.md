<h1 id="12a/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Split the array in its first two slots:

$$
d^s_{ijk}=\frac{d_{ijk}+d_{jik}}2,\qquad
d^a_{ijk}=\frac{d_{ijk}-d_{jik}}2.
$$

For every [symmetric second-rank tensor](../../../../../../../symmetric-second-rank-tensor.md) $s$, antisymmetry gives $d^a_{ijk}s_{ij}=0$. Hence the stipulated [vector](../../../../../../../vector.md) equals $d^s_{ijk}s_{ij}$.

Let $R$ change the orthonormal frame, so $s'_{ab}=R_{ai}R_{bj}s_{ij}$. The [vector](../../../../../../../vector.md) transformation law gives

$$
d^{s\prime}_{abc}R_{ai}R_{bj}s_{ij}
=R_{ck}d^s_{ijk}s_{ij}
$$

for every symmetric test $s$. Both coefficient arrays in $i,j$ are symmetric, so equality against every symmetric [matrix](../../../../../../../matrix.md) forces equality of the coefficients; one may test the individual diagonal entries and the symmetric off-diagonal [basis](../../../../../../../basis.md) [matrices](../../../../../../../matrix.md). Multiplying by $R_{ai}R_{bj}$ and using orthogonality yields

$$
\boxed{d^{s\prime}_{abc}=R_{ai}R_{bj}R_{ck}d^s_{ijk}.}
$$

This is exactly the rank-three [tensor](../../../../../../../tensor.md) law. It is the [symmetric-test criterion for a third-rank Cartesian tensor](../../../../../../../symmetric-test-criterion-for-a-third-rank-cartesian-tensor.md), a form of the [quotient theorem for Cartesian tensors](../../../../../../../quotient-theorem-for-cartesian-tensors.md). Equivalently one may test $s_{ij}=(u_iv_j+v_iu_j)/2$ for arbitrary [vectors](../../../../../../../vector.md) $u,v$ and apply the quotient theorem twice.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [12A](../../../12a.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ia](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
