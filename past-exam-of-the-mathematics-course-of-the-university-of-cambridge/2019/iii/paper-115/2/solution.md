<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

An [immersed submanifold](../../../../../immersed-submanifold.md) of $M$ is a manifold $Y$ equipped with an injective [immersion](../../../../../immersion.md) $\psi:Y\to M$. It is an [embedded submanifold](../../../../../embedded-submanifold.md) when $\psi$ is also a homeomorphism onto its image with the subspace topology, equivalently when it is a [smooth embedding](../../../../../smooth-embedding.md). For irrational $\alpha$, the [irrational winding of the torus](../../../../../irrational-winding-of-the-torus.md)

$$
t\longmapsto(e^{it},e^{i\alpha t})
$$

is an injective immersion $\mathbb R\to T^2$ with dense image, and therefore is not an embedding. If $Y$ is compact, however, an injective immersion is a continuous bijection from a [compact](../../../../../compact-space.md) space to its image in the [Hausdorff](../../../../../hausdorff-space.md) manifold $M$; its inverse is continuous. Thus the [compact injective immersion is an embedding](../../../../../compact-injective-immersion-is-an-embedding.md) theorem makes $\psi(Y)$ embedded.

Now let $X\subset M$ be embedded, with $\dim M=m$, $\dim X=m-k$, and $p\in X$. Apply the [constant rank theorem](../../../../../constant-rank-theorem.md) to its inclusion. After choosing coordinates and reordering them, there is a neighborhood $U$ of $p$ with coordinates $(x^1,\ldots,x^m)$ for which

$$
\boxed{U\cap X=\{x^1=\cdots=x^k=0\}.}
$$

This is the [slice chart for an embedded submanifold](../../../../../slice-chart-for-an-embedded-submanifold.md).

It is **false** that every embedded submanifold is the inverse image of a regular value of a map to a [Euclidean space](../../../../../euclidean-norm.md). If a codimension-$k$ submanifold is $f^{-1}(y)$ for a [regular value](../../../../../regular-value.md) of $f:M\to\mathbb R^k$, the differentials of the component functions give a global frame of its conormal bundle, so its [normal bundle](../../../../../normal-bundle.md) is trivial. The core circle of the [Möbius band](../../../../../mobius-band.md) is embedded but has the nontrivial Möbius normal line bundle. This is the [normal-bundle obstruction to being a regular level set](../../../../../normal-bundle-obstruction-to-being-a-regular-level-set.md).

Finally, an inductive spinning construction gives the requested torus. Place an embedding $F:N^m\hookrightarrow\mathbb R^{m+1}$ in the half-space $F_{m+1}>0$ and define

$$
\widetilde F(x,e^{i\theta})=
\bigl(F_1(x),\ldots,F_m(x),F_{m+1}(x)\cos\theta,F_{m+1}(x)\sin\theta\bigr).
$$

The positive radius makes this map injective, and its differential is injective in both the $N$ and circle directions; compactness then makes it an embedding. Starting with $S^1\hookrightarrow\mathbb R^2$ and iterating proves the [embedding of the n-dimensional torus in codimension one](../../../../../embedding-of-the-n-dimensional-torus-in-codimension-one.md):

$$
\boxed{T^n\hookrightarrow\mathbb R^{n+1}.}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 115](../../paper-115-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
