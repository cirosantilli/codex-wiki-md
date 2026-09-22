<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [preimage](../../../../../../preimage.md) is

$$
T^{-1}(X)=\{u\in U:T(u)\in X\}.
$$

It contains $0$, and if $u,v$ belong to it and $a,b\in\mathbb R$, then $T(au+bv)=aT(u)+bT(v)\in X$, since $X$ is a [vector subspace](../../../../../../vector-subspace.md). Thus $T^{-1}(X)$ is a [vector subspace](../../../../../../vector-subspace.md). It contains the [kernel](../../../../../../kernel-of-a-linear-map-split.md) of $T$ because $0\in X$.

To establish the [dimension of the preimage of a vector subspace](../../../../../../dimension-of-the-preimage-of-a-vector-subspace.md) formula without assuming the theorem to be deduced, choose a [basis](../../../../../../basis.md) $k_1,\ldots,k_{n_T}$ of $\ker T$ and a [basis](../../../../../../basis.md) $y_1,\ldots,y_d$ of $X\cap\operatorname{im}T$, where $d=\dim(X\cap\operatorname{im}T)$. For each $j$, choose $u_j\in U$ with $T(u_j)=y_j$. These $u_j$ lie in $T^{-1}(X)$.

The family $k_1,\ldots,k_{n_T},u_1,\ldots,u_d$ is [linearly independent](../../../../../../linear-independence.md): applying $T$ to a vanishing [linear combination](../../../../../../linear-combination.md) forces all $u_j$ [coefficients](../../../../../../coefficient.md) to vanish by [linear independence](../../../../../../linear-independence.md) of the $y_j$, and then all remaining [coefficients](../../../../../../coefficient.md) vanish by [linear independence](../../../../../../linear-independence.md) of the $k_i$. It also [spans](../../../../../../linear-span.md) $T^{-1}(X)$: for $u$ in that [preimage](../../../../../../preimage.md), write $T(u)=\sum_j b_jy_j$. Then $u-\sum_j b_ju_j\in\ker T$, so it is a [linear combination](../../../../../../linear-combination.md) of the $k_i$. Consequently

$$
\boxed{\dim T^{-1}(X)=\dim(X\cap\operatorname{im}T)+n_T.}
$$

Set $X=V$. Then $T^{-1}(V)=U$ and $V\cap\operatorname{im}T=\operatorname{im}T$, giving the [rank-nullity theorem](../../../../../../rank-nullity-theorem.md):

$$
\boxed{\dim U=r_T+n_T.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Mathematics I](../../../mathematics-i-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
