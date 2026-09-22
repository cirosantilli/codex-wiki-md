<h1 id="4h/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let

$$
L_1=\{w^n:w\in\{a,b\}^*,\ n\geq2\}.
$$

Intersect it with the [regular language](../../../../../../../regular-language.md)

$$
R=a^+ba^+b.
$$

Every word of $R$ contains exactly two copies of $b$. If it is a proper power, its exponent must therefore be two and its root must contain one $b$. Hence

$$
L_1\cap R=\{a^mba^mb:m\geq1\}.
$$

This language is not regular: if $p$ were a [pumping length](../../../../../../../pumping-length.md), pumping any nonempty substring among the first $p$ copies of $a$ in $a^pba^pb$ would change only its first $a$-block. Since regular languages are closed under intersection,

$$
\boxed{L_1\text{ is not regular}.}
$$

This is the [proper-power language is not regular](../../../../../../../proper-power-language-is-not-regular.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [4H](../../../4h.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
