# Backward search

↑ **Parent:** [String-searching algorithm](string-searching-algorithm.md)

[Backward search](backward-search.md) finds a query's matching interval in a [suffix array](suffix-array.md) by processing the query from right to left. With inclusive one-based interval $[l,r]$, prepending $c$ changes it to $[C(c)+\operatorname{Occ}(c,l-1)+1,C(c)+\operatorname{Occ}(c,r)]$. An empty interval means no match. This works through the occurrence-order property of the [last-to-first mapping](last-to-first-mapping.md).[§3.1, Figure 1, BW Search](opportunistic-data-structures-with-applications-by-paolo-ferragina-and-others.md)

## ↑ Ancestors (4)

1. [String-searching algorithm](string-searching-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Backward search](backward-search.md)
- [Burrows-Wheeler transform](burrows-wheeler-transform.md)
- [FM-index](fm-index.md)
- [Opportunistic Data Structures with Applications by Paolo Ferragina and others](opportunistic-data-structures-with-applications-by-paolo-ferragina-and-others.md)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-2/1/c/solution.md)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-2/1/d/solution.md)
