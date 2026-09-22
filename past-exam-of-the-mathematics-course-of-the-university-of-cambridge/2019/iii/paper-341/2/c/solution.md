<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For [algebraic stability](../../../../../../algebraic-stability-of-a-runge-kutta-method.md), the weights must be nonnegative and the real [symmetric matrix](../../../../../../symmetric-matrix.md) $M=BA+A^TB-bb^T$, where $B=\operatorname{diag}(b)$, must be a [positive semidefinite matrix](../../../../../../positive-semidefinite-matrix.md).

The weights are positive, but $a_{11}=0$ and $b_1=1/6$, so

$$
M_{11}=2b_1a_{11}-b_1^2=-\frac1{36}<0.
$$

A [positive semidefinite matrix](../../../../../../positive-semidefinite-matrix.md) cannot have a negative diagonal entry, as its [quadratic form](../../../../../../quadratic-form.md) at the first [standard basis](../../../../../../standard-basis.md) vector would be negative. Thus this [Lobatto IIIA method](../../../../../../lobatto-iiia-method.md) is **not [algebraically stable](../../../../../../algebraic-stability-of-a-runge-kutta-method.md)**, despite its [A-stability](../../../../../../a-stability.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
