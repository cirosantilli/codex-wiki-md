<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Givens rotation](../../../../givens-rotation.md) acts as the [identity matrix](../../../../identity-matrix.md) outside two selected coordinates $i,j$, and has the following block on those coordinates:

$$
\boxed{G_{\{i,j\},\{i,j\}}=\begin{pmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{pmatrix}.}
$$

The convention with the opposite signs of the sines is equivalent after replacing $\theta$ by $-\theta$. A [Householder reflection](../../../../householder-transformation.md) with nonzero normal [vector](../../../../vector.md) $w\in\mathbb R^n$ is

$$
\boxed{H(w)=I-\frac{2ww^T}{w^Tw}.}
$$

It reverses the component parallel to $w$ and fixes the perpendicular [hyperplane](../../../../hyperplane.md). Both are [orthogonal matrices](../../../../orthogonal-matrix.md), so their transposes are their inverses and they preserve the [Euclidean norm](../../../../euclidean-norm.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
