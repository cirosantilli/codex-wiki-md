<h1 id="16f/solution">Solution</h1>

↑ **Parent:** [16F](../16f.md)

The [compactness theorem](../../../../../compactness-theorem.md) says that a set $T$ of [first-order sentences](../../../../../first-order-sentence.md) has a [model](../../../../../model-of-a-first-order-theory.md) if and only if every finite subset of $T$ has a model. One implication follows by taking the same model. Conversely, if $T$ had no model, then by the [Godel completeness theorem](../../../../../godel-s-completeness-theorem.md) it would prove a contradiction. A formal proof uses only finitely many assumptions, so some finite subset of $T$ would already have no model. This contradiction proves compactness.

The [Upward Lowenheim-Skolem theorem](../../../../../upward-lowenheim-skolem-theorem.md) says that if an $L$-theory $T$ has an infinite model, then it has models of arbitrarily large cardinality; more precisely, it has a model of cardinality at least $\kappa$ for every cardinal $\kappa$. Add new constants $c_\alpha$ for $\alpha<\kappa$ and the sentences

$$
c_\alpha\ne c_\beta\qquad(\alpha\ne\beta).
$$

Every finite subset of the enlarged theory can be interpreted in the given infinite model, since it mentions only finitely many constants. Compactness supplies a model of the whole enlarged theory, in which the $c_\alpha$ are pairwise distinct. Its reduct to $L$ is a model of $T$ having at least $\kappa$ elements. If $\kappa\geq|L|+\aleph_0$, the [Downward Lowenheim-Skolem theorem](../../../../../downward-lowenheim-skolem-theorem.md) gives a model of cardinality exactly $\kappa$.

## ↑ Ancestors (10)

1. [16F](../16f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
