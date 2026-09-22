<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The multiplication order needs care. Use the standard right-hand [rotation matrices](../../../../../../rotation-matrix.md), consistent with the printed $G$ and the stated positive $z$ [rotation](../../../../../../rotation-mathematics.md). For column [vectors](../../../../../../vector.md), direct multiplication of the two products _in the order printed_ gives

$$
R_y(-\pi/2)R_z(-\pi/2)=\begin{pmatrix}0&0&-1\\-1&0&0\\0&1&0\end{pmatrix},\qquad (x,y,z)\mapsto(-z,-x,y),
$$



$$
R_y(\pi/2)R_z(\pi/2)=\begin{pmatrix}0&0&1\\1&0&0\\0&1&0\end{pmatrix},\qquad (x,y,z)\mapsto(z,x,y).
$$

Both permute the dimensions $(d,w,h)$ into $(h,d,w)$, rather than the required $(w,h,d)$. Therefore, with ordinary column-vector [matrix multiplication](../../../../../../matrix-multiplication.md), **neither printed product is the permutation in part (ii)**. A [translation](../../../../../../translation-geometry.md) can correct the position of a cuboid, but cannot correct these permuted side lengths for general $w,h,d$. This order mismatch is present in the original printed question.[Printed p. 5, Question 2(b)(iii): the products are written with ROT\_y to the left of ROT\_z](../../../../../../computer-graphics-examination-paper-by-the-university-of-oxford-2015.md)

The apparent intended comparison is obtained if “chain” means apply the $y$ [rotation](../../../../../../rotation-mathematics.md) first, then the $z$ [rotation](../../../../../../rotation-mathematics.md). Under that interpretation the actual column-vector products have the reverse order:

$$
\boxed{R_z(-\pi/2)R_y(-\pi/2)=\begin{pmatrix}0&1&0\\0&0&1\\1&0&0\end{pmatrix}=P_{3\times3}.}
$$

Thus the _negative-angle sequence_ is correct when read as operations performed from left to right. The positive-angle sequence gives

$$
R_z(\pi/2)R_y(\pi/2)=\begin{pmatrix}0&-1&0\\0&0&1\\-1&0&0\end{pmatrix},\qquad (x,y,z)\mapsto(-y,z,-x).
$$

It occupies $[-w,0]\times[0,h]\times[-d,0]$. Apply the world-space [translation](../../../../../../translation-geometry.md)

$$
\boxed{t=(w,0,d),\qquad (x',y',z')=(w-y,z,d-x).}
$$

This puts the cuboid in $[0,w]\times[0,h]\times[0,d]$ and still maps $z=k\,\texttt{step}$ to $y'=k\,\texttt{step}$. The distinction is purely the action order: ordinary products act rightmost first, while a library may describe an ordered sequence of operations in application order. Giving the coordinate maps makes either convention explicit. If one merely wanted to place the literal printed negative product in the positive octant, its [translation](../../../../../../translation-geometry.md) would instead be $(h,d,0)$, producing dimensions $(h,d,w)$ and still failing the requested general bounds.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
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
