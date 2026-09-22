# Greedy matching

↑ **Parent:** [Maximal matching](maximal-matching.md)

A [greedy matching](greedy-matching.md) starts with the empty [matching in a graph](matching-graph-theory-split.md), scans all [edges](edge-of-a-graph.md) in some order, and selects an [edge](edge-of-a-graph.md) exactly when both endpoints are [unmatched vertices in a matching](unmatched-vertex-in-a-matching.md). For a finite [graph](graph-split.md), a complete scan returns a [maximal matching](maximal-matching.md): a rejected [edge](edge-of-a-graph.md) had a matched endpoint, which stays matched thereafter. Stopping before all [edges](edge-of-a-graph.md) have been considered need not give maximality. Changing the order can change the result; on P₄, middle-first gives one pair, whereas outer-first gives two. A [greedy algorithm](greedy-algorithm.md) of this form never revisits its choices, while an [augmenting path in a matching](augmenting-path-in-a-matching.md) does.

## ↑ Ancestors (7)

1. [Maximal matching](maximal-matching.md)
2. [Matching (graph theory)](matching-graph-theory-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Augmenting path in a matching](augmenting-path-in-a-matching.md)
- [Greedy matching](greedy-matching.md)
- [Matching (graph theory)](matching-graph-theory-split.md)
