<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The hard-margin constraints are feasible exactly when the classes are separated by a [separating hyperplane](../../../../../../separating-hyperplane.md). Failure after the corrections in part a therefore means the classes overlap.

Introduce [slack variables of a support vector machine](../../../../../../slack-variables-of-a-support-vector-machine.md) and solve the soft-margin problem

$$
\min_{b,\beta,\xi}
\left\{\frac12\|\beta\|_2^2+C\sum_i\xi_i\right\}
$$

subject to

$$
y_i(b+X_i^T\beta)\geq1-\xi_i,
\qquad \xi_i\geq0.
$$

Large $C$ strongly penalizes violations and approaches the hard-margin solution when separation is possible. Small $C$ tolerates more violations in exchange for a wider, more strongly regularized margin.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
