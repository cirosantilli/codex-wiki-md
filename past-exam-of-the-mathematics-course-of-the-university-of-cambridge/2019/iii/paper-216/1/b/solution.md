<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The posterior mean of the number infected is

$$
\mathbb E\left[\sum_{i\in V}X_i\,middle|\,V_2\right]
=\sum_{i\in V}\mathbb P(X_i=1\mid V_2).
$$

Run [sum-product belief propagation](../../../../../../sum-product-belief-propagation.md) on the tree to compute every exact one-vertex posterior marginal. Summing their probabilities of state one gives the requested mean. Messages have fixed size and every directed edge is processed once, so the exact computation costs

$$
\boxed{O(|V|).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
