# Disjoint-set representative

↑ **Parent:** [Disjoint-set data structure](disjoint-set-data-structure.md)

A [disjoint-set representative](disjoint-set-representative.md) is a chosen member of a [block of a set partition](block-of-a-set-partition.md). It may be any member; it need not be the [minimum](minimum-of-a-subset-of-a-total-order.md), the first inserted member or a permanent identifier. A merge may change the [disjoint-set representative](disjoint-set-representative.md) of an existing member. At any one state, the required rule is

$$
\operatorname{find}(x)=\operatorname{find}(y)\quad\Longleftrightarrow\quad x,y\text{ belong to the same block}.
$$

If an application needs the [minimum](minimum-of-a-subset-of-a-total-order.md) member, store it separately with the [disjoint-set representative](disjoint-set-representative.md) and update that extra information on merging.

## ↑ Ancestors (4)

1. [Disjoint-set data structure](disjoint-set-data-structure.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Disjoint-set data structure](disjoint-set-data-structure.md)
- [Disjoint-set find operation](disjoint-set-find-operation.md)
- [Disjoint-set forest](disjoint-set-forest.md)
- [Disjoint-set representative](disjoint-set-representative.md)
- [Disjoint-set union operation](disjoint-set-union-operation.md)
- [Path compression](path-compression.md)
- [Union by rank](union-by-rank.md)
