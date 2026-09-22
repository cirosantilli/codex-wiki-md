# Change of basis

↑ **Parent:** [Linear algebra](linear-algebra-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Change_of_basis)

A [change of basis](change-of-basis.md) rewrites a [vector](vector.md) using a different [ordered basis](ordered-basis.md) of the same [vector space](vector-space-split.md). The [vector](vector.md) stays fixed; its [coordinate vector](coordinate-vector.md) changes because the measuring directions change. Both [bases](basis.md) must describe every [vector](vector.md) uniquely, so a [change of basis](change-of-basis.md) is reversible.

Start with the [Cartesian basis](cartesian-basis.md) $e_1=(1,0)$, $e_2=(0,1)$, and choose the new [basis vectors](basis-vector.md) $u=(1,1)$ and $v=(1,-1)$. For the [vector](vector.md) $z=(2,0)$,

$$
z=2e_1+0e_2=u+v,\qquad
[z]_{\rm old}=\begin{pmatrix}2\\0\end{pmatrix},\qquad
[z]_{\rm new}=\begin{pmatrix}1\\1\end{pmatrix}.
$$

The second [coordinate vector](coordinate-vector.md) says to travel once along $u$ and once along $v$. Their vertical contributions cancel, leaving exactly the original horizontal arrow. The diagram shows two descriptions of that same arrow, with the same origin and endpoint.

<a id="image-the-same-vector-expressed-in-two-bases-2e-1-u-plus-v"></a>
![](change-of-basis-coordinates.png)

**[Figure 13](#image-the-same-vector-expressed-in-two-bases-2e-1-u-plus-v). The same vector expressed in two bases: $2e_1=u+v$**.

Choosing a useful [basis](basis.md) can reveal simple structure hidden by the old [coordinate vectors](coordinate-vector.md). Here the new [basis](basis.md) describes common and opposing contributions. For two equal measurements $(5,5)$, the new [coordinate vector](coordinate-vector.md) is $(5,0)$: only the common contribution is present. In larger examples, a suitable [basis](basis.md) can concentrate important information into a few [coefficients](coefficient.md). Strang's lecture on [change of basis](change-of-basis.md) develops this principle through applications: the reversible [change of basis](change-of-basis.md) preserves information, while subsequently discarding small [coefficients](coefficient.md) loses information.[Strang, Lecture 31: Change of basis; image compression](https://ocw.mit.edu/courses/18-06-linear-algebra-spring-2010/resources/lecture-31-change-of-basis-image-compression/)

**Table of contents**

- [Orthogonal change of coordinates](orthogonal-change-of-coordinates.md)
- [Change-of-basis matrix](change-of-basis-matrix.md)

## ↑ Ancestors (5)

1. [Linear algebra](linear-algebra-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (27)

- [Cartesian basis under rotation](cartesian-basis-under-rotation.md)
- [Change of basis](change-of-basis.md)
- [Circulant matrix](circulant-matrix.md)
- [Coordinate vector](coordinate-vector.md)
- [Covector](covector.md)
- [Diagonalizable matrix](diagonalizable-matrix.md)
- [Equivalent sheared representations of the Klein four-group](equivalent-sheared-representations-of-the-klein-four-group.md)
- [Four-dimensional symplectic basis change](four-dimensional-symplectic-basis-change.md)
- [Linear algebra](linear-algebra-split.md)
- [Matrix congruence](matrix-congruence.md)
- [Matrix of a bilinear form](matrix-of-a-bilinear-form.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-1/5c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-1/1b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-1/1a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-1/1a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-1/2a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-1/6a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-3/11c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-1/2b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-4/8e/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-2/8f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-2/10/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1/5/a/solution.md)
- [Similarity and the coordinate metric](similarity-and-the-coordinate-metric.md)
- [Symmetric bilinear form](symmetric-bilinear-form.md)
- [Vector space](vector-space-split.md)
