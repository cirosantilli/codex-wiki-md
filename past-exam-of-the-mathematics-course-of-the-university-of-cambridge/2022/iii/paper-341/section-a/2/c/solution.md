<h1 id="section-a/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For [algebraic stability of a Runge-Kutta method](../../../../../../../algebraic-stability-of-a-runge-kutta-method.md), the weights must be nonnegative and

$$
M=BA+A^TB-bb^T,
\qquad B=\operatorname{diag}(b_1,b_2),
$$

must be [positive semidefinite](../../../../../../../positive-semidefinite-matrix.md). With the intended collocation weights,

$$
\det M=-\frac{(3\alpha-1)^2}{16(\alpha-1)^2}.
$$

Positive semidefiniteness is therefore possible only at $\alpha=1/3$; substitution gives nonnegative weights and a positive-semidefinite $M$. Hence the intended family is algebraically stable exactly when

$$
\boxed{\alpha=\frac13.}
$$

With the sign printed in the paper, one instead obtains

$$
M_{22}=-\frac{3(2\alpha-1)^2}{4(\alpha-1)^2}\leq0.
$$

Equality forces $\alpha=1/2$, where $M$ still has nonzero off-diagonal entries and is indefinite. The literal printed tableau is consequently algebraically stable for no value of $\alpha$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Section A](../../../section-a.md)
4. [Paper 341](../../../../paper-341-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
