<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a real [skew-symmetric matrix](../../../../../../skew-symmetric-matrix.md), $P^T=-P$. A scalar quadratic form satisfies $y^TPy=(y^TPy)^T=y^TP^Ty=-y^TPy$, so it is zero. Therefore

$$
\frac d{dt}\lVert y(t)\rVert^2=2y^Ty'=2y^TPy=0,\qquad\boxed{\lVert y(t)\rVert=\lVert y_0\rVert\quad(t\geq0).}
$$

The finite-dimensional linear system has the global solution $e^{tP}y_0$. Equivalently, $(e^{tP})^Te^{tP}=e^{-tP}e^{tP}=I$, so its exact flow is an [orthogonal matrix](../../../../../../orthogonal-matrix.md) and preserves the [Euclidean norm](../../../../../../euclidean-norm.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
