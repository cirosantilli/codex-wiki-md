<h1 id="16h/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Part (b) proves one implication. Conversely, assume in ZF that

$$
\kappa^2=\kappa
$$

for every infinite cardinal $\kappa$. Let $X$ be any set and let $\gamma=h(X)$ be its Hartogs ordinal. Finite $X$ is already well-orderable, so suppose $X$ is infinite and form the [disjoint union](../../../../../../disjoint-union.md)

$$
A=X\sqcup\gamma.
$$

By hypothesis, $A\times A$ is bijective with $A$. Since $\gamma\times X$ injects into $A\times A$, we obtain

$$
|\gamma|\,|X|\leq|\gamma|+|X|.
$$

Apply part (c), with $K=\gamma$ and $L=X$. It gives either an injection $\gamma\to X$ or a surjection $s:\gamma\to X$. The first alternative contradicts [Hartogs theorem](../../../../../../hartogs-theorem.md). In the second, every fiber $s^{-1}(\{x\})$ is a nonempty set of ordinals and therefore has a least member. The map

$$
x\longmapsto\min s^{-1}(\{x\})
$$

is an injection of $X$ into the ordinal $\gamma$ and pulls its well-order back to $X$. Thus every set is well-orderable, so the [well-ordering theorem](../../../../../../well-ordering-theorem.md) gives the [axiom of choice](../../../../../../axiom-of-choice.md). This proves the [Tarski cardinal-square theorem](../../../../../../tarski-cardinal-square-theorem.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [16H](../../16h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
