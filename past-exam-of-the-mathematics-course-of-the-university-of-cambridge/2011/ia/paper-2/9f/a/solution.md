<h1 id="9f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

By the definition of [conditional probability](../../../../../../conditional-probability.md),

$$
\mathbb P(B_i\mid A)=\frac{\mathbb P(A\cap B_i)}{\mathbb P(A)}
=\frac{\mathbb P(A\mid B_i)\mathbb P(B_i)}{\mathbb P(A)}.
$$

Since the $B_j$ form a disjoint partition of the [sample space](../../../../../../sample-space.md), the [law of total probability](../../../../../../law-of-total-probability.md) gives $\mathbb P(A)=\sum_j\mathbb P(A\mid B_j)\mathbb P(B_j)$. Substitution proves [Bayes' theorem](../../../../../../bayes-theorem.md) in the required form:

$$
\boxed{\mathbb P(B_i\mid A)=
\frac{\mathbb P(A\mid B_i)\mathbb P(B_i)}
{\sum_j\mathbb P(A\mid B_j)\mathbb P(B_j)}.}
$$

The hypotheses make the denominator positive and each conditioning probability well defined.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [9F](../../9f.md)
3. [Section II](../../section-ii.md)
4. [Paper 2](../../../paper-2-split.md)
5. [Ia](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
