<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [rank of a linear map](../../../../../../rank-of-a-linear-map.md) and [nullity of a linear map](../../../../../../nullity-of-a-linear-map.md) are

$$
r(T)=\dim\operatorname{im}T,\qquad n(T)=\dim\ker T.
$$

The [rank-nullity theorem](../../../../../../rank-nullity-theorem.md) states that

$$
\boxed{r(T)+n(T)=\dim V=n.}
$$

To prove it, choose a [basis](../../../../../../basis.md) $u_1,\ldots,u_k$ of the [kernel of a linear map](../../../../../../kernel-of-a-linear-map-split.md) and use [basis extension](../../../../../../basis-extension.md) to obtain a [basis](../../../../../../basis.md)

$$
u_1,\ldots,u_k,v_1,\ldots,v_{n-k}
$$

of $V$. The [vectors](../../../../../../vector.md) $T(v_1),\ldots,T(v_{n-k})$ [span](../../../../../../linear-span.md) the [image of a linear map](../../../../../../image-of-a-linear-map.md): applying $T$ to an arbitrary [linear combination](../../../../../../linear-combination.md) of the displayed [basis](../../../../../../basis.md) removes all the $u_i$ terms. They are also [linearly independent](../../../../../../linear-independence.md). Indeed,

$$
\sum_j a_jT(v_j)=0\quad\Longrightarrow\quad\sum_j a_jv_j\in\ker T,
$$

so $\sum_j a_jv_j=\sum_i b_iu_i$ for some [scalars](../../../../../../scalar.md) $b_i$. The [linear independence](../../../../../../linear-independence.md) of the extended [basis](../../../../../../basis.md) forces every $a_j$ and $b_i$ to vanish. Consequently $r(T)=n-k$ and $n(T)=k$, proving the identity. The same argument covers an empty [basis](../../../../../../basis.md) when one of these [dimensions](../../../../../../dimension-vector-space.md) is zero.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Mathematics I](../../../mathematics-i-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
