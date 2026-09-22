<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Algebraic stability](../../../../../../algebraic-stability-of-a-runge-kutta-method.md) requires $b_i\geq0$ and positive semidefiniteness of

$$
\mathcal M=BA+A^TB-bb^T,\qquad B=\operatorname{diag}(b).
$$

The three weights are positive, but direct calculation gives

$$
\mathcal M_{11}=2b_1a_{11}-b_1^2=-\frac1{81}<0.
$$

A positive-semidefinite matrix cannot have a negative diagonal entry. Hence

$$
\boxed{\text{the method is not algebraically stable}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
