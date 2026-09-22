<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

For a [linear map](../../../../../linear-map.md) $T:V\to W$ with $V$ finite-dimensional, the [rank-nullity theorem](../../../../../rank-nullity-theorem.md) states

$$
\boxed{\dim V=\dim\ker T+\dim\operatorname{im}T.}
$$

To prove it, choose a [basis](../../../../../basis.md) $v_1,\ldots,v_k$ of the [kernel of a linear map](../../../../../kernel-of-a-linear-map.md) and use [basis extension](../../../../../basis-extension.md) to obtain $v_1,\ldots,v_n$ as a basis of $V$. The vectors $Tv_{k+1},\ldots,Tv_n$ span the [image of a linear map](../../../../../image-of-a-linear-map.md): applying $T$ to a basis expansion kills the first $k$ terms. They are also linearly independent. Indeed, if $\sum_{j>k}a_jTv_j=0$, then $\sum_{j>k}a_jv_j\in\ker T$, so it is a combination of $v_1,\ldots,v_k$. Independence of the full basis forces every $a_j=0$. Consequently $\dim\operatorname{im}T=n-k$, proving the theorem.

Here the [image of a linear map](../../../../../image-of-a-linear-map.md) has dimension $r\in\{0,1,2,3\}$, since it lies in $\mathbb R^3$. Thus

$$
\boxed{\dim\ker\alpha\in\{2,3,4,5\}.}
$$

Every possibility occurs: for $0\le r\le3$, map $(x_1,\ldots,x_5)$ to $(x_1,\ldots,x_r,0,\ldots,0)\in\mathbb R^3$. This map has rank $r$ and kernel dimension $5-r$.

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
