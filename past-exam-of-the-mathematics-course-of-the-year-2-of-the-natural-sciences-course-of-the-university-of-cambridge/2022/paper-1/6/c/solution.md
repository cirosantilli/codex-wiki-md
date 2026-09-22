<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

To avoid confusing the diagonalizing [matrix](../../../../../matrix.md) with the exponential, write $A=WDW^\dagger$ from part (b). The convergent [matrix exponential](../../../../../matrix-exponential.md) series gives

$$
E=e^A=W e^D W^\dagger=W\operatorname{diag}(e^{\lambda_1},\ldots,e^{\lambda_n})W^\dagger.
$$

Each $\lambda_j$ is purely imaginary, so $|e^{\lambda_j}|=1$. The diagonal exponential is therefore a [unitary matrix](../../../../../unitary-matrix.md), and

$$
\boxed{E^\dagger E=W\operatorname{diag}(|e^{\lambda_j}|^2)W^\dagger=I.}
$$

Hence the matrix called $U=\exp(A)$ in this part is unitary. The series identity $(e^A)^\dagger=e^{A^\dagger}=e^{-A}$ gives the same conclusion directly and also covers repeated [eigenvalues](../../../../../eigenvalue.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
