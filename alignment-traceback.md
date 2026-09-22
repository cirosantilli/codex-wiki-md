# Alignment traceback

↑ **Parent:** [Sequence alignment](sequence-alignment.md)

Store a maximizing predecessor at each [dynamic programming](dynamic-programming.md) table entry. A diagonal predecessor emits a pair of letters; a vertical or horizontal predecessor emits a letter opposite a gap. Construct the columns in reverse and then reverse the output. For [global sequence alignment without mismatches](global-sequence-alignment-without-mismatches.md), start at the full-prefix entry and stop at the origin. For [local sequence alignment without mismatches](local-sequence-alignment-without-mismatches.md), start at any largest entry and stop at a zero entry. Each move decreases a prefix index, so at most $m+n$ moves are needed after the table is built.

## ↑ Ancestors (5)

1. [Sequence alignment](sequence-alignment.md)
2. [Molecular genetics](molecular-genetics-split.md)
3. [Genetics](genetics-split.md)
4. [Biology](biology-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Global sequence alignment without mismatches](global-sequence-alignment-without-mismatches.md)
- [Local sequence alignment without mismatches](local-sequence-alignment-without-mismatches.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/8/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/8/e/solution.md)
