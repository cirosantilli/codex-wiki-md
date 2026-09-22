<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Taking the [conjugate transpose](../../../../../conjugate-transpose.md) term by term in the convergent [matrix exponential](../../../../../matrix-exponential.md) gives

$$
U^\dagger=e^{A^\dagger}=e^{-A}.
$$

The [matrices](../../../../../matrix.md) $A$ and $-A$ [commute](../../../../../commuting-elements.md), so the [matrix exponential](../../../../../matrix-exponential.md) product law gives $U^\dagger U=e^{-A}e^A=I$ and likewise $UU^\dagger=I$. Hence $\boxed{U\text{ is unitary}}$.

For $V$, use the inverse and product rules for the [conjugate transpose](../../../../../conjugate-transpose.md):

$$
V^\dagger=[(I+A)^{-1}]^\dagger(I-A)^\dagger=(I-A)^{-1}(I+A).
$$

The factors $I\pm A$ [commute](../../../../../commuting-elements.md), as do their inverses, since they are expressions in the same [matrix](../../../../../matrix.md). Consequently

$$
V^\dagger V=(I-A)^{-1}(I+A)(I-A)(I+A)^{-1}=I,
$$

and similarly $VV^\dagger=I$. Therefore $\boxed{V\text{ is unitary}}$. This rational construction is the skew-Hermitian form of the [Cayley transform of a Hermitian matrix](../../../../../cayley-transform-of-a-hermitian-matrix.md), obtained by writing $A=iH$ with $H$ a [Hermitian matrix](../../../../../hermitian-operator.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
