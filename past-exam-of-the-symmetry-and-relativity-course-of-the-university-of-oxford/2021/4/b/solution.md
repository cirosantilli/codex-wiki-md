<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an active clockwise [rotation](../../../../rotation-mathematics.md) of column [vectors](../../../../vector.md) in the usual oriented $xy$ plane, take

$$
R_{\rm cw}(\theta)=\begin{pmatrix}\cos\theta&\sin\theta\\-\sin\theta&\cos\theta\end{pmatrix}.
$$

Direct [matrix multiplication](../../../../matrix-multiplication.md) gives

$$
R_{\rm cw}^TR_{\rm cw}
=\begin{pmatrix}\cos^2\theta+\sin^2\theta&0\\0&\cos^2\theta+\sin^2\theta\end{pmatrix}
=I.
$$

Thus the [rotation matrix](../../../../rotation-matrix.md) is an [orthogonal matrix](../../../../orthogonal-matrix.md), preserving the Euclidean [inner product](../../../../inner-product-split.md), with [determinant](../../../../determinant.md) $+1$.

For a passive one-dimensional [Lorentz boost](../../../../lorentz-boost.md), use [rapidity](../../../../rapidity.md) $\eta$, $\beta=\tanh\eta$:

$$
\Lambda(\eta)=\begin{pmatrix}\cosh\eta&-\sinh\eta\\-\sinh\eta&\cosh\eta\end{pmatrix},\qquad
\Lambda^T\Lambda=\begin{pmatrix}\cosh2\eta&-\sinh2\eta\\-\sinh2\eta&\cosh2\eta\end{pmatrix}.
$$

This is not $I$ unless $\eta=0$. Hence a nontrivial [Lorentz boost](../../../../lorentz-boost.md) is not an [orthogonal matrix](../../../../orthogonal-matrix.md) for the Euclidean [inner product](../../../../inner-product-split.md). Instead it preserves the [Minkowski metric](../../../../minkowski-metric.md):

$$
\boxed{\Lambda^Tg\Lambda=g,\qquad g=\operatorname{diag}(-1,1),}
$$

by $\cosh^2\eta-\sinh^2\eta=1$. Thus it is pseudo-orthogonal. The zero-[rapidity](../../../../rapidity.md) identity is the explicit exception to the assertion that a [Lorentz boost](../../../../lorentz-boost.md) is not orthogonal.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the symmetry and relativity course of the University of Oxford](../../../split.md)
5. [Symmetry and relativity course of the University of Oxford](../../../../symmetry-and-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
