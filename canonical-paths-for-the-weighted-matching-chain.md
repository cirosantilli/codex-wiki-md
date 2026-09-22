# Canonical paths for the weighted matching chain

↑ **Parent:** [Weighted matching Markov chain](weighted-matching-markov-chain.md)

Here the [graph](graph-split.md) has $2n$ [vertices](vertex-graph-theory.md) and $m\geq1$ [edges](edge-of-a-graph.md). The bound is a deliberately loose [canonical paths Poincare bound](canonical-paths-poincare-bound.md), sufficient for polynomial [mixing time](mixing-time-of-a-markov-chain.md) when both activity and reciprocal activity are polynomially bounded. Order the alternating [graph paths](path-in-a-graph.md) and cycles of $I\triangle F$ canonically. Convert each component from initial [matching in a graph](matching-graph-theory.md) $I$ to final [matching in a graph](matching-graph-theory.md) $F$ by moving an unmatched endpoint using exchanges; open a cycle with one deletion and finish it with one addition.

At an intermediate [matching in a graph](matching-graph-theory.md) $M$, the complementary encoding $K=I\triangle F\triangle M$ is a [matching in a graph](matching-graph-theory.md) away from the active component and has at most two degree-two [vertices](vertex-graph-theory.md). Remove at most two [edges](edge-of-a-graph.md) to obtain a [matching in a graph](matching-graph-theory.md) $K'$. Record those [edges](edge-of-a-graph.md) and one bit selecting the initial alternating colour on the active component. For a fixed directed transition this data reconstructs $K$, $I\triangle F$, the active component and its ordering, and then $I,F$; common [edges](edge-of-a-graph.md) are $M\cap K$. There are at most $2(m+1)^2$ auxiliary records per $K'$.

If $d=|K|-|K'|\leq2$, then $\pi_\lambda(I)\pi_\lambda(F)=\lambda^d\pi_\lambda(M)\pi_\lambda(K')$. The transition capacity is at least $\pi_\lambda(M)/(2m\max(\lambda,\lambda^{-1}))$, and the [path](continuous-path.md) length is at most $4n$. Summing over the injective encodings proves the displayed [path congestion](path-congestion.md) bound.

## ↑ Ancestors (9)

1. [Weighted matching Markov chain](weighted-matching-markov-chain.md)
2. [Reversible Markov chain](reversible-markov-chain.md)
3. [Markov chain](markov-chain.md)
4. [Markov process](markov-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-13/1/solution.md)
