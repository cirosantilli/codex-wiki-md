<h1 id="p/p1/solution">Solution</h1>

↑ **Parent:** [P1](../p1.md)

A [Givens rotation](../../../../givens-rotation.md) equals the identity except in coordinates $i,j$, where its block can be taken as

$$
\begin{pmatrix}c&s\\-s&c\end{pmatrix},\qquad c=\cos\theta,\ s=\sin\theta.
$$

The two block columns are orthonormal because $c^2+s^2=1$; other coordinates are unchanged, so the full matrix is [orthogonal](../../../../orthogonal-vectors.md). If $(v_i,v_j)\ne(0,0)$, take $r=\sqrt{v_i^2+v_j^2}$, $c=v_i/r$ and $s=v_j/r$. The transformed pair is $(r,0)$. If both entries are zero, the identity already suffices.

For the specified vector one possible matrix is

$$
\boxed{Q=\begin{pmatrix}4/5&0&-3/5\\3/5&0&4/5\\0&-1&0\end{pmatrix},\qquad Qv=\begin{pmatrix}0\\5\\0\end{pmatrix}}.
$$

Its rows are orthonormal. It is **not unique**: premultiply by any [orthogonal](../../../../orthogonal-vectors.md) transformation fixing the second coordinate axis pointwise. This rotates or reflects the other two output coordinates without changing the required image. Equivalently its second row must be $v^T/\|v\|$, but any orthonormal completion of that row works.

## ↑ Ancestors (12)

1. [P1](../p1.md)
2. [P](../../p.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
