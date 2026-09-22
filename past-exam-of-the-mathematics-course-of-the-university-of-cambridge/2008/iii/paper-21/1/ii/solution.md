<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Suppose the map were nonconstant. Since [projective space](../../../../../../projective-space-split.md) is proper, its image $Z$ is a closed projective subvariety of $\mathbb P^n$, of positive dimension $r\le n$. Fix $y\in Z$. Regard the map as surjective onto $Z$; the [fiber dimension theorem](../../../../../../fiber-dimension-theorem.md) just proved gives

$$
\dim\phi^{-1}(y)\ge m-r\ge m-n>0.
$$

Choose a target hyperplane $H$ not containing $y$. It meets $Z$: the [affine cone](../../../../../../affine-cone.md) over $Z$ has dimension $r+1\ge2$, and the hyperplane equation vanishes at its vertex but not identically. By the [principal hypersurface dimension lemma](../../../../../../principal-hypersurface-dimension-lemma.md) its zero set on the cone has dimension $r\ge1$, so it contains a nonzero cone point and hence a point of $Z\cap H$.

The inverse image $D=\phi^{-1}(H)$ is therefore nonempty and proper. Locally the hyperplane equation is a single regular equation, after trivializing the pulled-back [line bundle](../../../../../../line-bundle.md). On the irreducible smooth source it is not identically zero, so the same hypersurface dimension lemma shows that each component of $D$ has dimension $m-1$. Choose one component $D_0$. Its cone is a codimension-one irreducible closed subset of affine $(m+1)$-space, whose prime ideal is principal because the [polynomial ring](../../../../../../polynomial-ring.md) is a [unique factorization domain](../../../../../../unique-factorization-domain.md). Thus $D_0$ is a [projective hypersurface](../../../../../../projective-hypersurface.md) defined by a homogeneous polynomial $P$ of positive degree.

Choose a positive-dimensional [irreducible component](../../../../../../irreducible-component.md) $F$ of $\phi^{-1}(y)$. Since $y\notin H$, $F$ is disjoint from $D_0$. On the cone over $F$, the equation $P$ is consequently nonzero everywhere except at the vertex. This contradicts the hypersurface dimension lemma: the cone has dimension at least two, so its nonempty proper zero set for $P$ has dimension at least one and cannot consist just of the vertex. Therefore **$\boxed{\phi\text{ is constant}}$**. The argument proves [morphisms from projective space to smaller projective space are constant](../../../../../../morphisms-from-projective-space-to-smaller-projective-space-are-constant.md) by combining the fibre bound with the forced intersection of a positive-dimensional [projective variety](../../../../../../projective-variety.md) and a hypersurface.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
