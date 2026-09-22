<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The call constructs dimensions $(d,w,h)$ along the old $(x,y,z)$ axes. To obtain target dimensions $(w,h,d)$ and make an old layer $z=k\,\texttt{step}$ become a new layer $y'=k\,\texttt{step}$, use the cyclic permutation

$$
\boxed{P=\begin{pmatrix}0&1&0&0\\0&0&1&0\\1&0&0&0\\0&0&0&1\end{pmatrix},\qquad (x,y,z)\mapsto(y,z,x).}
$$

The new coordinate ranges are immediately $[0,w]$, $[0,h]$, $[0,d]$. Its spatial block is [orthogonal](../../../../../../orthogonal-vectors.md) with determinant $+1$, since a three-cycle is an even [permutation](../../../../../../permutation.md). Hence this is a [proper rotation](../../../../../../proper-rotation.md), through $-2\pi/3$ about the axis in direction $(1,1,1)$ under the right-hand convention. No [translation](../../../../../../translation-geometry.md) is required.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
