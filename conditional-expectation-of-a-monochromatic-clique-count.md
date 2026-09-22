# Conditional expectation of a monochromatic clique count

↑ **Parent:** [Method of conditional probabilities](method-of-conditional-probabilities.md)

In a partially fixed two-colour [edge coloring](edge-coloring.md) of a [complete graph](complete-graph.md), complete all unassigned [edges](edge-of-a-graph.md) independently and fairly. For a fixed [clique](clique-graph-theory.md) with $r$ unassigned [edges](edge-of-a-graph.md), its [conditional probability](conditional-probability.md) of becoming [monochromatic](monochromatic-set.md) is zero if both colours already occur; $2^{-r}$ if a colour is fixed and no conflicting colour occurs; and $2^{1-r}$ if none is fixed. Sum these [conditional probabilities](conditional-probability.md) over the [cliques](clique-graph-theory.md) to obtain a computable [conditional expectation](conditional-expectation.md). Fix each next [edge](edge-of-a-graph.md) to a colour that does not increase this [conditional expectation](conditional-expectation.md), yielding a deterministic minimization construction.

## ↑ Ancestors (6)

1. [Method of conditional probabilities](method-of-conditional-probabilities.md)
2. [Derandomization](derandomization.md)
3. [Randomized algorithm](randomized-algorithm.md)
4. [Algorithm](algorithm-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/probability-and-computing/3/f/solution.md)
