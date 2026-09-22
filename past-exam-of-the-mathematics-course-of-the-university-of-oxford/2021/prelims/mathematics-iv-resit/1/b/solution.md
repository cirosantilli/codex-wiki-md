<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Decompose $\mathbf v$ by [orthogonal projection](../../../../../../orthogonal-projection.md) onto the [straight line](../../../../../../straight-line.md) spanned by $\mathbf n$ and its [orthogonal complement](../../../../../../orthogonal-complement.md):

$$
\mathbf v=(\mathbf v\cdot\mathbf n)\mathbf n+\mathbf w,\qquad \mathbf w=\mathbf n\times(\mathbf v\times\mathbf n).
$$

The first term is fixed by the [rotation](../../../../../../rotation-mathematics.md). If $\mathbf w\ne0$, the [vectors](../../../../../../vector.md) $\mathbf w/|\mathbf w|$ and $(\mathbf n\times\mathbf w)/|\mathbf w|$ form an [orthonormal basis](../../../../../../orthonormal-basis.md) of the perpendicular [plane](../../../../../../plane.md), oriented in the positive sense about $\mathbf n$. A [planar rotation](../../../../../../planar-rotation.md) through $\theta$ therefore sends

$$
\mathbf w\longmapsto\cos\theta\,\mathbf w+\sin\theta\,(\mathbf n\times\mathbf w).
$$

Here $\mathbf n\times\mathbf w=\mathbf n\times\mathbf v$. Adding the fixed parallel component proves the [Rodrigues rotation formula](../../../../../../rodrigues-rotation-formula.md) in the required form:

$$
\boxed{R(\mathbf v)=(\mathbf v\cdot\mathbf n)\mathbf n+\sin\theta(\mathbf n\times\mathbf v)+\cos\theta\bigl(\mathbf n\times(\mathbf v\times\mathbf n)\bigr).}
$$

When $\mathbf w=0$, both perpendicular terms vanish, so the same formula fixes $\mathbf v$ as required. Positive [angles](../../../../../../angle.md) use the right-hand convention about $\mathbf n$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Mathematics IV resit](../../../mathematics-iv-resit-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
