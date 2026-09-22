<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [finite-dimensional spectral theorem](../../../../../finite-dimensional-spectral-theorem.md) gives a [spectral decomposition](../../../../../spectral-decomposition.md) of the [Hermitian matrix](../../../../../hermitian-operator.md):

$$
A=QDQ^\dagger,\qquad D=\operatorname{diag}(\lambda_1,\ldots,\lambda_n),\quad\lambda_j\in\mathbb R.
$$

The [matrix exponential respects similarity](../../../../../matrix-exponential-respects-similarity.md), so

$$
e^A=Q\operatorname{diag}(e^{\lambda_1},\ldots,e^{\lambda_n})Q^\dagger.
$$

The diagonal entries are real, so the [conjugate transpose](../../../../../conjugate-transpose.md) of this expression equals itself. Its [eigenvalues](../../../../../eigenvalue.md) are $e^{\lambda_j}>0$, proving

$$
\boxed{(e^A)^\dagger=e^A,\qquad \operatorname{spec}(e^A)=\{e^{\lambda_j}\}_j\subset(0,\infty)}.
$$

In particular, for any nonzero $v$, $v^\dagger e^Av=\sum_j e^{\lambda_j}|(Q^\dagger v)_j|^2>0$. Thus the [exponential of a Hermitian matrix](../../../../../exponential-of-a-hermitian-matrix.md) is a [Hermitian positive-definite matrix](../../../../../hermitian-positive-definite-matrix.md), even when $A$ itself has negative [eigenvalues](../../../../../eigenvalue.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
