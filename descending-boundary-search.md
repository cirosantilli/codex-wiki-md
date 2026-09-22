# Descending boundary search

↑ **Parent:** [Binary search](binary-search.md)

For a nonincreasing [array](array-data-structure.md), maintain indices $0\leq a\leq b\leq n$ such that entries before $a$ exceed the target and entries from $b$ onward are at most the target. Probe the middle of the half-open interval. A value above the target advances $a$ past that index; otherwise [set](set-split.md) $b$ to that index. The interval length decreases geometrically. At termination the common boundary is the first possible match, so one guarded equality test decides presence even with duplicates.

## ↑ Ancestors (4)

1. [Binary search](binary-search.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
