<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $A_n=A(\mathbf y_n)$. The [trapezoidal rule](../../../../../../trapezoidal-rule.md) is

$$
\mathbf y_{n+1}-\mathbf y_n
=\frac h2(A_n\mathbf y_n+A_{n+1}\mathbf y_{n+1}).
$$

Taking the [inner product](../../../../../../inner-product.md) with $\mathbf y_{n+1}+\mathbf y_n$ gives

$$
\begin{aligned}
\|\mathbf y_{n+1}\|_2^2-\|\mathbf y_n\|_2^2
=\frac h2\bigl(&\mathbf y_{n+1}^TA_n\mathbf y_n
+\mathbf y_n^TA_{n+1}\mathbf y_{n+1}\\
&+\mathbf y_n^TA_n\mathbf y_n
+\mathbf y_{n+1}^TA_{n+1}\mathbf y_{n+1}\bigr).
\end{aligned}
$$

The two quadratic terms vanish because each $A_j$ is [skew-symmetric](../../../../../../skew-symmetric-matrix.md). Moreover $\mathbf y_{n+1}^TA_n\mathbf y_n=-\mathbf y_n^TA_n\mathbf y_{n+1}$. Hence

$$
\boxed{
\|\mathbf y_{n+1}\|_2^2-\|\mathbf y_n\|_2^2
=\frac h2\mathbf y_n^T(A_{n+1}-A_n)\mathbf y_{n+1}.}
$$

Unlike the [implicit midpoint rule](../../../../../../implicit-midpoint-rule.md), the trapezoidal rule evaluates $A$ at two different states, so the mixed terms need not cancel.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
