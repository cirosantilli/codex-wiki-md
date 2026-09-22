<h1 id="algebra/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

**$\dim_{\mathbb R}V=4$.** For arbitrary matrices,

$$
\langle A\mid B\rangle=\operatorname{tr}(A^tB)=\sum_{i,j=1}^2a_{ij}b_{ij}.
$$

This is [bilinear](../../../../bilinear-map.md) and [symmetric](../../../../symmetric-relation.md). Also $\langle A\mid A\rangle=\sum_{i,j}a_{ij}^2\geq0$, with equality exactly when every entry vanishes. Thus it is an [inner product](../../../../inner-product-split.md), the [Frobenius inner product](../../../../frobenius-inner-product.md).

If $S^t=S$ and $K^t=-K$, invariance of [trace](../../../../matrix-trace.md) under transposition and cyclicity give

$$
\langle S\mid K\rangle=\operatorname{tr}(SK)=\operatorname{tr}((SK)^t)=-\operatorname{tr}(KS)=-\operatorname{tr}(SK)=0.
$$

Furthermore $\langle I\mid A\rangle=\operatorname{tr}A$, so every traceless [matrix](../../../../matrix.md) is [orthogonal](../../../../orthogonal-vectors.md) to the identity. One convenient [orthonormal basis](../../../../orthonormal-basis.md) adapted to these observations is

$$
\boxed{\frac1{\sqrt2}\begin{pmatrix}1&0\\0&1\end{pmatrix},\quad\frac1{\sqrt2}\begin{pmatrix}1&0\\0&-1\end{pmatrix},\quad\frac1{\sqrt2}\begin{pmatrix}0&1\\1&0\end{pmatrix},\quad\frac1{\sqrt2}\begin{pmatrix}0&1\\-1&0\end{pmatrix}.}
$$

Their entrywise inner products are zero in distinct pairs and one on the diagonal; four orthonormal vectors in this four-dimensional space form a [basis](../../../../basis.md).

## ↑ Ancestors (12)

1. [1](../1.md)
2. [Algebra](../../algebra.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
