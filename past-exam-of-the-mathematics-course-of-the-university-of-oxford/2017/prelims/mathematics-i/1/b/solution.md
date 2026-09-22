<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $u=(a,b)^T$, $v=(c,d)^T$ and $\Delta=ad-bc$. If $xu+yv=0$, then

$$
ax+cy=0,\qquad bx+dy=0.
$$

Eliminating $y$ gives $\Delta x=0$, and eliminating $x$ gives $\Delta y=0$. Hence $\Delta\ne0$ implies [linear independence](../../../../../../linear-independence.md).

For the converse, suppose $\Delta=0$. If $u=0$, the family already contains the [zero vector](../../../../../../zero-vector.md) and is [linearly dependent](../../../../../../linear-dependence.md). If $a\ne0$, the equality $ad=bc$ gives $v=(c/a)u$. If $a=0$ but $u\ne0$, then $b\ne0$ and $bc=0$ forces $c=0$, so $v=(d/b)u$. Both cases give a nontrivial [linear relation](../../../../../../linear-relation.md). Therefore

$$
\boxed{u,v\text{ are linearly independent}\iff ad-bc\ne0.}
$$

This is the two-dimensional [determinant](../../../../../../determinant.md) criterion, proved directly without assuming that criterion.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
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
