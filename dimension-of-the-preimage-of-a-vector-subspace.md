# Dimension of the preimage of a vector subspace

↑ **Parent:** [Preimage](preimage.md)

Let $T:U\to V$ be a [linear map](linear-map.md) between finite-dimensional [vector spaces](vector-space-split.md) and $X$ a [vector subspace](vector-subspace.md) of $V$. The [preimage](preimage.md) $T^{-1}(X)$ is a [vector subspace](vector-subspace.md) containing $\ker T$. To compute its [dimension](dimension-vector-space.md), choose a [basis](basis.md) $k_1,\ldots,k_s$ of $\ker T$ and a [basis](basis.md) $y_1,\ldots,y_d$ of $X\cap\operatorname{im}T$. Lift each $y_j$ to $u_j\in U$ with $Tu_j=y_j$. Then $k_1,\ldots,k_s,u_1,\ldots,u_d$ is a [basis](basis.md) of $T^{-1}(X)$: applying $T$ proves [linear independence](linear-independence.md), and subtracting a suitable [linear combination](linear-combination.md) of the lifts reduces every element of the [preimage](preimage.md) to the [kernel](kernel-of-a-linear-map-split.md). This proves the displayed formula without using the [rank-nullity theorem](rank-nullity-theorem.md). Taking $X=V$ then proves the [rank-nullity theorem](rank-nullity-theorem.md) itself.

## ↑ Ancestors (7)

1. [Preimage](preimage.md)
2. [Image and preimage of a function](image-and-preimage-of-a-function.md)
3. [Set theory](set-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2017/prelims/mathematics-i/3/a/solution.md)
