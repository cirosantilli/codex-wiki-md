# Change-of-basis matrix

↑ **Parent:** [Change of basis](change-of-basis.md)

Fix the convention: the columns of the [change-of-basis matrix](change-of-basis-matrix.md) $P$ are the new [basis vectors](basis-vector.md) written in the old [basis](basis.md). Thus $P$ converts new [coordinate vectors](coordinate-vector.md) into old ones; its [matrix inverse](matrix-inverse-split.md) converts old [coordinate vectors](coordinate-vector.md) into new ones. For the preceding [basis](basis.md),

$$
P=\begin{pmatrix}1&1\\1&-1\end{pmatrix},\qquad
P^{-1}=\frac12\begin{pmatrix}1&1\\1&-1\end{pmatrix},\qquad
P^{-1}\begin{pmatrix}2\\0\end{pmatrix}=\begin{pmatrix}1\\1\end{pmatrix}.
$$

Its [determinant](determinant.md) is $-2$, so $P$ is an [invertible matrix](invertible-matrix.md). Checking which direction $P$ converts is essential: different books may call either $P$ or $P^{-1}$ the [change-of-basis matrix](change-of-basis-matrix.md).

For a [linear operator](linear-operator.md), convert the input into the old [basis](basis.md), apply the old [matrix](matrix.md), and convert the output back. Reading that sequence from right to left gives

$$
A_{\rm new}=P^{-1}A_{\rm old}P.
$$

For example, let the old [diagonal matrix](diagonal-matrix.md) stretch horizontal components by $2$ and vertical components by $3$. Then

$$
A_{\rm old}=\begin{pmatrix}2&0\\0&3\end{pmatrix},\qquad
A_{\rm new}=\begin{pmatrix}2.5&-0.5\\-0.5&2.5\end{pmatrix},\qquad
A_{\rm new}\begin{pmatrix}1\\1\end{pmatrix}=\begin{pmatrix}2\\2\end{pmatrix}.
$$

The output represents $2u+2v=(4,0)$, just as $A_{\rm old}(2,0)^T=(4,0)^T$. The [matrices](matrix.md) look different because their [bases](basis.md) differ, but they encode the same [linear operator](linear-operator.md). This relation is called [matrix similarity](matrix-similarity.md); it preserves the underlying action.[Strang, Lecture 31 transcript: coordinate conversion and similar matrices](https://ocw.mit.edu/courses/18-06-linear-algebra-spring-2010/46108efb43dcf33e989eb5e101fcf9b5_MIT18_06S10_L31.pdf)

## ↑ Ancestors (6)

1. [Change of basis](change-of-basis.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (14)

- [Change-of-basis matrix](change-of-basis-matrix.md)
- [Determinant of a complex block representation](determinant-of-a-complex-block-representation.md)
- [Matrix inverse](matrix-inverse-split.md)
- [Matrix similarity](matrix-similarity.md)
- [Matrix trace](matrix-trace.md)
- [Passive rotation of coordinates](passive-rotation-of-coordinates.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-4/6c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1/7b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-1/1a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-1/1a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-1/8b/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-2/10g/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-1/6b/solution.md)
- [Similarity transformation](similarity-transformation.md)
