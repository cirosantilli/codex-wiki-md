<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The finite [sigma-algebra](../../../../../../sigma-algebra.md) $\mathcal F_n=\sigma(A_1,\ldots,A_n)$ is partitioned by the nonempty [events](../../../../../../event.md)

$$
C=\bigcap_{j=1}^n B_j,
\qquad B_j\in\{A_j,A_j^c\}.
$$

These are its [atoms](../../../../../../atom-of-a-sigma-algebra.md). Define the [random variable](../../../../../../random-variable-split.md)

$$
X_n=\sum_{C:\,\mathbb P(C)>0}
\frac{\mathbb E[X\mathbf1_C]}{\mathbb P(C)}\mathbf1_C,
$$

and give it any finite value on the union of the null atoms. It is $\mathcal F_n$-measurable and [integrable](../../../../../../lebesgue-integrable-function.md). Every $A\in\mathcal F_n$ is a union of atoms, so

$$
\mathbb E[X_n\mathbf1_A]
=\sum_{C\subseteq A}\mathbb E[X\mathbf1_C]
=\mathbb E[X\mathbf1_A].
$$

This constructs the requested variable directly, without invoking the general existence theorem for [conditional expectation](../../../../../../conditional-expectation.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
