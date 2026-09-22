<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $a_1,\ldots,a_d>0$ be the [eigenvalues](../../../../../eigenvalue.md) of the [positive-definite matrix](../../../../../positive-definite-matrix.md) $V_n$. Its [trace](../../../../../matrix-trace.md) satisfies

$$
\sum_{j=1}^d a_j=\operatorname{tr}V_n
=d\lambda+\sum_{t=1}^n\|X_t\|_2^2\leq d\lambda+n.
$$

The [arithmetic-geometric mean inequality](../../../../../arithmetic-geometric-mean-inequality.md) gives

$$
\det V_n=\prod_{j=1}^d a_j
\leq\left(\frac{\sum_j a_j}{d}\right)^d
\leq\left(\lambda+\frac nd\right)^d.
$$

Since $\det V_0=\lambda^d$, taking the [logarithm](../../../../../logarithm.md) proves

$$
\boxed{\log\frac{\det V_n}{\det V_0}\leq d\log\left(1+\frac{n}{d\lambda}\right).}
$$

The determinant is largest, for a fixed trace, when the eigenvalues are equal; this is the geometric content of the estimate.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the algorithmic foundations of learning course of the University of Oxford](../../../../split.md)
6. [Algorithmic foundations of learning course of the University of Oxford](../../../../../algorithmic-foundations-of-learning-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
