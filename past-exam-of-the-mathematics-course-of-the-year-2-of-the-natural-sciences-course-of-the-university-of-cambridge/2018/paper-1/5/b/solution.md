<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If $A^\dagger=-A$, then $H=-iA$ is a [Hermitian matrix](../../../../../hermitian-operator.md), because $H^\dagger=iA^\dagger=-iA=H$. By the [finite-dimensional spectral theorem](../../../../../finite-dimensional-spectral-theorem.md), there is a [unitary matrix](../../../../../unitary-matrix.md) $Q$ with

$$
H=Q\operatorname{diag}(\theta_1,\ldots,\theta_n)Q^\dagger,\qquad \theta_j\in\mathbb R.
$$

Thus $A=Q\operatorname{diag}(i\theta_j)Q^\dagger$. Since the [matrix exponential respects similarity](../../../../../matrix-exponential-respects-similarity.md),

$$
\boxed{e^A=QCQ^\dagger,\qquad C=\operatorname{diag}(e^{i\theta_1},\ldots,e^{i\theta_n})}.
$$

Each diagonal entry has modulus one, so $C^\dagger C=I$. Using $Q^\dagger Q=QQ^\dagger=I$,

$$
(e^A)^\dagger e^A=QC^\dagger Q^\dagger QCQ^\dagger=I.
$$

Hence **the [exponential of a skew-Hermitian matrix](../../../../../exponential-of-a-skew-hermitian-matrix.md) is unitary**.

## ↑ Ancestors (13)

1. [B](../b.md)
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
