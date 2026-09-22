<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Differentiate the squared [Euclidean norm](../../../../../../euclidean-norm.md) and use the [skew-symmetric matrix](../../../../../../skew-symmetric-matrix.md) identity $A^T=-A$:

$$
\frac d{dt}\|\mathbf y(t)\|_2^2
=2\mathbf y^T\mathbf y'
=2\mathbf y^TA(\mathbf y)\mathbf y
=\mathbf y^T(A+A^T)\mathbf y=0.
$$

Thus $\|\mathbf y(t)\|_2^2$ is [constant](../../../../../../constant-mathematics.md), and continuity of the nonnegative [square root](../../../../../../square-root.md) gives

$$
\boxed{\|\mathbf y(t)\|_2=\|\mathbf y_0\|_2\quad(t\geq0).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
