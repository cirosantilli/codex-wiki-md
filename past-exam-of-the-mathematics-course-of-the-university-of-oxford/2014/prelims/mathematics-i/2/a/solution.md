<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [linear map](../../../../../../linear-map.md) $T:V\to V$, its [kernel of a linear map](../../../../../../kernel-of-a-linear-map-split.md) and [image of a linear map](../../../../../../image-of-a-linear-map.md) are

$$
\ker T=\{v\in V:T(v)=0\},\qquad\operatorname{im}T=\{T(v):v\in V\}.
$$

Its [nullity of a linear map](../../../../../../nullity-of-a-linear-map.md) is $n(T)=\dim\ker T$, and its [rank of a linear map](../../../../../../rank-of-a-linear-map.md) is $r(T)=\dim\operatorname{im}T$.

Choose a [basis](../../../../../../basis.md) $u_1,\ldots,u_k$ of $\ker T$ and extend it to a [basis](../../../../../../basis.md) $u_1,\ldots,u_k,v_1,\ldots,v_m$ of $V$. The [vectors](../../../../../../vector.md) $T(v_1),\ldots,T(v_m)$ span $\operatorname{im}T$, because applying $T$ to an arbitrary [linear combination](../../../../../../linear-combination.md) of the full [basis](../../../../../../basis.md) eliminates the $u_i$ terms. They are also [linearly independent](../../../../../../linear-independence.md): if $\sum_jb_jT(v_j)=0$, then $\sum_jb_jv_j\in\ker T$, so $\sum_jb_jv_j=\sum_i a_i u_i$ for some coefficients. Independence of the extended [basis](../../../../../../basis.md) forces all $a_i,b_j$ to vanish.

Consequently $r(T)=m$, $n(T)=k$ and $\dim V=k+m$. This proves the [rank-nullity theorem](../../../../../../rank-nullity-theorem.md):

$$
\boxed{\dim V=r(T)+n(T).}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Mathematics I](../../../mathematics-i-split.md)
4. [Prelims](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
