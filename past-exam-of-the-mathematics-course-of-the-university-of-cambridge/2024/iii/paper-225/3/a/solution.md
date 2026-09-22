<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The minimizer is the arithmetic mean

$$
\overline C=\frac1n\sum_{k=1}^nC_k.
$$

It remains a positive self-adjoint trace-class operator and hence a [covariance operator](../../../../../../covariance-operator.md). The [Hilbert-Schmidt inner product](../../../../../../hilbert-schmidt-inner-product.md) gives, for every Hilbert-Schmidt operator $C$,

$$
\sum_{k=1}^n\lVert C_k-C\rVert_{\mathrm{HS}}^2
=\sum_{k=1}^n\lVert C_k-\overline C\rVert_{\mathrm{HS}}^2
+n\lVert C-\overline C\rVert_{\mathrm{HS}}^2,
$$

because $\sum_k(C_k-\overline C)=0$. Thus $\overline C$ is the unique minimizer, including when the minimization is restricted to covariance operators.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 225](../../../paper-225-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
