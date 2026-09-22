# Snapshot representatives before quick-find union

↑ **Parent:** [Disjoint-set union operation](disjoint-set-union-operation.md)

When merging two blocks in [quick-find](quick-find.md), let $a=rep_0(x)$ and $b=rep_0(y)$ be fixed saved labels. Replacing every old occurrence of $b$ by $a$ preserves all other blocks. A scan [loop invariant](loop-invariant.md) says processed cells already have their specified final labels while unprocessed cells still have their old labels. Recomputing $rep(y)$ during this mutation can change the replacement label after the cell for $y$ is processed, causing remaining old-$b$ cells to be missed. Saving both labels makes the update criterion stable and the invariant provable.

## ↑ Ancestors (5)

1. [Disjoint-set union operation](disjoint-set-union-operation.md)
2. [Disjoint-set data structure](disjoint-set-data-structure.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)
