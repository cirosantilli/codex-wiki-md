<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [i](../i.md)

Let $\mathbf r(u,v)$ parametrize $S$. Then $A\mathbf r$ parametrizes its image, with [tangent vectors](../../../../../../../tangent-vector-split.md) $A\mathbf r_u$ and $A\mathbf r_v$. An [orthogonal matrix](../../../../../../../orthogonal-matrix.md) preserves [dot products](../../../../../../../dot-product.md), so the [Lagrange identity for the cross product](../../../../../../../lagrange-identity-for-the-cross-product.md) gives, for any $\mathbf p,\mathbf q$,

$$
\begin{aligned}
\|A\mathbf p\times A\mathbf q\|^2
&=\|A\mathbf p\|^2\|A\mathbf q\|^2-(A\mathbf p\cdot A\mathbf q)^2\\
&=\|\mathbf p\|^2\|\mathbf q\|^2-(\mathbf p\cdot\mathbf q)^2
=\|\mathbf p\times\mathbf q\|^2.
\end{aligned}
$$

The [area element of a surface](../../../../../../../area-element-of-a-surface.md) is therefore the same pointwise before and after applying $A$. Integrating proves

$$
\boxed{\operatorname{Area}(A S)=\operatorname{Area}(S).}
$$

This includes [orthogonal transformations](../../../../../../../orthogonal-transformation.md) with [determinant](../../../../../../../determinant.md) $-1$: reversal of [orientation](../../../../../../../orientation-of-a-simplex.md) does not affect the [Euclidean norm](../../../../../../../euclidean-norm.md) in the [surface area](../../../../../../../surface-area.md) formula.

## ↑ Ancestors (13)

1. [i](../i.md)
2. [c](../../c.md)
3. [3](../../../3.md)
4. [Mathematics IV](../../../../mathematics-iv-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
