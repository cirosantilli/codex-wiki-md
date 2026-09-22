<h1 id="p/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [Givens rotation](../../../../givens-rotation.md) acts as the identity except on coordinates $i,j$, where its block can be written

$$
\begin{pmatrix}\cos\theta&\sin\theta\\
-\sin\theta&\cos\theta\end{pmatrix}.
$$

The block has orthonormal columns because $\cos^2\theta+\sin^2\theta=1$ and their inner product is zero, so $J^TJ=I$. For $r=\sqrt{v_i^2+v_j^2}>0$, choose $\cos\theta=v_i/r$, $\sin\theta=v_j/r$. The new coordinates are $(r,0)$, eliminating the $j$th entry. If both entries are zero, the identity already works.

For the specified vector, one suitable matrix is

$$
\boxed{Q=\begin{pmatrix}
4/5&0&-3/5\\3/5&0&4/5\\0&-1&0
\end{pmatrix},\qquad Qv=\begin{pmatrix}0\\5\\0\end{pmatrix}.}
$$

Its rows are orthonormal, so it is orthogonal; in fact its [determinant](../../../../determinant.md) is one. The positive nonzero output component must be five because an [orthogonal matrix](../../../../orthogonal-matrix.md) preserves [Euclidean norm](../../../../euclidean-norm.md).

**The matrix is not unique.** Left multiplication by any [orthogonal matrix](../../../../orthogonal-matrix.md) fixing the second coordinate vector preserves this output. For example arbitrary rotations of the first and third coordinates provide infinitely many alternatives.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [P](../../p.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
