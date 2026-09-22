<h1 id="2/2/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

[Algebraic stability of a Runge-Kutta method](../../../../../../../algebraic-stability-of-a-runge-kutta-method.md) requires $b_i\geq0$ and a positive-semidefinite symmetric [matrix](../../../../../../../matrix.md)

$$
M_{ij}=b_i a_{ij}+b_j a_{ji}-b_i b_j.
$$

Although all weights are positive, its first diagonal entry is

$$
M_{11}=2b_1a_{11}-b_1^2=-\frac1{36}.
$$

The quadratic form on the first coordinate vector is negative, so $M$ cannot be [positive semidefinite](../../../../../../../positive-semidefinite-matrix.md). **The method is not algebraically stable.** This distinguishes nonlinear contractivity from the [A-stability](../../../../../../../a-stability.md) proved in part 2.

## ↑ Ancestors (13)

1. [3](../3.md)
2. [2](../../2.md)
3. [2](../../../2.md)
4. [Section I](../../../section-i.md)
5. [Paper 69](../../../../paper-69-split.md)
6. [Iii](../../../../split.md)
7. [2012](../../../../../split.md)
8. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
9. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
