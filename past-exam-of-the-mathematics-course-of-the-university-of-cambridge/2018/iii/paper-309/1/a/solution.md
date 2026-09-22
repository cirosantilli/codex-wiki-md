<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $q$ denote the quotient map and write $[X]$ for a point of [Real projective space](../../../../../../real-projective-space.md). For $i=1,\ldots,n+1$, take the open set

$$
U_i=\{[X]:X_i\ne0\}.
$$

It is open in the [quotient topology](../../../../../../quotient-topology.md) because its inverse image under $q$ is the open set $\{X:X_i\ne0\}$. These sets cover, since a nonzero vector has at least one nonzero coordinate. Define the [manifold chart](../../../../../../manifold-chart.md)

$$
\varphi_i([X])=(X_1/X_i,\ldots,\widehat{X_i/X_i},\ldots,X_{n+1}/X_i)\in\mathbb R^n.
$$

The hat means that the $i$th coordinate is omitted. Ratios are unchanged by multiplying $X$ by any nonzero real number, so the chart is well defined. Its inverse inserts $1$ into position $i$ and takes the resulting equivalence class. The ratios and this inverse are continuous, giving a [homeomorphism](../../../../../../homeomorphism.md) $U_i\to\mathbb R^n$.

For a compact description of the [smooth transition maps](../../../../../../smooth-transition-map.md), write $a_i=1$ and let $a_k=X_k/X_i$ for $k\ne i$. On $U_i\cap U_j$ one has $a_j\ne0$, and

$$
\boxed{(\varphi_j\circ\varphi_i^{-1})(a)_k=\frac{a_k}{a_j}\quad(k\ne j).}
$$

Each coordinate is a rational [smooth function](../../../../../../smooth-function.md) on the open domain $a_j\ne0$; reversing $i,j$ gives a smooth inverse. Thus these $n+1$ charts form the [standard affine atlas of real projective space](../../../../../../standard-affine-atlas-of-real-projective-space.md).

For completeness, the underlying space is [Hausdorff](../../../../../../hausdorff-space.md): normalizing $X$ identifies it with the antipodal quotient of the [unit sphere](../../../../../../unit-sphere.md), and the continuous injective map $[X]\mapsto XX^T/(X^TX)$ into the space of [symmetric matrices](../../../../../../symmetric-matrix.md) separates any two distinct classes by disjoint open neighborhoods. It is also a [second-countable space](../../../../../../second-countable-space.md): pull back the countable bases of rational balls in these finitely many charts, and take their union. Therefore

$$
\boxed{\mathbb{RP}^n\text{ is a smooth manifold of dimension }n,\text{ with an atlas of }n+1\text{ charts}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
