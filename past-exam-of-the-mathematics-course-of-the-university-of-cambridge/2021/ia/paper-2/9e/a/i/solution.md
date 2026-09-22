<h1 id="9e/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $\mathbb P(B)>0$, the [conditional probability](../../../../../../../conditional-probability.md) is

$$
\mathbb P(A\mid B)
=\frac{\mathbb P(A\cap B)}{\mathbb P(B)}.
$$

Hence

$$
\mathbb P(B_j\mid A)
=\frac{\mathbb P(A\mid B_j)\mathbb P(B_j)}
{\mathbb P(A)}.
$$

Because the $B_k$ form a partition, the law of total probability gives

$$
\mathbb P(A)
=\sum_{k=1}^n\mathbb P(A\mid B_k)\mathbb P(B_k).
$$

Substitution proves [Bayes' theorem](../../../../../../../bayes-theorem.md) in the required form:

$$
\boxed{
\mathbb P(B_j\mid A)
=\frac{\mathbb P(A\mid B_j)\mathbb P(B_j)}
{\sum_{k=1}^n\mathbb P(A\mid B_k)\mathbb P(B_k)}}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [9E](../../../9e.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ia](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
