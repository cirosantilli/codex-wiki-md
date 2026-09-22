<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Apply the [Friedman–Moschovakis coding lemma](../../../../../../friedman-moschovakis-coding-lemma.md) with

$$
\lambda=\aleph_2.
$$

The given map $\pi:\omega^\omega\twoheadrightarrow\aleph_2$ supplies the required real codes for ordinals below $\lambda$, while each $g_\xi:\omega^\omega\twoheadrightarrow\mathcal P(\xi)$ supplies codes for all possible initial segments of a subset of $\lambda$.

For completeness, fix $A\subseteq\aleph_2$ and form the associated [Friedman–Moschovakis coding game](../../../../../../friedman-moschovakis-coding-game.md). The players use $\pi$ to announce ordinals and $g_\xi$ to announce candidate codes for $A\cap\xi$, while each may challenge the other's code at a larger ordinal. The Friedman–Moschovakis diagonal argument shows that Player I cannot have a winning strategy. By the [axiom of determinacy](../../../../../../axiom-of-determinacy.md), Player II has one. The coherence tests in the game ensure that a fixed winning strategy for II can belong to at most one set $A$: if it purported to code distinct $A$ and $B$, a play reaching an ordinal above the least point of disagreement would defeat it.

Every strategy for a game on $\omega$ is coded by a real. Define $F:\omega^\omega\to\mathcal P(\aleph_2)$ by sending a code for a winning II-strategy to the unique set that it determines, and sending all other reals to the empty set. Every $A\subseteq\aleph_2$ has such a strategy, so $F$ is surjective. Hence

$$
\boxed{\omega^\omega\twoheadrightarrow\mathcal P(\aleph_2).}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 158](../../../paper-158-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
