# Linear search correctness

↑ **Parent:** [Linear search](linear-search.md)

The [loop invariant](loop-invariant.md) just before inspecting index $i$ is: $0\leq i\leq n$, and no entry at an index $k<i$ matches $x$. Initially $i=0$, so there are no earlier entries. A failed [equality test](equality-test.md) extends the excluded region by one position and preserves the [loop invariant](loop-invariant.md). A successful [equality test](equality-test.md) at index $i$ establishes a match; the [loop invariant](loop-invariant.md) establishes that it is the first one. At exhaustion, $i=n$ and every entry has failed, so the absent result is correct. The number $n-i$ of remaining entries decreases after each failed [equality test](equality-test.md), proving termination for a finite [sequence](sequence.md). Together these establish [algorithm correctness](algorithm-correctness.md) under the assumptions that the [input](input-computer-science.md) is stable and each [equality test](equality-test.md) terminates. No step of the argument compares the relative order of values.

## ↑ Ancestors (4)

1. [Linear search](linear-search.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
