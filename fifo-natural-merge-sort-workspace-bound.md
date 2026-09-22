# FIFO natural merge sort workspace bound

↑ **Parent:** [Merge sort](merge-sort.md)

Repeatedly removing the first two [maximal initial runs](maximal-initial-run.md) and appending their sorted merge uses $\Theta(n\log n)$ total fresh output cells in the worst case if obsolete cells are never reused. Group merges into rounds that consume the runs present at the start: the run count is at least halved up to rounding, and each round writes at most $2n$ values. A tight-order family consists of $2^h$ copies of $[0,1]$: run boundaries never coalesce and every merging level writes $n=2^{h+1}$ entries. Its final append-only endpoint is exactly $n\log_2 n$.

## ↑ Ancestors (5)

1. [Merge sort](merge-sort.md)
2. [Sorting algorithm](sorting-algorithm.md)
3. [Algorithm](algorithm-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)
