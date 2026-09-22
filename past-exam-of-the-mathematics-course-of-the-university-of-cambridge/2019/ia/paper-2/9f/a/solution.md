<h1 id="9f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Kolmogorov axioms](../../../../../../kolmogorov-axioms.md) for a [probability measure](../../../../../../probability-measure.md) $\mathbb P$ are nonnegativity, normalization $\mathbb P(\Omega)=1$, and [countable additivity](../../../../../../countable-additivity.md) on pairwise disjoint events. For $\mathbb P(B)>0$, [conditional probability](../../../../../../conditional-probability.md) is defined by

$$
\mathbb P(A\mid B)=\frac{\mathbb P(A\cap B)}{\mathbb P(B)}.
$$

Because the events $A\cap B_i$ are pairwise disjoint and their union is $A$, countable additivity gives the [law of total probability](../../../../../../law-of-total-probability.md)

$$
\mathbb P(A)=\sum_{i=1}^{\infty}\mathbb P(A\cap B_i)
=\sum_{i=1}^{\infty}\mathbb P(A\mid B_i)\mathbb P(B_i).
$$

For any $j$ with $\mathbb P(A)>0$, the definition of conditional probability and this identity give [Bayes' theorem](../../../../../../bayes-theorem.md):

$$
\boxed{\mathbb P(B_j\mid A)=
\frac{\mathbb P(A\mid B_j)\mathbb P(B_j)}
{\sum_i\mathbb P(A\mid B_i)\mathbb P(B_i)}}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9F](../../9f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
