<h1 id="9f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $\mathbb P(B)>0$, the [conditional probability](../../../../../../conditional-probability.md) is $\mathbb P(A\mid B)=\mathbb P(A\cap B)/\mathbb P(B)$. Since the [events](../../../../../../event.md) $B_i$ partition the [sample space](../../../../../../sample-space.md), their intersections with $A$ are disjoint and exhaust $A$. The [law of total probability](../../../../../../law-of-total-probability.md) therefore gives $\mathbb P(A)=\sum_j\mathbb P(A\mid B_j)\mathbb P(B_j)$. Substituting this and $\mathbb P(A\cap B_i)=\mathbb P(A\mid B_i)\mathbb P(B_i)$ into the definition proves [Bayes' theorem](../../../../../../bayes-theorem.md):

$$
\boxed{\mathbb P(B_i\mid A)=\frac{\mathbb P(A\mid B_i)\mathbb P(B_i)}{\sum_j\mathbb P(A\mid B_j)\mathbb P(B_j)}.}
$$

The denominator is positive by the given hypothesis on $A$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9F](../../9f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
