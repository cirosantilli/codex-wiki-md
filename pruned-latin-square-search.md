# Pruned Latin square search

↑ **Parent:** [Latin square enumeration](latin-square-enumeration.md)

Build a [Latin square](latin-square.md) row by row, maintaining the symbols already used in each column. While choosing a row, remove each selected symbol from the row's available pool and reject any symbol already used in that column. The [invariant](invariant-mathematics.md) proves every complete output valid. Conversely every valid target row survives the checks, proving completeness by [induction](mathematical-induction.md). A partial branch may still have no completion; avoiding complete invalid outputs does not mean every explored [list prefix](prefix-of-a-list.md) is extendable.

## ↑ Ancestors (9)

1. [Latin square enumeration](latin-square-enumeration.md)
2. [Latin square](latin-square.md)
3. [Design of experiments](design-of-experiments-split.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
