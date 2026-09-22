<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose [homogeneous polynomials](../../../../../../homogeneous-polynomial.md) $F,G$ defining the two [projective plane curves](../../../../../../projective-plane-curve.md). Their absence of a common [irreducible component](../../../../../../irreducible-component.md) makes them coprime. For a point $O=[1:0:0]$ outside both [curves](../../../../../../curve.md), they have degrees $n,m$ in $X$ and nonzero constant leading coefficients. The [resultant](../../../../../../resultant.md)

$$
R(Y,Z)=\operatorname{Res}_X(F(X,Y,Z),G(X,Y,Z))
$$

is therefore nonzero. Indeed, a vanishing [resultant](../../../../../../resultant.md) over $k(Y,Z)$ would give a common factor there, and [Gauss's lemma](../../../../../../gauss-s-lemma-riemannian-geometry.md) would give a common component of the original [curves](../../../../../../curve.md).

The [homogeneity](../../../../../../homogeneity.md) of $F,G$ makes $R$ a [homogeneous polynomial](../../../../../../homogeneous-polynomial.md) of degree $nm$: scaling $(Y,Z)$ by $a$ scales their $X$-roots by $a$, and the product of the $nm$ differences of roots scales by $a^{nm}$. Every point in the [intersection](../../../../../../set-intersection.md) projects from $O$ to a zero of $R$ in the [projective line](../../../../../../projective-line.md). Each such projection line contains only finitely many points of either [curve](../../../../../../curve.md), since it passes through $O$ outside them. Thus the [intersection](../../../../../../set-intersection.md) is finite already.

We may now choose $O$ also outside the finitely many joining lines of distinct intersection points. Projection is then injective on the [intersection](../../../../../../set-intersection.md). A nonzero degree-$nm$ [homogeneous polynomial](../../../../../../homogeneous-polynomial.md) on the [projective line](../../../../../../projective-line.md) has at most $nm$ distinct zeros, so the [resultant bound for intersections of plane curves](../../../../../../resultant-bound-for-intersections-of-plane-curves.md) gives

$$
\boxed{|C\cap D|\le nm.}
$$

This derives the required cardinality bound without assuming the full intersection-multiplicity statement of [Bézout's theorem](../../../../../../bezout-s-theorem.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 14](../../../paper-14-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
