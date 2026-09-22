<h1 id="30j/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [empirical risk](../../../../../../empirical-risk.md) is

$$
f(\beta)=\frac1n\sum_{i=1}^n\log_2(1+e^{-y_ix_i^T\beta}).
$$

For $g(z)=\log_2(1+e^{-z})$,

$$
g''(z)=\frac{e^z}{\log(2)(1+e^z)^2}\geq0,
$$

so $g$ is a [convex function](../../../../../../convex-function.md). Each signed margin $y_ix_i^T\beta$ is an [affine function](../../../../../../affine-function.md) of $\beta$, and composition with an affine function preserves convexity. Equivalently,

$$
\nabla^2f(\beta)=\frac1n\sum_{i=1}^ng''(y_ix_i^T\beta)x_ix_i^T
$$

is a [positive semidefinite matrix](../../../../../../positive-semidefinite-matrix.md). Therefore $f$ is convex.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [30J](../../30j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
