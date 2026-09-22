<h1 id="2i/solution">Solution</h1>

↑ **Parent:** [2I](../2i.md)

Let $\mathcal A$ be the closure of the [polynomials](../../../../../polynomial-split.md) in $C(K)$ for the [uniform norm](../../../../../supremum-norm.md). It is a closed [algebra](../../../../../algebra-split.md), since products of uniformly convergent sequences converge uniformly on the [compact set](../../../../../compact-space.md) $K$.

Choose a point $W$ with $|W|>\sup_{z\in K}|z|$. The uniformly convergent [geometric series](../../../../../geometric-series.md)

$$
\frac1{W-z}=\sum_{j=0}^{\infty}\frac{z^j}{W^{j+1}}
$$

shows that this reciprocal belongs to $\mathcal A$. Join $w$ to $W$ by a [continuous path](../../../../../continuous-path.md) in $\mathbb C\setminus K$. Its image is compact and disjoint from $K$, so their distance $d$ is positive. Partition the path into finitely many steps shorter than $d/2$.

Suppose $1/(b-z)\in\mathcal A$ and $|a-b|<d/2$, with $b$ on the path. Then

$$
\frac1{a-z}=\sum_{j=0}^{\infty}\frac{(b-a)^j}{(b-z)^{j+1}}
$$

converges uniformly on $K$, since $|b-z|\geq d$. Every partial sum belongs to $\mathcal A$, by its algebra property, and so does the limit. Working backwards along the partition transfers the pole from $W$ to $w$. Thus $1/(w-z)\in\mathcal A$: **a polynomial $P$ exists with**

$$
\boxed{\sup_{z\in K}\left|P(z)-\frac1{w-z}\right|<\epsilon.}
$$

This [pole-moving polynomial approximation](../../../../../pole-moving-polynomial-approximation.md) is the elementary mechanism behind the [polynomial Runge theorem](../../../../../polynomial-runge-theorem.md).

## ↑ Ancestors (10)

1. [2I](../2i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
