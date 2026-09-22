<h1 id="1f/solution">Solution</h1>

↑ **Parent:** [1F](../1f.md)

For a [linear map](../../../../../linear-map.md) $\alpha:U\to V$ with $U$ a [finite-dimensional vector space](../../../../../finite-dimensional-vector-space.md), the [rank-nullity theorem](../../../../../rank-nullity-theorem.md) is

$$
\boxed{\dim U=\dim\ker\alpha+\dim\operatorname{im}\alpha.}
$$

Choose a [basis](../../../../../basis.md) $u_1,\ldots,u_k$ of the [kernel of a linear map](../../../../../kernel-of-a-linear-map.md) and extend it to a basis $u_1,\ldots,u_k,v_1,\ldots,v_r$ of $U$. The vectors $\alpha(v_j)$ span the [image of a linear map](../../../../../image-of-a-linear-map.md), because the kernel basis contributes zero. If $\sum_j c_j\alpha(v_j)=0$, then $\sum_j c_jv_j$ belongs to the kernel and is a combination of the $u_i$; independence of the extended basis makes every $c_j=0$. Thus the image basis has $r$ elements and $\dim U=k+r$, proving the theorem.

For a rank-two map on $\mathbb R^3$, the [direct sum](../../../../../direct-sum.md) occurs for $\alpha(x,y,z)=(x,y,0)$: its kernel is $\mathbb Re_3$ and its image is $\operatorname{span}(e_1,e_2)$. It fails for $\beta(x,y,z)=(y,z,0)$: the kernel is $\mathbb Re_1$, contained in the two-dimensional image $\operatorname{span}(e_1,e_2)$. The [rank-nullity theorem](../../../../../rank-nullity-theorem.md) fixes the sum of the dimensions, but does not imply zero intersection.

## ↑ Ancestors (10)

1. [1F](../1f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
