<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Backtracking](../../../../../backtracking.md) assigns one [variable](../../../../../variable-mathematics.md) at a time and abandons a partial assignment as soon as it cannot extend to a solution. With [forward checking](../../../../../forward-checking.md), placing a knight deletes its occupied and attacked squares from every remaining knight's [constraint domain](../../../../../constraint-domain.md). An empty [constraint domain](../../../../../constraint-domain.md) rejects the branch immediately; stronger [constraint propagation](../../../../../constraint-propagation.md), such as [arc consistency](../../../../../arc-consistency.md), can detect additional incompatibilities among future choices.

This combines early rejection with depth-first storage. It retains the current assignment and domain changes rather than the entire breadth-first layer of partial placements. A direct knight-variable implementation uses $O(kn^2)$ space for explicit domains, plus its assignment and restoration trail, instead of an exponentially large [breadth-first search](../../../../../breadth-first-search.md) [search frontier](../../../../../search-frontier.md). Propagation has a computational cost and does not guarantee improvement on every input, but often prevents exploration of vast inconsistent subtrees.

The **[minimum remaining values heuristic](../../../../../minimum-remaining-values-heuristic.md)** selects an unassigned [variable](../../../../../variable-mathematics.md) with the fewest currently legal values, exposing the likeliest failure first. The **[degree heuristic](../../../../../degree-heuristic.md)** selects a [variable](../../../../../variable-mathematics.md) constrained to the largest number of other unassigned [variables](../../../../../variable-mathematics.md), often breaking [minimum remaining values heuristic](../../../../../minimum-remaining-values-heuristic.md) ties. Degree is measured in the remaining [constraint graph](../../../../../constraint-graph.md), not by counting assigned neighbors. In the symmetric knight-variable encoding the remaining degrees can all tie, so the heuristic need not discriminate there.[§2.4, Minimum Remaining Values: choose an unassigned variable with the fewest valid remaining values](../../../../../cs-188-constraint-ordering-and-structure-notes.md)

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
