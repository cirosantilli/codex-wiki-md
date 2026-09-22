<h1 id="19d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Givens rotation](../../../../../../givens-rotation.md) is the identity outside rows and columns $p,q$, with the $2\times2$ block

$$
\begin{pmatrix}c&s\\-s&c\end{pmatrix},\qquad c^2+s^2=1.
$$

The block's transpose times itself is the identity, so the whole matrix satisfies $\boxed{\Omega^T\Omega=I}$ and is an [orthogonal matrix](../../../../../../orthogonal-matrix.md). In particular it preserves the [Euclidean norm](../../../../../../euclidean-norm.md). To annihilate the lower entry of a column pair $(a,b)^T$, take $c=a/r$, $s=b/r$, $r=\sqrt{a^2+b^2}$; the rotated pair is $(r,0)^T$. If both entries are zero, take the identity rotation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [19D](../../19d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
