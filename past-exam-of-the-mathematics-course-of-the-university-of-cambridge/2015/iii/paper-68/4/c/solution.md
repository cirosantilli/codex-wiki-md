<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The criterion for [algebraic stability of a Runge-Kutta method](../../../../../../algebraic-stability-of-a-runge-kutta-method.md) is $b_i\geq0$ and positive semidefiniteness of

$$
 M=BA+A^TB-bb^T,\qquad B=\operatorname{diag}(b).
$$

The [Runge-Kutta contractivity identity](../../../../../../runge-kutta-contractivity-identity.md) implies that this criterion is sufficient for [B-stability](../../../../../../b-stability.md), namely contractivity for a [dissipative vector field](../../../../../../dissipative-vector-field.md), whenever the stage equations are defined. The implication from [algebraic stability](../../../../../../algebraic-stability-of-a-runge-kutta-method.md) to [B-stability](../../../../../../b-stability.md) is the relevant nonlinear theorem; [A-stability](../../../../../../a-stability.md) alone is a linear property.

All weights here are positive, but

$$
 M=\frac1{36}\begin{pmatrix}-1&1&0\\1&0&-1\\0&-1&1\end{pmatrix},
 \qquad e_1^TMe_1=-\frac1{36}<0.
$$

A [positive semidefinite matrix](../../../../../../positive-semidefinite-matrix.md) cannot have this negative quadratic value. Hence **the method is not [algebraically stable](../../../../../../algebraic-stability-of-a-runge-kutta-method.md)**. Failure of this sufficient criterion alone would not be a proof of failure of [B-stability](../../../../../../b-stability.md); no such converse is needed for the question.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Section A](../../section-a.md)
4. [Paper 68](../../../paper-68-split.md)
5. [Iii](../../../split.md)
6. [2015](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
