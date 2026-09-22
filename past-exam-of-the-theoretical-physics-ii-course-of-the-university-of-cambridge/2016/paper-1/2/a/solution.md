<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume the composite [pure state](../../../../../pure-state.md) has unit norm. Put its amplitudes into the [matrix](../../../../../matrix.md)

$$
C=\begin{pmatrix}a_1&a_2\\a_3&a_4\end{pmatrix},
\qquad |\chi\rangle=\sum_{s,t}C_{st}|s\rangle_A|t\rangle_B.
$$

The [partial trace](../../../../../partial-trace.md) contracts the same $B$ index between ket and bra:

$$
(\rho_A)_{ss'}=\sum_t C_{st}C^*_{s't}.
$$

Thus

$$
\boxed{\rho_A=CC^\dagger=
\begin{pmatrix}
|a_1|^2+|a_2|^2&a_1a_3^*+a_2a_4^*\\
a_1^*a_3+a_2^*a_4&|a_3|^2+|a_4|^2
\end{pmatrix}.}
$$

It is [Hermitian](../../../../../hermitian-operator.md), [positive semidefinite](../../../../../positive-semidefinite-matrix.md) and has [trace](../../../../../matrix-trace.md) one. Its [determinant](../../../../../determinant.md) is particularly useful:

$$
\boxed{\det\rho_A=|\det C|^2=|a_1a_4-a_2a_3|^2.}
$$

This follows from multiplicativity of the [determinant](../../../../../determinant.md), or by expanding the two-by-two expression. If the supplied amplitudes were not normalized, the physical reduced state would be $CC^\dagger/\operatorname{tr}(CC^\dagger)$ instead.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the theoretical physics II course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics II course of the University of Cambridge](../../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
