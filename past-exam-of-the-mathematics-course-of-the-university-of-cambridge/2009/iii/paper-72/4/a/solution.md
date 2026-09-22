<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an $s$-stage [Runge-Kutta method](../../../../../../runge-kutta-method.md) with coefficient [matrix](../../../../../../matrix.md) $A=(a_{ij})$ and weights $b=(b_i)$, put $B=\operatorname{diag}(b_i)$. It is [algebraically stable](../../../../../../algebraic-stability-of-a-runge-kutta-method.md) when

$$
\boxed{b_i\geq0\quad\text{for every }i,\qquad
M=BA+A^TB-bb^T\succeq0.}
$$

Equivalently, $m_{ij}=b_ia_{ij}+b_ja_{ji}-b_ib_j$ defines a [positive semidefinite](../../../../../../positive-semidefinite-matrix.md) symmetric [matrix](../../../../../../matrix.md). The condition concerns the full coefficient tableau and nonlinear contractivity, not merely the scalar [stability function](../../../../../../stability-function.md). It is normally used with a consistent [Runge-Kutta method](../../../../../../runge-kutta-method.md) and stage equations satisfying the necessary [stage solvability of an implicit Runge-Kutta method](../../../../../../stage-solvability-of-an-implicit-runge-kutta-method.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
