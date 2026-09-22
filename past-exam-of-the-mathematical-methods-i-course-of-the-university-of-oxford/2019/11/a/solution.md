<h1 id="11/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a finite [matrix](../../../../matrix.md), the series defining the [matrix exponential](../../../../matrix-exponential.md) converges absolutely in any [matrix norm](../../../../matrix-norm.md), because $\|A^m/m!\|\leq\|A\|^m/m!$. Thus the [Hermitian adjoint](../../../../adjoint-operator.md) may be taken term by term. Since $A^\dagger=A$,

$$
(e^A)^\dagger=\sum_{m=0}^\infty\frac{(A^m)^\dagger}{m!}
=\sum_{m=0}^\infty\frac{(A^\dagger)^m}{m!}
=\sum_{m=0}^\infty\frac{A^m}{m!}=e^A.
$$

Therefore the [matrix exponential](../../../../matrix-exponential.md) of a [Hermitian matrix](../../../../hermitian-operator.md) is Hermitian.

If $A=\operatorname{diag}(a_1,\ldots,a_n)$ is a [diagonal matrix](../../../../diagonal-matrix.md), then $A^m=\operatorname{diag}(a_1^m,\ldots,a_n^m)$. Summing each entry separately gives

$$
\boxed{e^A=\operatorname{diag}(e^{a_1},\ldots,e^{a_n}),\qquad(e^A)_{ij}=\delta_{ij}e^{a_i}.}
$$

For the [Hermitian matrix](../../../../hermitian-operator.md) case each $a_i$ is real. The diagonal entry formula itself remains valid for complex diagonal entries.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [11](../../11.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../b/solution.md)
