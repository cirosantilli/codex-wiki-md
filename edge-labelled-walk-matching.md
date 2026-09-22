# Edge-labelled walk matching

↑ **Parent:** [Dynamic programming](dynamic-programming.md)

Given a finite [directed graph](directed-graph.md), an [edge](edge-of-a-graph.md) labelling and a finite target label sequence, [edge-labelled walk matching](edge-labelled-walk-matching.md) asks whether a [directed walk](directed-walk.md) spells that sequence. Begin with the designated start set and update reachable [vertices](vertex-graph-theory.md) one label at a time by the recurrence in the title. Appending a final matching [edge](edge-of-a-graph.md) proves the invariant by [induction](mathematical-induction.md). Repeated [vertices](vertex-graph-theory.md) are allowed; a requirement of a vertex-simple [directed path](directed-path.md) is a different problem and can encode [Hamiltonian path](hamiltonian-path.md). Scanning all [edges](edge-of-a-graph.md) and clearing a [vertex](vertex-graph-theory.md) layer costs $O(k(|V|+|E|))$ for $k$ labels.

**Table of contents**

- [Maximum-product edge-labelled walk](maximum-product-edge-labelled-walk.md)

## ↑ Ancestors (5)

1. [Dynamic programming](dynamic-programming.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Edge-labelled walk matching](edge-labelled-walk-matching.md)
- [Maximum-product edge-labelled walk](maximum-product-edge-labelled-walk.md)
