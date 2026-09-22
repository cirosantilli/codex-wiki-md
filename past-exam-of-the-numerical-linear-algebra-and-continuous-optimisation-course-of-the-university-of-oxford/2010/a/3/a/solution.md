<h1 id="a/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The off-diagonal [Toeplitz matrix](../../../../../toeplitz-matrix.md) $T=A-I$ is symmetric and has row and column absolute sums bounded by

$$
r=2\sum_{j=2}^m|t_j|\leq\frac23.
$$

For an elementary Euclidean bound, apply the weighted [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) in each row:

$$
|(Tx)_i|^2\leq\left(\sum_j|T_{ij}|\right)\left(\sum_j|T_{ij}|\,|x_j|^2\right).
$$

Sum over $i$ and use both absolute-sum bounds to get $\|Tx\|_2^2\leq r^2\|x\|_2^2$. Therefore

$$
\boxed{\|T\|_2\leq2\sum_{j=2}^m|t_j|\leq\frac23.}
$$

The entry $t_1$ is unused because the diagonal of $A$ is fixed to one; including it only weakens the bound. This is the [row-column bound for the matrix 2-norm](../../../../../row-column-bound-for-the-matrix-2-norm.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
