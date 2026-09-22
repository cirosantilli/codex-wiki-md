# Pairwise intersections need not give a common intersection

↑ **Parent:** [Clique (graph theory)](clique-graph-theory.md)

A [clique](clique-graph-theory.md) records pairwise relationships. If [vertices](vertex-graph-theory.md) represent [sets](set-split.md) and an [edge](edge-of-a-graph.md) means a nonempty [intersection](set-intersection.md), a [clique](clique-graph-theory.md) does not by itself guarantee an element common to every [set](set-split.md). Take

$$
A=\{1,2\},\qquad B=\{2,3\},\qquad C=\{1,3\}.
$$

Then $A\cap B=\{2\}$, $B\cap C=\{3\}$ and $C\cap A=\{1\}$, so their [intersection graph](intersection-graph.md) is $K_3$. But $A\cap B\cap C=\varnothing$. The [graph](graph-split.md) faithfully records all three pairwise intersections; the stronger claim of a single shared element requires additional hypotheses.

## ↑ Ancestors (7)

1. [Clique (graph theory)](clique-graph-theory.md)
2. [Complete graph](complete-graph.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
