<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Part (a) makes each $\lambda_j$ real. In the [eigenvector](../../../../../eigenvector.md) basis,

$$
(A+iaI)e_j=(\lambda_j+ia)e_j,
$$

and $|\lambda_j+ia|^2=\lambda_j^2+a^2>0$. Hence $\boxed{A+iaI\text{ is invertible}}$.

All factors that are rational functions of $A$ commute. Taking the [Hermitian conjugate](../../../../../hermitian-conjugation.md) reverses product order and gives

$$
V^\dagger=(A-iaI)^{-1}(A+iaI).
$$

Therefore

$$
V^\dagger V=(A-iaI)^{-1}(A+iaI)(A-iaI)(A+iaI)^{-1}=I,
$$

so $\boxed{V\text{ is unitary}}$. This is a [Cayley transform of a Hermitian matrix](../../../../../cayley-transform-of-a-hermitian-matrix.md), with scale $a$ and the convention that an infinite real eigenvalue maps to one.

Applying it to each [eigenvector](../../../../../eigenvector.md) yields

$$
\boxed{Ve_j=\nu_je_j,\qquad\nu_j=\frac{\lambda_j-ia}{\lambda_j+ia}.}
$$

The [eigenvectors](../../../../../eigenvector.md) are unchanged, and $|\nu_j|=1$ because numerator and denominator are [complex conjugates](../../../../../complex-conjugate.md). No $\nu_j$ equals one when $a>0$. The scalar map is injective on real $\lambda$, so the [eigenspaces](../../../../../eigenspace.md), including any degeneracies, are preserved exactly.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
