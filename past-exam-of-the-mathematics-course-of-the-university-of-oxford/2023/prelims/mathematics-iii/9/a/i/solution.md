<h1 id="9/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Minimize the [residual sum of squares](../../../../../../../residual-sum-of-squares.md)

$$
Q(b_0,b_1,b_2)=\sum_i(Y_i-b_0-b_1x_{i1}-b_2x_{i2})^2.
$$

Setting its three [partial derivatives](../../../../../../../partial-derivative.md) to zero gives the [normal equations](../../../../../../../normal-equation.md)

$$
\boxed{\sum_i(Y_i-\hat\beta_0-\hat\beta_1x_{i1}-\hat\beta_2x_{i2})=0,\quad
\sum_i x_{ij}(Y_i-\hat\beta_0-\hat\beta_1x_{i1}-\hat\beta_2x_{i2})=0\quad(j=1,2).}
$$

These equations characterize the [linear least squares](../../../../../../../linear-least-squares.md) minimizers, since $Q$ is a convex quadratic. A unique coefficient vector additionally requires full [column rank](../../../../../../../column-rank.md) of the [design matrix](../../../../../../../design-matrix.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [9](../../../9.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
