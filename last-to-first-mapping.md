# Last-to-first mapping

↑ **Parent:** [String-searching algorithm](string-searching-algorithm.md)

In a sorted [cyclic rotation](cyclic-rotation.md) matrix, the [last-to-first mapping](last-to-first-mapping.md) sends the $k$th occurrence of a character in the last column to its $k$th occurrence in the first column. For one-based rows, $\operatorname{LF}(r)=C(L_r)+\operatorname{Occ}(L_r,r)$, where $C(c)$ counts smaller characters and $\operatorname{Occ}(c,r)$ counts $c$ in the first $r$ entries of the last column. It moves a rotation's start one character backwards cyclically. Equal characters retain the [lexicographic order](lexicographic-order.md) of their following sequences, which proves the occurrence-order rule.[§2, properties (a)–(b) and LF-mapping](opportunistic-data-structures-with-applications-by-paolo-ferragina-and-others.md)

## ↑ Ancestors (4)

1. [String-searching algorithm](string-searching-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Backward search](backward-search.md)
- [Burrows-Wheeler transform](burrows-wheeler-transform.md)
- [Last-to-first mapping](last-to-first-mapping.md)
- [Opportunistic Data Structures with Applications by Paolo Ferragina and others](opportunistic-data-structures-with-applications-by-paolo-ferragina-and-others.md)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-2/1/c/solution.md)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-2/1/d/solution.md)
