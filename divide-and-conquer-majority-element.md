# Divide-and-conquer majority element

↑ **Parent:** [Divide-and-conquer algorithm](divide-and-conquer-algorithm.md)

An entry occurring strictly more than half the time in an [array](array-data-structure.md) must occur strictly more than half the time in at least one half: otherwise the two frequency bounds sum to at most half the whole length. Recursively find each half's possible [majority element](majority-element.md), then verify at most two candidates over the whole subarray using only equality tests. [Induction](mathematical-induction.md) proves correctness, and linear combination work over a balanced [recursion](recursion-computer-science.md) tree gives worst-case $\Theta(n\log n)$ time. A tagged absent result avoids confusing failure with a valid element.

## ↑ Ancestors (4)

1. [Divide-and-conquer algorithm](divide-and-conquer-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
