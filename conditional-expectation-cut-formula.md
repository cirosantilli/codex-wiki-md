# Conditional expectation cut formula

↑ **Parent:** [Conditional expectations for maximum cut](conditional-expectations-for-maximum-cut.md)

For any partial assignment $P$, let $f(P)$ count [edges](edge-of-a-graph.md) whose two endpoints are already fixed on opposite sides, and let $u(P)$ count [edges](edge-of-a-graph.md) with at least one unassigned endpoint. Under the remaining [independent](independent-random-variables.md) fair [bits](bit.md),

$$
q(P)=\mathbb E[C\mid P]=f(P)+\frac{u(P)}2.
$$

An [edge](edge-of-a-graph.md) with fixed equal labels contributes zero; fixed unequal labels contribute one. If one endpoint is unassigned, its fair [bit](bit.md) disagrees with the fixed label with [probability](probability.md) $1/2$. If both endpoints are unassigned, their [independent](independent-random-variables.md) fair [bits](bit.md) disagree with [probability](probability.md) $1/2$ as well. Count each unresolved [edge](edge-of-a-graph.md) once, even when both endpoints are unassigned.

Process [vertices](vertex-graph-theory.md) in a fixed order. Evaluate the [conditional expectation cut formula](conditional-expectation-cut-formula.md) after setting the next label to zero and after setting it to one; retain the larger value, choosing zero on ties. The [conditional expectation choice invariant](conditional-expectation-choice-invariant.md) ensures the final [cut of a graph](cut-graph-theory.md) has size at least $m/2$. This is a deterministic [approximation algorithm](approximation-algorithm.md) for [maximum cut](maximum-cut.md).[CS 4820: Algorithms, Spring 2011; Cornell CS 4820, Lecture notes on randomized approximation algorithms, 2 May 2011, §1.1.2, printed pp. 2–3: conditional expectations, Algorithms 1–2 and the half-total-edge-weight guarantee; no individual byline stated](cs-4820-algorithms-spring-2011/lecture-notes-on-randomized-approximation-algorithms.md)

## ↑ Ancestors (7)

1. [Conditional expectations for maximum cut](conditional-expectations-for-maximum-cut.md)
2. [Method of conditional probabilities](method-of-conditional-probabilities.md)
3. [Derandomization](derandomization.md)
4. [Randomized algorithm](randomized-algorithm.md)
5. [Algorithm](algorithm-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Conditional expectation cut formula](conditional-expectation-cut-formula.md)
- [Conditional expectations algorithm cost](conditional-expectations-algorithm-cost.md)
- [Conditional expectations cut example](conditional-expectations-cut-example.md)
