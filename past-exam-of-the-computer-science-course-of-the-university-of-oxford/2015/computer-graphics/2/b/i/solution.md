<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In the solid-modelling convention used here, a [rigid-body transformation](../../../../../../rigid-body-transformation.md) is an orientation-preserving [rigid transformation](../../../../../../rigid-transformation.md), represented by a [proper rotation](../../../../../../proper-rotation.md) and a [translation](../../../../../../translation-geometry.md). The proposed upper-left block $S$ is [orthogonal](../../../../../../orthogonal-vectors.md) but has

$$
S=\begin{pmatrix}0&1&0\\1&0&0\\0&0&1\end{pmatrix},\qquad S^TS=I,\qquad \det S=-1.
$$

It is a [reflection](../../../../../../reflection-mathematics.md) in the [plane](../../../../../../plane.md) $x=y$. It preserves distances, but reverses handedness, so it cannot describe continuous motion of a rigid solid through [proper rotations](../../../../../../proper-rotation.md) and [translations](../../../../../../translation-geometry.md). Some mathematical uses of [rigid transformation](../../../../../../rigid-transformation.md) include this orientation-reversing case; the [determinant](../../../../../../determinant.md) is the distinction relevant to the warning.

In a solid modeller, [triangle](../../../../../../triangle.md) winding and outward [normal vectors](../../../../../../normal-vector.md) must agree. A [reflection](../../../../../../reflection-mathematics.md) reverses the winding: for edge [vectors](../../../../../../vector.md) $a,b$,

$$
(Sa)\times(Sb)=\det(S)S(a\times b)=-S(a\times b).
$$

Simply transforming stored [normal vectors](../../../../../../normal-vector.md) by $S$ while retaining the original vertex order therefore makes the geometric and stored normals disagree. [Back-face culling](../../../../../../back-face-culling.md), inside/outside tests and [Phong reflection model](../../../../../../phong-reflection-model.md) calculations can then use the wrong side. Code assuming a positive oriented volume can likewise interpret the reflected solid incorrectly. A modeller can support [reflections](../../../../../../reflection-mathematics.md) if it deliberately corrects these orientation conventions.

A suitable alternative rotates by $-\pi/2$ about $z$ and then translates upward by `height`. Writing $h=\texttt{height}$,

$$
\boxed{T=\begin{pmatrix}0&1&0&0\\-1&0&0&h\\0&0&1&0\\0&0&0&1\end{pmatrix},\qquad (x,y,z)\mapsto(y,h-x,z).}
$$

Its [rotation matrix](../../../../../../rotation-matrix.md) has determinant $+1$. The source bounds $0\leq x\leq h$, $0\leq y\leq w$, $z=0$ become $0\leq x'\leq w$, $0\leq y'\leq h$, $z'=0$, where $w=\texttt{width}$. A horizontal stripe $y=k\,\texttt{step}$ becomes the vertical stripe $x'=k\,\texttt{step}$, so even the stripe positions from the left edge are preserved. The face's $+z$ [normal vector](../../../../../../normal-vector.md) is also preserved.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Computer graphics](../../../../computer-graphics-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
