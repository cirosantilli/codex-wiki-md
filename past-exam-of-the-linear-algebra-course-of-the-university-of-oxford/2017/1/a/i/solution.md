<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a [linear transformation](../../../../../linear-map.md) $T$ of a [finite-dimensional vector space](../../../../../finite-dimensional-vector-space.md) over a [field](../../../../../field.md) $F$, its [minimal polynomial](../../../../../minimal-polynomial.md) $m_T$ is the unique [monic polynomial](../../../../../monic-polynomial.md) of least degree satisfying $m_T(T)=0$. There is at least one nonzero [polynomial](../../../../../polynomial-split.md) with this property because the powers $I,T,T^2,\ldots$ lie in the finite-dimensional [vector space](../../../../../vector-space-split.md) of linear maps $V\to V$. Dividing any other such [polynomial](../../../../../polynomial-split.md) by $m_T$ leaves a remainder of smaller degree that also vanishes at $T$, so that remainder must be zero. This also proves uniqueness.

If $C$ represents $T$ in any [basis](../../../../../basis.md), the paper's [characteristic polynomial](../../../../../characteristic-polynomial.md) is

$$
\boxed{\chi_T(x)=\det(C-xI).}
$$

It is independent of the [basis](../../../../../basis.md), since changing the [basis](../../../../../basis.md) replaces $C-xI$ by a [similar matrix](../../../../../matrix-similarity.md), preserving its [determinant](../../../../../determinant.md). Its degree is $\dim V$ and its leading coefficient is $(-1)^{\dim V}$; $m_T$ is always [monic](../../../../../monic-polynomial.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the linear algebra course of the University of Oxford](../../../../split.md)
6. [Linear algebra course of the University of Oxford](../../../../../linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
