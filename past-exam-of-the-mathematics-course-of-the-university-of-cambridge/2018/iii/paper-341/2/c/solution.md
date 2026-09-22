<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For [algebraic stability of a Runge-Kutta method](../../../../../../algebraic-stability-of-a-runge-kutta-method.md), the weights must be nonnegative and

$$
M=BA+A^TB-bb^T,\qquad B=\operatorname{diag}(b),
$$

must be a [positive semidefinite matrix](../../../../../../positive-semidefinite-matrix.md). Here all weights are positive, but direct calculation gives

$$
M=\frac1{36}\begin{pmatrix}-1&1&0\\1&0&-1\\0&-1&1\end{pmatrix}.
$$

In particular $e_1^TMe_1=-1/36<0$; equivalently, its [eigenvalues](../../../../../../eigenvalue.md) are $0,\pm\sqrt3/36$. Therefore **the method is not [algebraically stable](../../../../../../algebraic-stability-of-a-runge-kutta-method.md)**. This does not contradict its [A-stability](../../../../../../a-stability.md): [algebraic stability](../../../../../../algebraic-stability-of-a-runge-kutta-method.md) is a stronger condition designed to guarantee nonlinear [B-stability](../../../../../../b-stability.md) through the [Runge-Kutta contractivity identity](../../../../../../runge-kutta-contractivity-identity.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
