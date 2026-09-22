# Greedy algorithm

↑ **Parent:** [Algorithm](algorithm-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Greedy_algorithm)

A [greedy algorithm](greedy-algorithm.md) builds a [feasible solution](feasible-point.md) by repeatedly committing to a locally preferred next choice. Each commitment is final: the [algorithm](algorithm-split.md) does not revisit it when later choices become available. In [mathematical optimization](mathematical-optimization-split.md), the important question is whether those commitments can still attain the best [objective function](objective-function.md) value.

For example, a shared telescope can accept several observation requests with fixed time slots. In [interval scheduling](interval-scheduling.md), every completed request counts equally, and overlapping requests cannot both be accepted. Choosing the request that finishes earliest leaves the resource available sooner. The example below turns that intuition into a precise rule, then shows why choosing the earliest start or shortest duration can lose jobs.

[Greedy algorithms](greedy-algorithm.md) are attractive because a single pass can replace a search through many candidate [subsets](subset.md). However, "locally best" is only a design proposal. A problem-specific [greedy-choice property](greedy-choice-property.md), often established by an [exchange argument](exchange-argument.md), must connect the local decision to the actual [objective function](objective-function.md). The largest-individual-value rule in the [0-1 knapsack problem](0-1-knapsack-problem.md) fails; [Dijkstra's algorithm](dijkstra-algorithm.md) needs its nonnegative-edge assumptions. A rule's success in one [optimization](mathematical-optimization-split.md) task does not justify it in another.

**Table of contents**

- [Greedy-choice property](greedy-choice-property.md)
  - [Exchange argument](exchange-argument.md)
- [Interval scheduling](interval-scheduling.md)
  - [Shortest-duration interval scheduling counterexample](shortest-duration-interval-scheduling-counterexample.md)
  - [Weighted interval scheduling](weighted-interval-scheduling.md)

## ↑ Ancestors (3)

1. [Algorithm](algorithm-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Dynamic programming](dynamic-programming.md)
- [Finite greedy basis extension and choice](finite-greedy-basis-extension-and-choice.md)
- [Graphic matroid](graphic-matroid.md)
- [Greedy algorithm](greedy-algorithm.md)
- [Greedy matching](greedy-matching.md)
- [Hereditary nonmatroid greedy obstruction](hereditary-nonmatroid-greedy-obstruction.md)
- [Huffman coding](huffman-coding.md)
- [Independence system](independence-system.md)
- [Interval scheduling](interval-scheduling.md)
- [Kruskal's algorithm](kruskal-s-algorithm.md)
- [Lagrange's four-square theorem](lagrange-s-four-square-theorem.md)
- [Maximal matching](maximal-matching.md)
- [Perfect elimination ordering](perfect-elimination-ordering.md)
