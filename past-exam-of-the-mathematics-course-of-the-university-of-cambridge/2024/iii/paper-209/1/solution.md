<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Harris-FKG inequality](../../../../../harris-fkg-inequality.md) gives

$$
\mathbb P(X\in A\cap B)\geq
\mathbb P(X\in A)\mathbb P(X\in B).
$$

Here is an induction proof of the product-measure version, also called [Harris' inequality](../../../../../harris-inequality.md). The result is immediate for one coordinate. For $n$ coordinates, define

$$
a_j=\mathbb P(A\mid X_n=j),
\qquad
b_j=\mathbb P(B\mid X_n=j),
\qquad j\in\{0,1\}.
$$

The sections of an [increasing event](../../../../../increasing-event.md) are increasing events in the first $n-1$ coordinates, so the induction hypothesis gives

$$
\mathbb P(A\cap B)
\geq(1-p_n)a_0b_0+p_na_1b_1.
$$

Monotonicity gives $a_1\geq a_0$ and $b_1\geq b_0$. The difference between the right side and

$$
\mathbb P(A)\mathbb P(B)
=\bigl((1-p_n)a_0+p_na_1\bigr)
\bigl((1-p_n)b_0+p_nb_1\bigr)
$$

is

$$
p_n(1-p_n)(a_1-a_0)(b_1-b_0)\geq0.
$$

This closes the induction and proves positive association.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 209](../../paper-209-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
